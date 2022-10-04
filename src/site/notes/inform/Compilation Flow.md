---
{"dg-publish":true,"permalink":"/inform/compilation-flow/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Compilation Flow
- A vague overview of the flow because it’s too many links back and forth.

## Build setup
- [[inform/Main|Main]] is the entry point.
	- Maybe there’s some stuff with [[inform/foundation|foundation]].
	- This then goes to [[inform/Inbuild Control|Inbuild Control]] for the setup of the project.
		- Which creates objects from [[inform/Project File Manager|Project File Manager]] and [[inform/Project Bundle Manager|Project Bundle Manager]].
		- And all the various build skill/step modules.
	- The [[inform/Inform7 Skill|Inform7 Skill]] is the final part of [[inform/supervisor|supervisor]] we use for now, which goes to [[inform/core|core]] via `Task::carry_out` in [[inform/What To Compile|What To Compile]] and then [[inform/How To Compile|How To Compile]] which has the actual passes.
## Reading and Lexing
- In [[inform/Project Services|Project Services]] there is `Projects::read_source_text_for` which does the lexing and sentence breaking.
	- The lexing is through [[inform/Source Text|Source Text]] → [[inform/Text From Files|Text From Files]] → [[inform/Lexer|Lexer]].
		- After this, we have:
			- A `source_file` with a bunch of individual words (with location metadata) and some file-level metadata.
			- A “vocabulary map” of some kind, though at this point we haven’t done any meaning analysis (other than checking if it’s an `ING_MC` and some basic numeric parsing).
	- The sentence breaking is just [[Sentences|Sentences]] directly. This has some rudimentary parsing.
		- The docs call this now a syntax tree, even though it’s just a tree of `SENTENCE_NT` nodes arranged under their respective [[Headings|Headings]].
		- [[Syntax Trees|Syntax Trees]] has the actual tree structure (it seems to be different to the norm with the “budding” and amending other trees to each other).
- Technically this is all *before* the [[inform/Inform7 Skill|Inform7 Skill]].

## Passes
- At this point we have sentences, but with a few minor exceptions they are all unparsed. There’s 3 major passes, all of which are in [[Passes through Major Nodes|Passes through Major Nodes]] in [[inform/assertions|assertions]].
- After the second pass there is `traverse_to_stock` in [[Tables (assertions)|Tables (assertions)]] and some [[Dialogue|Dialogue]] stuff.
- I think at this point the parsing is primarily done and we have a list of assertions about the world.

## Model World Building
- Base kinds are made; apparently this is in [[Kind Declarations|Kind Declarations]] in [[inform/runtime|runtime]] which seems awfully late? Maybe by building it means building it in inter?
- We go back to [[inform/assertions|assertions]] for the “late namings” in [[Translation Requests|Translation Requests]]. I have no idea what this is yet. [[Inform TODO list|Inform TODO list]].
- `OrderingInstances::objects_in_definition_sequence` is in [[inform/knowledge|knowledge]] → [[inform/Ordering Instances|Ordering Instances]].
- For some reason there simply isn’t a `Stage I` of the world building in this part, and `Stage II and III` are put together. Oh, and `Stage V` is later on.
- Stages II, III, and IV are in (whoever could guess this) [[inform/knowledge|knowledge]] → [[inform/The Model World|The Model World]].
	- I need to work out what these actually are.

## Tables and Grammar
- `Measurements::validate_definitions` is in [[inform/knowledge|knowledge]] → [[inform/Measurements|Measurements]].
- `BinaryPredicateFamilies::second_stock` is in [[inform/calculus|calculus]] → [[Binary Predicate Families|Binary Predicate Families]].
- `Tables::check_tables_for_kind_clashes` is in [[inform/assertions|assertions]] → [[Tables (assertions)|Tables (assertions)]].

We then have a couple more model world checks which need to come after the tables for…whatever reason? I guess because we need some predicates before we can do the last stage?

- `World::stage_V` is in [[inform/knowledge|knowledge]] → [[inform/The Model World|The Model World]].
- `MappingHints::traverse_for_map_parameters` is in [[inform/if|if]] → [[Mapping Hint Requests|Mapping Hint Requests]].

## Phrases and Rules
- `LiteralPatterns::define_named_phrases` is in [[inform/values|values]] → [[Literal Patterns (values)|Literal Patterns (values)]].
- `ImperativeDefinitions::assess_all` is in [[inform/assertions|assertions]] → [[Imperative Definitions|Imperative Definitions]].
- `Equations::traverse_to_stock` is in [[inform/assertions|assertions]] → [[Equations (assertions)|Equations (assertions)]].
- Another call to `Tables::traverse_to_stock` because I guess we have more information than the second pass? [[Tables (assertions)|Tables (assertions)]].
- `RTRulebooks::RulebookOutcomePrintingRule` is in [[inform/runtime|runtime]] → [[Rulebooks (runtime)|Rulebooks (runtime)]].

This is the end of the actual compiler, I think. At this point we have a fully stocked AST and other various symbol tables and the like.

# Inter
Why does part 4 do literally nothing?

### Part 1
- `RTUseOptions::compile` is in [[inform/runtime|runtime]] → [[Use Options (runtime)|Use Options (runtime)]].
- `RTCommandGrammars::compile_non_generic_constants` is in [[inform/runtime|runtime]] → [[Command Grammars|Command Grammars]].
- `Interventions::make_all` is in [[inform/runtime|runtime]] → [[Interventions|Interventions]].
- `RTKindConstructors::compile` is in [[inform/runtime|runtime]] → [[Kind Constructors|Kind Constructors]].
- `RTLiteralPatterns::compile` is in [[inform/runtime|runtime]] → [[Literal Patterns (runtime)|Literal Patterns (runtime)]].

### Part 2
- `CompletionModule::compile` is in [[inform/runtime|runtime]] → [[Completion Module|Completion Module]].
- `RTProperties::compile` is in [[inform/runtime|runtime]] → [[Properties (runtime)|Properties (runtime)]]
- `RTKindConstructors::compile_permissions` is in [[inform/runtime|runtime]] → [[Kind Constructors|Kind Constructors]].
- `InferenceSubjects::emit_all` is in [[inform/knowledge|knowledge]] → [[inform/Inference Subjects|Inference Subjects]].
- `Tables::complete` is in [[inform/assertions|assertions]] → [[Tables (assertions)|Tables (assertions)]].
- `RTTables::compile` is in [[inform/runtime|runtime]] → [[Tables (runtime)|Tables (runtime)]].
- `RTTableColumns::compile` is in [[inform/runtime|runtime]] → [[Table Columns (runtime)|Table Columns (runtime)]].
- `RTEquations::compile` is in [[inform/runtime|runtime]] → [[Equations (runtime)|Equations (runtime)]].
- `ImperativeDefinitions::compile_first_block` is in [[inform/assertions|assertions]] → [[Imperative Definitions|Imperative Definitions]].
- `RTDialogueBeats::compile` - [[Dialogue|Dialogue]].
- RTDialogueLines::compile - [[Dialogue|Dialogue]].
- RTDialogueChoices::compile - [[Dialogue|Dialogue]].
- `RTRules::compile` is in [[inform/runtime|runtime]] → [[Rules (runtime)|Rules (runtime)]].
- `RTRulebooks::compile` is in [[inform/runtime|runtime]] → [[Rulebooks (runtime)|Rulebooks (runtime)]].
- `RTRulebooks::compile_nros` is also in [[inform/runtime|runtime]] → [[Rulebooks (runtime)|Rulebooks (runtime)]].
- `RTActivities::compile` is in [[inform/runtime|runtime]] → [[Activities (runtime)|Activities (runtime)]].
- `RTVerbs::compile_conjugations` is in [[inform/runtime|runtime]] → [[Conjugations|Conjugations]].
- `RTVerbs::compile_forms` is in [[inform/runtime|runtime]] → [[Conjugations|Conjugations]] too.
- `CompilationUnits::complete_metadata` - [[Inform TODO list|Inform TODO list]].

### Parts 3 and 5
- `PhraseRequests::invoke_to_begin` is in [[inform/imperative|imperative]] → [[Phrase Requests|Phrase Requests]].
- `Closures::compile_closures` is in [[inform/imperative|imperative]] → [[Closures|Closures]].
- `RTRelations::compile` is in [[inform/runtime|runtime]] → [[inform/Relations|Relations]].
- `RTAdjectives::compile_mdef_test_functions` is in [[inform/runtime|runtime]] → [[Adjectives|Adjectives]]. 
- `RTPhrasebook::compile_entries` is in [[inform/runtime|runtime]] → [[Phrasebook Index|Phrasebook Index]].
- `RTMappingHints::compile` is in [[inform/runtime|runtime]] → [[Mapping Hints|Mapping Hints]].
- `RTKindIDs::compile_structures` is in [[inform/runtime|runtime]] → [[Kind IDs|Kind IDs]].
- `TheHeap::compile_configuration` is in [[inform/runtime|runtime]] → [[The Heap|The Heap]].
- `Rules::check_response_usages` is in [[inform/assertions|assertions]] → [[Rules (assertions)|Rules (assertions)]].
- `LocalParking::compile_array` is in [[inform/imperative|imperative]] → [[Local Parking|Local Parking]].
- `RTBibliographicData::IFID_text` is in [[inform/runtime|runtime]] → [[Bibliographic Data|Bibliographic Data]].

I’ve dropped the many calls to `Sequence::undertake_queued_tasks`.

## Index

We’re finally done. [[Inform TODO list|Inform TODO list]]
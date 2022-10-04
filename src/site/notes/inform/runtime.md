---
{"dg-publish":true,"permalink":"/inform/runtime/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# runtime
```ad-info
Link: [https://ganelson.github.io/inform/runtime-module/index.html](https://ganelson.github.io/inform/runtime-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```



# Contents
- Chapter 1: Configuration and Control
    - [[Runtime Module|Runtime Module]]https://ganelson.github.io/inform/runtime-module/1-rm.html - Setting up the use of this module.
-   Chapter 2: Emission
    - [[Hierarchy|Hierarchy]]https://ganelson.github.io/inform/runtime-module/2-hrr.html - To provide an enforced structure and set of naming conventions for packages and names in the Inter code we generate.
    - [[Noun Identifiers|Noun Identifiers]]https://ganelson.github.io/inform/runtime-module/2-ni.html - Instances and kinds are both referred to by nouns, and here we create corresponding inames for use in compiled Inter code, and identifiers for use in the index.
    - [[Compilation Units|Compilation Units]]https://ganelson.github.io/inform/runtime-module/2-cu.html - The source text is divided into compilation units, and the material they lead to is similarly divided up.
    - [[Emit|Emit]]https://ganelson.github.io/inform/runtime-module/2-emt.html - "Emitting" is the process of generating Inter bytecode, and this section provides a comprehensive API for the runtime and imperative modules to do that.
    - [[Emit Code|Emit Code]]https://ganelson.github.io/inform/runtime-module/2-ec.html - Here is how bytecode for instructions inside functions is emitted.
    - [[Emit Arrays|Emit Arrays]]https://ganelson.github.io/inform/runtime-module/2-ea.html - Here is how bytecode to create ready-initialised arrays of Inter data is emitted.
    - [[Interventions|Interventions]]https://ganelson.github.io/inform/runtime-module/2-int.html - Material written in low-level Inform 6 notation can be emitted for later linking, a distasteful process called "intervening".
    - [[Shared Variables (runtime)|Shared Variables (runtime)]]https://ganelson.github.io/inform/runtime-module/2-sv.html - Functions to create sets of shared variables.
    - [[The Heap|The Heap]]https://ganelson.github.io/inform/runtime-module/2-th.html - Texts, lists and other flexibly-sized structures make use of a pool of run-time storage called "the heap".
    - [[Default Values|Default Values]]https://ganelson.github.io/inform/runtime-module/2-dv.html - An unusual feature of Inform is that every kind has a default value, so that it is impossible for any variable or property to be uninitialised.
    - [[Equality Schemas|Equality Schemas]]https://ganelson.github.io/inform/runtime-module/2-es.html - To define how to compile a comparison of two values.
    - [[Instance Counting|Instance Counting]]https://ganelson.github.io/inform/runtime-module/2-ic.html - Though a feature, for convenience of implementation, this code is always active and provides for efficient loops through instances at runtime.
    - [[Kind Declarations|Kind Declarations]]https://ganelson.github.io/inform/runtime-module/2-kd.html - Each different kind used anywhere in the tree must be declared with an Inter kind declaration.
    - [[Showme Command|Showme Command]]https://ganelson.github.io/inform/runtime-module/2-sc.html - A feature to provide some support for the SHOWME testing command.
    - [[Here, Nowhere and Everywhere|Here, Nowhere and Everywhere]]https://ganelson.github.io/inform/runtime-module/2-hnae.html - Almost a Beatles song, but really a set of schemas for compiling the meaning of the unary predicates here, nowhere and everywhere.
    - [[Short Names|Short Names]]https://ganelson.github.io/inform/runtime-module/2-sn.html - To compile the "short name" and "capitalised short name" properties.
    - [[General Parsing Routines|General Parsing Routines]]https://ganelson.github.io/inform/runtime-module/2-gpr.html - To compile "general parsing routines", or GPRs, which are runtime functions used to match noun phrases in the command parser.
    - [[Index Extensions|Index Extensions]]https://ganelson.github.io/inform/runtime-module/2-ie.html - To keep details of the extensions currently loaded, their authors, titles, versions and rubrics, and to index and credit them suitably.
-   Chapter 3: Basics
    - [[Generic Module|Generic Module]]https://ganelson.github.io/inform/runtime-module/3-gm.html - A variety of Inter constants which do not depend on the content of the program.
    - [[Completion Module|Completion Module]]https://ganelson.github.io/inform/runtime-module/3-cm.html - The completion module contains material turning the collection of resources into a playable work.
    - [[Use Options (runtime)|Use Options (runtime)]]https://ganelson.github.io/inform/runtime-module/3-uo.html - To give use options a presence at run-time.
-   Chapter 4: Enclosed Resources
    - [[Enclosures|Enclosures]]https://ganelson.github.io/inform/runtime-module/4-enc.html - Packages which contain all the resources any of their subpackages will need are called "enclosures".
    - [[List Literals|List Literals]]https://ganelson.github.io/inform/runtime-module/4-ll.html - Each enclosure contains the literal lists needed by its functions.
    - [[Text Literals|Text Literals]]https://ganelson.github.io/inform/runtime-module/4-tl.html - In this section we compile text constants.
    - [[Text Substitutions|Text Substitutions]]https://ganelson.github.io/inform/runtime-module/4-ts.html - In this section we compile text with substitutions.
    - [[Responses|Responses]]https://ganelson.github.io/inform/runtime-module/4-rsp.html - In this section we keep track of response texts.
    - [[Box Quotations|Box Quotations]]https://ganelson.github.io/inform/runtime-module/4-bq.html - In this section we compile text constants.
    - [[Relation Literals|Relation Literals]]https://ganelson.github.io/inform/runtime-module/4-rl.html - In fact there is only one literal relation: the empty one, used as a default value.
    - [[Stored Action Literals|Stored Action Literals]]https://ganelson.github.io/inform/runtime-module/4-sal.html - Explicit actions stored in memory as literals.
    - [[Group Together|Group Together]]https://ganelson.github.io/inform/runtime-module/4-gt.html - The "group together" phrase in the Standard Rules needs support functions, which are compiled within the user's enclosure.
    - [[Looping Over Scope|Looping Over Scope]]https://ganelson.github.io/inform/runtime-module/4-los.html - To compile functions which implement conditions such as "in the presence of Mrs Dalloway".
-   Chapter 5: Provision Submodules
    - [[Activities (runtime)|Activities (runtime)]]https://ganelson.github.io/inform/runtime-module/5-act.html - To compile the activities submodule for a compilation unit, which contains _activity packages.
    - [[Adjectives|Adjectives]]https://ganelson.github.io/inform/runtime-module/5-adj.html - To compile the adjectives submodule for a compilation unit, which contains _adjective, _adjective_phrase and _measurement packages.
    - [[Chronology|Chronology]]https://ganelson.github.io/inform/runtime-module/5-chr.html - To compile the chronology submodule for a compilation unit, which contains _past_condition and _action_history_condition packages.
    - [[Conjugations|Conjugations]]https://ganelson.github.io/inform/runtime-module/5-cnj.html - To compile the conjugations submodule for a compilation unit, which contains _verb, _modal_verb and _verb_form packages.
    - [[Equations (runtime)|Equations (runtime)]]https://ganelson.github.io/inform/runtime-module/5-eqt.html - To compile the equations submodule for a compilation unit, which contains _equation packages.
    - [[Instances (runtime)|Instances (runtime)]]https://ganelson.github.io/inform/runtime-module/5-ins.html - To compile the instances submodule for a compilation unit, which contains _instance packages.
    - [[Backdrop Instances|Backdrop Instances]]https://ganelson.github.io/inform/runtime-module/5-bi.html - Some additions to an _instance package for instances of the kind "backdrop".
    - [[Door Instances|Door Instances]]https://ganelson.github.io/inform/runtime-module/5-di.html - Property values for two-sided doors to make them interconnect with the map at runtime.
    - [[Region Instances|Region Instances]]https://ganelson.github.io/inform/runtime-module/5-ri.html - Some additions to an _instance package for instances of the kind "region".
    - [[Scene Instances|Scene Instances]]https://ganelson.github.io/inform/runtime-module/5-si.html - Some additions to an _instance package for instances of the kind "backdrop".
    - [[inform/multimedia|Multimedia]]https://ganelson.github.io/inform/runtime-module/5-mlt.html - To compile the multimedia submodule for a compilation unit, which contains _external_file, _figure and _sound packages.
    - [[Tables (runtime)|Tables (runtime)]]https://ganelson.github.io/inform/runtime-module/5-tbl.html - To compile the tables submodule for a compilation unit, which contains _table packages containing _table_column_usage subpackages.
    - [[Table Columns (runtime)|Table Columns (runtime)]]https://ganelson.github.io/inform/runtime-module/5-tc.html - To compile the table_columns submodule for a compilation unit, which contains _table_column packages.
    - [[Dialogue Beat Instances|Dialogue Beat Instances]]https://ganelson.github.io/inform/runtime-module/5-dbi.html - To compile any dialogue details in the instances submodule.
    - [[Dialogue|Dialogue]]https://ganelson.github.io/inform/runtime-module/5-dli.html - To compile any dialogue details in the instances submodule.
    - [[Dialogue Choice Instances|Dialogue Choice Instances]]https://ganelson.github.io/inform/runtime-module/5-dci.html - To compile any dialogue details in the instances submodule.
    - [[Rules (runtime)|Rules (runtime)]]https://ganelson.github.io/inform/runtime-module/5-rls.html - To compile the rules submodule for a compilation unit, which contains _rule packages.
    - [[Rulebooks (runtime)|Rulebooks (runtime)]]https://ganelson.github.io/inform/runtime-module/5-rlb.html - To compile the rulebooks submodule for a compilation unit, which contains _rulebook and _outcome packages.
    - [[Variables|Variables]]https://ganelson.github.io/inform/runtime-module/5-vrb.html - To compile the variables submodule for a compilation unit, which contains _variable packages.
    - [[Properties (runtime)|Properties (runtime)]]https://ganelson.github.io/inform/runtime-module/5-prp.html - To compile the properties submodule for a compilation unit, which contains _property packages.
    - [[Relations (runtime)|Relations (runtime)]]https://ganelson.github.io/inform/runtime-module/5-rlt.html - To compile the relations submodule for a compilation unit, which contains _relation packages.
    - [[Literal Patterns (runtime)|Literal Patterns (runtime)]]https://ganelson.github.io/inform/runtime-module/5-lp.html - Compiled code to print and parse values expressed as literals.
    - [[Kind Constructors|Kind Constructors]]https://ganelson.github.io/inform/runtime-module/5-kc.html - Each kind constructor has an Inter package of resources.
    - [[Kind IDs|Kind IDs]]https://ganelson.github.io/inform/runtime-module/5-ki.html - To compile the equations submodule for a compilation unit, which contains _equation packages.
    - [[Actions (runtime)|Actions (runtime)]]https://ganelson.github.io/inform/runtime-module/5-act2.html - To compile the actions submodule for a compilation unit, which contains _action packages.
    - [[inform/Named Action Patterns|Named Action Patterns]]https://ganelson.github.io/inform/runtime-module/5-nap.html - To compile the named_action_patterns submodule for a compilation unit, which contains _named_action_pattern packages.
    - [[Test Scripts|Test Scripts]]https://ganelson.github.io/inform/runtime-module/5-ts.html - To compile the tests submodule for a compilation unit, which contains _test packages.
-   Chapter 6: Completion Resources
    - [[Bibliographic Data|Bibliographic Data]]https://ganelson.github.io/inform/runtime-module/6-bd.html - Recording bibliographic data, such as title and authorship, in Inter.
    - [[The Player|The Player]]https://ganelson.github.io/inform/runtime-module/6-tp.html - Providing for the player and her initial situation, that is, at the start of play.
    - [[The Map|The Map]]https://ganelson.github.io/inform/runtime-module/6-tm.html - The runtime representation of the spatial map for works of interactive fiction: that is, how the rooms and doors connect up.
    - [[Property Permissions (runtime)|Property Permissions (runtime)]]https://ganelson.github.io/inform/runtime-module/6-pp.html - Each property needs permission to be used, and here we emit the Inter statements necessary.
    - [[Property Values|Property Values]]https://ganelson.github.io/inform/runtime-module/6-pv.html - Compiling Inter property value instructions for the properties of instances and kinds.
    - [[Action Bitmap Property|Action Bitmap Property]]https://ganelson.github.io/inform/runtime-module/6-abp.html - To compile tiny arrays as values of the action_bitmap property.
    - [[Phrasebook Index|Phrasebook Index]]https://ganelson.github.io/inform/runtime-module/6-pi.html - Compiling what amounts to the Phrasebook index into the Inter hierarchy.
    - [[Mapping Hints|Mapping Hints]]https://ganelson.github.io/inform/runtime-module/6-mh.html - To transcribe mapping hints for the World Index into suitable packages.
    - [[Inferences (runtime)|Inferences (runtime)]]https://ganelson.github.io/inform/runtime-module/6-inf.html - To index inferences.
-   Chapter 7: Command Grammar
    - [[Command Grammars|Command Grammars]]https://ganelson.github.io/inform/runtime-module/7-cg.html - Runtime support for CGs.
    - [[Command Grammar Lines|Command Grammar Lines]]https://ganelson.github.io/inform/runtime-module/7-cgl.html - Compiling lines of command parser grammar.
    - [[Command Grammar Tokens|Command Grammar Tokens]]https://ganelson.github.io/inform/runtime-module/7-cgt.html - Compiling single command parser tokens.
    - [[Kind GPRs|Kind GPRs]]https://ganelson.github.io/inform/runtime-module/7-kg.html - General parsing routine (GPR) functions to match values of non-object kinds in the command parser.
    - [[Noun Filter Tokens|Noun Filter Tokens]]https://ganelson.github.io/inform/runtime-module/7-nft.html - General parsing routine (GPR) functions to match objects which fit some description, or have some scoping requirement.
    - [[Name Properties|Name Properties]]https://ganelson.github.io/inform/runtime-module/7-np.html - Small arrays of dictionary words which are values of the name property for objects.
    - [[Parse Name Properties|Parse Name Properties]]https://ganelson.github.io/inform/runtime-module/7-pnp.html - Functions which are values of the parse_name property for objects.
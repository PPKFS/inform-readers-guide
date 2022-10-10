---
{"dg-publish":true,"permalink":"/inform/runtime/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# runtime
```ad-info
Link: [ https://ganelson.github.io/inform/runtime-module/index.html]( https://ganelson.github.io/inform/runtime-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```



# Contents
- Chapter 1: Configuration and Control
    - [[inform/Runtime Module|Runtime Module]] - Setting up the use of this module.
-   Chapter 2: Emission
    - [[inform/Hierarchy|Hierarchy]] - To provide an enforced structure and set of naming conventions for packages and names in the Inter code we generate.
    - [[inform/Noun Identifiers|Noun Identifiers]] - Instances and kinds are both referred to by nouns, and here we create corresponding inames for use in compiled Inter code, and identifiers for use in the index.
    - [[inform/Compilation Units|Compilation Units]]  - The source text is divided into compilation units, and the material they lead to is similarly divided up.
    - [[inform/Emit|Emit]] - "Emitting" is the process of generating Inter bytecode, and this section provides a comprehensive API for the runtime and imperative modules to do that.
    - [[inform/Emit Code|Emit Code]] - Here is how bytecode for instructions inside functions is emitted.
    - [[inform/Emit Arrays|Emit Arrays]] - Here is how bytecode to create ready-initialised arrays of Inter data is emitted.
    - [[inform/Interventions|Interventions]] - Material written in low-level Inform 6 notation can be emitted for later linking, a distasteful process called "intervening".
    - [[inform/Shared Variables (runtime)|Shared Variables (runtime)]]  - Functions to create sets of shared variables.
    - [[inform/The Heap|The Heap]] - Texts, lists and other flexibly-sized structures make use of a pool of run-time storage called "the heap".
    - [[inform/Default Values|Default Values]] - An unusual feature of Inform is that every kind has a default value, so that it is impossible for any variable or property to be uninitialised.
    - [[inform/Equality Schemas|Equality Schemas]] - To define how to compile a comparison of two values.
    - [[inform/Instance Counting|Instance Counting]] - Though a feature, for convenience of implementation, this code is always active and provides for efficient loops through instances at runtime.
    - [[inform/Kind Declarations|Kind Declarations]] - Each different kind used anywhere in the tree must be declared with an Inter kind declaration.
    - [[inform/Showme Command|Showme Command]] - A feature to provide some support for the SHOWME testing command.
    - [[inform/Here, Nowhere and Everywhere|Here, Nowhere and Everywhere]] - Almost a Beatles song, but really a set of schemas for compiling the meaning of the unary predicates here, nowhere and everywhere.
    - [[inform/Short Names|Short Names]] - To compile the "short name" and "capitalised short name" properties.
    - [[inform/General Parsing Routines|General Parsing Routines]] - To compile "general parsing routines", or GPRs, which are runtime functions used to match noun phrases in the command parser.
    - [[inform/Index Extensions|Index Extensions]] - To keep details of the extensions currently loaded, their authors, titles, versions and rubrics, and to index and credit them suitably.
-   Chapter 3: Basics
    - [[inform/Generic Module|Generic Module]] - A variety of Inter constants which do not depend on the content of the program.
    - [[inform/Completion Module|Completion Module]] - The completion module contains material turning the collection of resources into a playable work.
    - [[inform/Use Options (runtime)|Use Options (runtime)]] - To give use options a presence at run-time.
-   Chapter 4: Enclosed Resources
    - [[inform/Enclosures|Enclosures]] - Packages which contain all the resources any of their subpackages will need are called "enclosures".
    - [[inform/List Literals|List Literals]] - Each enclosure contains the literal lists needed by its functions.
    - [[inform/Text Literals|Text Literals]] - In this section we compile text constants.
    - [[inform/Text Substitutions|Text Substitutions]] - In this section we compile text with substitutions.
    - [[inform/Responses|Responses]] - In this section we keep track of response texts.
    - [[inform/Box Quotations|Box Quotations]] - In this section we compile text constants.
    - [[inform/Relation Literals|Relation Literals]] - In fact there is only one literal relation: the empty one, used as a default value.
    - [[inform/Stored Action Literals|Stored Action Literals]] - Explicit actions stored in memory as literals.
    - [[inform/Group Together|Group Together]] - The "group together" phrase in the Standard Rules needs support functions, which are compiled within the user's enclosure.
    - [[inform/Looping Over Scope|Looping Over Scope]]- To compile functions which implement conditions such as "in the presence of Mrs Dalloway".
-   Chapter 5: Provision Submodules
    - [[inform/Activities (runtime)|Activities (runtime)]]  To compile the activities submodule for a compilation unit, which contains _activity packages.
    - [[inform/Adjectives (runtime)|Adjectives (runtime)]] - To compile the adjectives submodule for a compilation unit, which contains _adjective, _adjective_phrase and _measurement packages.
    - [[inform/Chronology|Chronology]] - To compile the chronology submodule for a compilation unit, which contains _past_condition and _action_history_condition packages.
    - [[inform/Conjugations|Conjugations]] - To compile the conjugations submodule for a compilation unit, which contains _verb, _modal_verb and _verb_form packages.
    - [[inform/Equations (runtime)|Equations (runtime)]] - To compile the equations submodule for a compilation unit, which contains _equation packages.
    - [[inform/Instances (runtime)|Instances (runtime)]] - To compile the instances submodule for a compilation unit, which contains _instance packages.
    - [[inform/Backdrop Instances|Backdrop Instances]] - Some additions to an _instance package for instances of the kind "backdrop".
    - [[inform/Door Instances|Door Instances]] - Property values for two-sided doors to make them interconnect with the map at runtime.
    - [[inform/Region Instances|Region Instances]] - Some additions to an _instance package for instances of the kind "region".
    - [[inform/Scene Instances|Scene Instances]] - Some additions to an _instance package for instances of the kind "backdrop".
    - [[inform/Multimedia (runtime)|Multimedia (runtime)]] - To compile the multimedia submodule for a compilation unit, which contains _external_file, _figure and _sound packages.
    - [[inform/Tables (runtime)|Tables (runtime)]] - To compile the tables submodule for a compilation unit, which contains _table packages containing _table_column_usage subpackages.
    - [[inform/Table Columns (runtime)|Table Columns (runtime)]] - To compile the table_columns submodule for a compilation unit, which contains _table_column packages.
    - [[inform/Dialogue Beat Instances|Dialogue Beat Instances]] - To compile any dialogue details in the instances submodule.
    - [[inform/Dialogue|Dialogue]] - To compile any dialogue details in the instances submodule.
    - [[inform/Dialogue Choice Instances|Dialogue Choice Instances]] - To compile any dialogue details in the instances submodule.
    - [[inform/Rules (runtime)|Rules (runtime)]] - To compile the rules submodule for a compilation unit, which contains _rule packages.
    - [[inform/Rulebooks (runtime)|Rulebooks (runtime)]] - To compile the rulebooks submodule for a compilation unit, which contains _rulebook and _outcome packages.
    - [[inform/Variables|Variables]] - To compile the variables submodule for a compilation unit, which contains _variable packages.
    - [[inform/Properties (runtime)|Properties (runtime)]] - To compile the properties submodule for a compilation unit, which contains _property packages.
    - [[inform/Relations (runtime)|Relations (runtime)]] - To compile the relations submodule for a compilation unit, which contains _relation packages.
    - [[inform/Literal Patterns (runtime)|Literal Patterns (runtime)]] - Compiled code to print and parse values expressed as literals.
    - [[inform/Kind Constructors|Kind Constructors]]  - Each kind constructor has an Inter package of resources.
    - [[inform/Kind IDs|Kind IDs]] - To compile the equations submodule for a compilation unit, which contains _equation packages.
    - [[inform/Actions (runtime)|Actions (runtime)]] - To compile the actions submodule for a compilation unit, which contains _action packages.
    - [[inform/Named Action Patterns (runtime)|Named Action Patterns (runtime)]] - To compile the named_action_patterns submodule for a compilation unit, which contains _named_action_pattern packages.
    - [[inform/Test Scripts (runtime)|Test Scripts (runtime)]] - To compile the tests submodule for a compilation unit, which contains _test packages.
-   Chapter 6: Completion Resources
    - [[inform/Bibliographic Data (runtime)|Bibliographic Data (runtime)]] - Recording bibliographic data, such as title and authorship, in Inter.
    - [[inform/The Player (runtime)|The Player (runtime)]] - Providing for the player and her initial situation, that is, at the start of play.
    - [[inform/The Map (runtime)|The Map (runtime)]] - The runtime representation of the spatial map for works of interactive fiction: that is, how the rooms and doors connect up.
    - [[inform/Property Permissions (runtime)|Property Permissions (runtime)]] - Each property needs permission to be used, and here we emit the Inter statements necessary.
    - [[inform/Property Values|Property Values]] - Compiling Inter property value instructions for the properties of instances and kinds.
    - [[inform/Action Bitmap Property|Action Bitmap Property]] - To compile tiny arrays as values of the action_bitmap property.
    - [[inform/Phrasebook Index|Phrasebook Index]] - Compiling what amounts to the Phrasebook index into the Inter hierarchy.
    - [[inform/Mapping Hints|Mapping Hints]] - To transcribe mapping hints for the World Index into suitable packages.
    - [[inform/Inferences (runtime)|Inferences (runtime)]] - To index inferences.
-   Chapter 7: Command Grammar
    - [[inform/Command Grammars (runtime)|Command Grammars (runtime)]] - Runtime support for CGs.
    - [[inform/Command Grammar Lines (runtime)|Command Grammar Lines (runtime)]] - Compiling lines of command parser grammar.
    - [[inform/Command Grammar Tokens (runtime)|Command Grammar Tokens (runtime)]] - Compiling single command parser tokens.
    - [[inform/Kind GPRs|Kind GPRs]] - General parsing routine (GPR) functions to match values of non-object kinds in the command parser.
    - [[inform/Noun Filter Tokens|Noun Filter Tokens]] - General parsing routine (GPR) functions to match objects which fit some description, or have some scoping requirement.
    - [[inform/Name Properties|Name Properties]] - Small arrays of dictionary words which are values of the name property for objects.
    - [[inform/Parse Name Properties|Parse Name Properties]] - Functions which are values of the parse_name property for objects.
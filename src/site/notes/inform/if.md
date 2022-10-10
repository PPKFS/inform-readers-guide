---
{"dg-publish":true,"permalink":"/inform/if/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# if
```ad-info
Link: [  https://ganelson.github.io/inform/if-module/index.html]]  https://ganelson.github.io/inform/if-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```

# Contents
- -   Chapter 1: Starting Up
    - [[inform/IF Module|IF Module]] - Setting up the use of this module.
-   Chapter 2: Bibliographic Data
    - [[inform/Bibliographic Data (if)|Bibliographic Data (if)]] - To manage the special variables providing bibliographic data on the work of IF being generated (title, author's name and so forth), and to write the Library Card in the index.
    - [[inform/Release Instructions|Release Instructions]] To write the iFiction record for the work of IF compiled, its release instructions and its picture manifest, if any.
    - [[inform/The iFiction Record|The iFiction Record]] - To write the iFiction record for the work of IF compiled.
    - [[inform/The Blurb File|The Blurb File]]  - To write the blurb file of instructions for inblorb to release the project.
-   Chapter 3: Space and Time
    - [[inform/Spatial Model|Spatial Model]] - A feature which constructs the fundamental spatial model used by IF, to represent containment, support, carrying, wearing, and incorporation.
    - [[inform/Everywhere, Nowhere and Here|Everywhere, Nowhere and Here]] - To define the unary predicates for some anaphoric location adjectives.
    - [[inform/Spatial Relations|Spatial Relations]] - Binary predicates for spatial relationships.
    - [[inform/Spatial Inferences|Spatial Inferences]] - Six families of inference used by the spatial feature.
    - [[inform/Persons|Persons]] - A feature giving minimal support for switchable devices.
    - [[inform/The Player (if)|The Player (if)]] - A feature to give a special role to a person who is the protagonist.
    - [[inform/Devices|Devices]] - A feature giving minimal support for switchable devices.
    - [[inform/Backdrops|Backdrops]] - A feature to provide support for backdrop objects, which are present as scenery in multiple rooms at once.
    - [[inform/Regions|Regions]] - A feature providing support for grouping rooms together into named and nestable regions.
    - [[inform/The Map (if)|The Map (if)]] - A feature to provide a geographical model, linking rooms and doors together in oppositely-paired directions.
    - [[inform/Map Connection Relations|Map Connection Relations]] - To define one binary predicate for each map direction, such as "mapped north of".
    - [[inform/Timed Rules|Timed Rules]]- A feature to support rules like "At 12:03AM: ...".
    - [[inform/Scenes|Scenes]] - A feature to support named periods of time during an interactive story.
    - [[inform/The Score|The Score]] - A feature to support the score variables.
    - [[inform/Mapping Hint Requests|Mapping Hint Requests]] - Special sentences giving layout or design hints on how to produce the World map in the index and an EPS map.
-   Chapter 4: Actions
    - [[inform/Actions Plugin|Actions Plugin]] - A feature for actions, by which animate characters change the world model.
    - [[inform/Actions-Only Nodes and Annotations|Actions-Only Nodes and Annotations]] - Additional syntax tree node and annotation types used by the actions feature.
    - [[inform/Action Kinds|Action Kinds]] - Three action-related kinds of value.
    - [[inform/Action Conditions|Action Conditions]] - A special condition for testing against action patterns.
    - [[inform/Actions (if)|Actions (if)]] - Each different sort of impulse to do something is an "action name".
    - [[inform/Action Semantics|Action Semantics]] - Constraints on how actions may be used in the model world.
    - [[inform/Action Variables|Action Variables]] - Variables shared by the rules of the rulebooks processing an action.
    - [[inform/Action Name Names|Action Name Names]] - There is an annoying profusion of ways an action can have a name.
    - [[inform/Action Patterns|Action Patterns]] - An action pattern is a description which may match many actions or none. The text "doing something" matches every action, while "throwing something at a door in a dark room" is seldom matched.
    - [[inform/Action Name Lists|Action Name Lists]] - Action name lists are used in parsing action patterns, and identify which action names seem to be possible within them.
    - [[inform/Action Pattern Clauses|Action Pattern Clauses]] - Pattern-matches on individual nouns in an action are called clauses.
    - [[inform/Parse Action Patterns|Parse Action Patterns]]  - Turning text into APs.
    - [[inform/Parse Clauses|Parse Clauses]] - Parsing the clauses part of an AP from source text.
    - [[inform/Explicit Actions|Explicit Actions]] - An exactly specified action is called "explicit".
    - [[inform/Named Action Patterns (if)|Named Action Patterns (if)]] - A named action pattern is a categorisation of behaviour.
    - [[inform/Going|Going]]  - A feature to provide a little extra support for the "going" action.
    - [[inform/Rules Predicated on Actions|Rules Predicated on Actions]] - Rules can be set to run only if the action matches a given pattern.
- Chapter 5: Command Parser
    - [[inform/Parsing Plugin|Parsing Plugin]] - A feature for command-parser support.
    - [[inform/Understand Sentences|Understand Sentences]] - Command parser grammar is laid out in special Understand... sentences.
    - [[inform/Command Grammars (if)|Command Grammars (if)]] - The possible command text following a command verb, or referring to a single concept or object, is gathered into a "command grammar".
    - [[inform/Command Grammar Lines (if)|Command Grammar Lines (if)]]  - A CG line is a list of CG tokens to specify a textual pattern. For example, "take [something] out" is a CG line of three tokens.
    - [[inform/Command Grammar Tokens (if)|Command Grammar Tokens (if)]] - CGs are list of CG lines, which are lists of CG tokens.
    - [[inform/Determination Types|Determination Types]] - Command grammars, their lines and their tokens may each "determine" up to two values, and here we provide a way to describe the range of those.
    - [[inform/Property Visibility|Property Visibility]]  - Some properties can be referred to in the player's commands.
    - [[inform/Test Scripts (if)|Test Scripts (if)]] - A rudimentary but useful testing system for runnign short sequences of commands through the command parser at runtime.
-   Chapter 6: Dialogue
    - [[inform/Dialogue (if)|Dialogue (if)]] - A nascent system for managing conversation.
    - [[inform/Dialogue Beats|Dialogue Beats]] - To manage dialogue beats and to parse their cue paragraphs.
    - [[inform/Dialogue Lines|Dialogue Lines]]  - To manage dialogue lines.
    - [[inform/Dialogue Choices|Dialogue Choices]] - To manage dialogue choices.
    - [[inform/Dialogue Nodes|Dialogue Nodes]] - The structure of a dialogue beat as a tree of nodes, each of which can be either a line or a choice.
    - [[inform/Dialogue Relations|Dialogue Relations]] - Binary predicates for spatial relationships.
    - [[inform/Performance Styles|Performance Styles]] - Manners of speaking, used in dialogue.
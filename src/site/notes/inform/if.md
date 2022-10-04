---
{"dg-publish":true,"permalink":"/inform/if/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# if
```ad-info
Link: [https://ganelson.github.io/inform/if-module/index.html]]https://ganelson.github.io/inform/if-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```



# Contents
- -   Chapter 1: Starting Up
    - [[IF Module|IF Module]]https://ganelson.github.io/inform/if-module/1-im.html - Setting up the use of this module.
-   Chapter 2: Bibliographic Data
    - [[Bibliographic Data|Bibliographic Data]]https://ganelson.github.io/inform/if-module/2-bd.html - To manage the special variables providing bibliographic data on the work of IF being generated (title, author's name and so forth), and to write the Library Card in the index.
    - [[Release Instructions|Release Instructions]]https://ganelson.github.io/inform/if-module/2-ri.html - To write the iFiction record for the work of IF compiled, its release instructions and its picture manifest, if any.
    - [[The iFiction Record|The iFiction Record]]https://ganelson.github.io/inform/if-module/2-tir.html - To write the iFiction record for the work of IF compiled.
    - [[The Blurb File|The Blurb File]]https://ganelson.github.io/inform/if-module/2-tbf.html - To write the blurb file of instructions for inblorb to release the project.
-   Chapter 3: Space and Time
    - [[Spatial Model|Spatial Model]]https://ganelson.github.io/inform/if-module/3-sm.html - A feature which constructs the fundamental spatial model used by IF, to represent containment, support, carrying, wearing, and incorporation.
    - [[Everywhere, Nowhere and Here|Everywhere, Nowhere and Here]]https://ganelson.github.io/inform/if-module/3-enah.html - To define the unary predicates for some anaphoric location adjectives.
    - [[Spatial Relations|Spatial Relations]]https://ganelson.github.io/inform/if-module/3-sr.html - Binary predicates for spatial relationships.
    - [[Spatial Inferences|Spatial Inferences]]https://ganelson.github.io/inform/if-module/3-si.html - Six families of inference used by the spatial feature.
    - [[Persons|Persons]]https://ganelson.github.io/inform/if-module/3-prs.html - A feature giving minimal support for switchable devices.
    - [[The Player|The Player]]https://ganelson.github.io/inform/if-module/3-tp.html - A feature to give a special role to a person who is the protagonist.
    - [[Devices|Devices]]https://ganelson.github.io/inform/if-module/3-dvc.html - A feature giving minimal support for switchable devices.
    - [[Backdrops|Backdrops]]https://ganelson.github.io/inform/if-module/3-bck.html - A feature to provide support for backdrop objects, which are present as scenery in multiple rooms at once.
    - [[Regions|Regions]]https://ganelson.github.io/inform/if-module/3-rgn.html - A feature providing support for grouping rooms together into named and nestable regions.
    - [[The Map|The Map]]https://ganelson.github.io/inform/if-module/3-tm.html - A feature to provide a geographical model, linking rooms and doors together in oppositely-paired directions.
    - [[Map Connection Relations|Map Connection Relations]]https://ganelson.github.io/inform/if-module/3-mcr.html - To define one binary predicate for each map direction, such as "mapped north of".
    - [[Timed Rules|Timed Rules]]https://ganelson.github.io/inform/if-module/3-tr.html - A feature to support rules like "At 12:03AM: ...".
    - [[Scenes|Scenes]]https://ganelson.github.io/inform/if-module/3-scn.html - A feature to support named periods of time during an interactive story.
    - [[The Score|The Score]]https://ganelson.github.io/inform/if-module/3-ts.html - A feature to support the score variables.
    - [[Mapping Hint Requests|Mapping Hint Requests]]https://ganelson.github.io/inform/if-module/3-mhr.html - Special sentences giving layout or design hints on how to produce the World map in the index and an EPS map.
-   Chapter 4: Actions
    - [[Actions Plugin|Actions Plugin]]https://ganelson.github.io/inform/if-module/4-ap.html - A feature for actions, by which animate characters change the world model.
    - [[Actions-Only Nodes and Annotations|Actions-Only Nodes and Annotations]]https://ganelson.github.io/inform/if-module/4-anaa.html - Additional syntax tree node and annotation types used by the actions feature.
    - [[Action Kinds|Action Kinds]]https://ganelson.github.io/inform/if-module/4-ak.html - Three action-related kinds of value.
    - [[Action Conditions|Action Conditions]]https://ganelson.github.io/inform/if-module/4-ac.html - A special condition for testing against action patterns.
    - [[Actions (if)|Actions (if)]]https://ganelson.github.io/inform/if-module/4-act.html - Each different sort of impulse to do something is an "action name".
    - [[Action Semantics|Action Semantics]]https://ganelson.github.io/inform/if-module/4-as.html - Constraints on how actions may be used in the model world.
    - [[Action Variables|Action Variables]]https://ganelson.github.io/inform/if-module/4-av.html - Variables shared by the rules of the rulebooks processing an action.
    - [[Action Name Names|Action Name Names]]https://ganelson.github.io/inform/if-module/4-ann.html - There is an annoying profusion of ways an action can have a name.
    - [[Action Patterns|Action Patterns]]https://ganelson.github.io/inform/if-module/4-ap2.html - An action pattern is a description which may match many actions or none. The text "doing something" matches every action, while "throwing something at a door in a dark room" is seldom matched.
    - [[Action Name Lists|Action Name Lists]]https://ganelson.github.io/inform/if-module/4-anl.html - Action name lists are used in parsing action patterns, and identify which action names seem to be possible within them.
    - [[Action Pattern Clauses|Action Pattern Clauses]]https://ganelson.github.io/inform/if-module/4-apc.html - Pattern-matches on individual nouns in an action are called clauses.
    - [[Parse Action Patterns|Parse Action Patterns]]https://ganelson.github.io/inform/if-module/4-pap.html - Turning text into APs.
    - [[Parse Clauses|Parse Clauses]]https://ganelson.github.io/inform/if-module/4-pc.html - Parsing the clauses part of an AP from source text.
    - [[Explicit Actions|Explicit Actions]]https://ganelson.github.io/inform/if-module/4-ea.html - An exactly specified action is called "explicit".
    - [[inform/Named Action Patterns|Named Action Patterns]]https://ganelson.github.io/inform/if-module/4-nap.html - A named action pattern is a categorisation of behaviour.
    - [[Going|Going]]https://ganelson.github.io/inform/if-module/4-gng.html - A feature to provide a little extra support for the "going" action.
    - [[Rules Predicated on Actions|Rules Predicated on Actions]]https://ganelson.github.io/inform/if-module/4-rpoa.html - Rules can be set to run only if the action matches a given pattern.
-   Chapter 5: Command Parser
    - [[Parsing Plugin|Parsing Plugin]]https://ganelson.github.io/inform/if-module/5-pp.html - A feature for command-parser support.
    - [[Understand Sentences|Understand Sentences]]https://ganelson.github.io/inform/if-module/5-us.html - Command parser grammar is laid out in special Understand... sentences.
    - [[Command Grammars|Command Grammars]]https://ganelson.github.io/inform/if-module/5-cg.html - The possible command text following a command verb, or referring to a single concept or object, is gathered into a "command grammar".
    - [[Command Grammar Lines|Command Grammar Lines]]https://ganelson.github.io/inform/if-module/5-cgl.html - A CG line is a list of CG tokens to specify a textual pattern. For example, "take [something] out" is a CG line of three tokens.
    - [[Command Grammar Tokens|Command Grammar Tokens]]https://ganelson.github.io/inform/if-module/5-cgt.html - CGs are list of CG lines, which are lists of CG tokens.
    - [[Determination Types|Determination Types]]https://ganelson.github.io/inform/if-module/5-dt.html - Command grammars, their lines and their tokens may each "determine" up to two values, and here we provide a way to describe the range of those.
    - [[Property Visibility|Property Visibility]]https://ganelson.github.io/inform/if-module/5-pv.html - Some properties can be referred to in the player's commands.
    - [[Test Scripts|Test Scripts]]https://ganelson.github.io/inform/if-module/5-ts.html - A rudimentary but useful testing system for runnign short sequences of commands through the command parser at runtime.
-   Chapter 6: Dialogue
    - [[Dialogue|Dialogue]]https://ganelson.github.io/inform/if-module/6-dlg.html - A nascent system for managing conversation.
    - [[Dialogue Beats|Dialogue Beats]]https://ganelson.github.io/inform/if-module/6-db.html - To manage dialogue beats and to parse their cue paragraphs.
    - [[Dialogue Lines|Dialogue Lines]]https://ganelson.github.io/inform/if-module/6-dl.html - To manage dialogue lines.
    - [[Dialogue Choices|Dialogue Choices]]https://ganelson.github.io/inform/if-module/6-dc.html - To manage dialogue choices.
    - [[Dialogue Nodes|Dialogue Nodes]]https://ganelson.github.io/inform/if-module/6-dn.html - The structure of a dialogue beat as a tree of nodes, each of which can be either a line or a choice.
    - [[Dialogue Relations|Dialogue Relations]]https://ganelson.github.io/inform/if-module/6-dr.html - Binary predicates for spatial relationships.
    - [[Performance Styles|Performance Styles]]https://ganelson.github.io/inform/if-module/6-ps.html - Manners of speaking, used in dialogue.
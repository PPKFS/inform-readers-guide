---
{"dg-publish":true,"permalink":"/inform/assertions/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# assertions
```ad-info
Link: [https://ganelson.github.io/inform/assertions-module/index.html](https://ganelson.github.io/inform/assertions-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```

# Contents
- Chapter 1: Configuration and Control
	- [[inform/Assertions Module|Assertions Module]] - Setting up the use of this module.
- Chapter 2: Declarations
	- [[inform/Booting Verbs|Booting Verbs]] - In Inform even verbs are created with natural language sentences, but this process has to start somewhere.
	- [[inform/Passes through Major Nodes|Passes through Major Nodes]] - To manage the overall process of traversing the parse tree for top-level declarations and assertion sentences.
	- [[inform/Anaphoric References|Anaphoric References]] - To keep track of the current object and subject of discussion.
	- [[inform/Classifying Sentences|Classifying Sentences]] - To work out the verbs used and to diagram sentences in the source.
	- [[inform/Property Sentences|Property Sentences]] - To examine assertion sentences for property creation.
	- [[inform/Imperative Subtrees|Imperative Subtrees]] - To tidy up blocks of rule and phrase definition in the syntax tree.
- Chapter 3: Requests
	- [[inform/Debugging Log Requests|Debugging Log Requests]] - Special sentences for changing what goes into the debugging log.
	- [[inform/Pluralisation Requests|Pluralisation Requests]] - Special sentences for setting exotic plural forms of nouns.
	- [[inform/Translation Requests|Translation Requests]] - Three unrelated senses of "X translates into Y as Z" sentences.
	- [[inform/New Use Option Requests|New Use Option Requests]] - Special sentences for creating new use options.
	- [[inform/Use Options (assertions)|Use Options (assertions)]] - Special sentences for setting compilation options.
	- [[inform/Test Requests|Test Requests]] - Special sentences for requesting unit tests or providing test scripts.
	- [[inform/Define by Table Requests|Define by Table Requests]] - Special sentences declaring that tables amount to massed groups of assertions.
	- [[inform/Rule Placement Requests|Rule Placement Requests]] - Special sentences for listing named rules in particular rulebooks.
	- [[inform/New Activity Requests|New Activity Requests]] - Special sentences creating new activities.
	- [[inform/New Literal Pattern Requests|New Literal Pattern Requests]] - Special sentences creating new notations for literal values.
	- [[inform/New Relation Requests|New Relation Requests]] - Special sentences for creating new relations.
	- [[inform/New Property Requests|New Property Requests]] - Special sentences creating new either/or properties.
	- [[inform/New Verb Requests|New Verb Requests]] - Special sentences for creating new verbs.
	- [[inform/New Adjective Requests|New Adjective Requests]] - Special sentences for creating new adjectives.
	- [[inform/Intervention Requests|Intervention Requests]] - Special sentences for inserting low-level material written in Inform 6 notation.
- Chapter 4: Assertions
    - [[inform/Name Resolution|Name Resolution]] - To resolve abbreviated or ambiguous nouns in context of their headings.
    - [[inform/Refine Parse Tree|Refine Parse Tree]] - To determine which subjects are referred to by noun phrases such as "the table" or "a paper cup" found in assertion sentences.
    - [[inform/The Creator|The Creator]] - This is where all objects, kinds of object, named values, kinds of value and global variables are made.
    - [[inform/Assertions (assertions)|Assertions (assertions)]] - To infer facts about the model world, or take other action, based on sentences asserted as being true in the source text.
    - [[inform/New Property Assertions|New Property Assertions]] - When regular assertion sentences create properties.
    - [[inform/Property Knowledge|Property Knowledge]] - This section draws inferences from assertions which seem to be about the properties of things, independent of their location.
    - [[inform/Relation Knowledge|Relation Knowledge]] - This section draws inferences about the relationships between objects or values.
    - [[inform/Assemblies|Assemblies]] - To build the complex multi-object assemblies which result from allowing the source text to say things like "in every room is a vehicle".
    - [[inform/Implications|Implications]] - To keep track of a dangerous form of super-assertion called an implication, which is allowed to generalise about properties.
-   Chapter 5: Imperative Code
    - [[inform/Imperative Definitions|Imperative Definitions]] - Each IMPERATIVE node in the syntax tree makes a definition using imperative code.
    - [[inform/Imperative Definition Families|Imperative Definition Families]]- Different categories of imperative definition.
    - [[inform/Adjectival Definition Family|Adjectival Definition Family]] - Imperative definitions of "Definition: X is Y: ..." adjectives.
    - [[inform/To Phrase Family|To Phrase Family]]- Imperative definitions of "To..." phrases.
    - [[inform/Phrase Type Data|Phrase Type Data]] - To create, manage, compare the logical specificity of, and assist excerpt parsing concerning, the type of a To phrase.
    - [[inform/Parsing Type Data|Parsing Type Data]]- To parse the prototype text of a To... phrase into its type data.
    - [[inform/Phrase Options|Phrase Options]] - To create and subsequently parse against the list of phrase options with which the user can choose to invoke a To phrase.
    - [[inform/Rule Family|Rule Family]] - Imperative definitions of rules.
    - [[inform/Runtime Context Data|Runtime Context Data]] - To store the circumstances in which a rule phrase should fire.
-   Chapter 6: Rules, Rulebooks and Activities
    - [[inform/Rules (assertions)|Rules (assertions)]]- Rules contain imperative code which is executed when certain actions, activities or other processes are being followed.
    - [[inform/Rule Bookings|Rule Bookings]]- Bookings are assignments of rules to rulebooks.
    - [[inform/Booking Lists|Booking Lists]]- Booking lists are linked lists of rule bookings. The content of a rulebook is a booking list.
    - [[inform/Rulebooks (assertions)|Rulebooks (assertions)]] - Rulebooks collate rules and provide an organised way for them to collaborate on a larger task.
    - [[inform/Focus and Outcome|Focus and Outcome]]- What a rulebook works on, and what it produces.
    - [[inform/Activities (assertions)|Activities (assertions)]] - To create and manage activities, which are bundles of rules for carrying out tasks.
    - [[inform/Shared Variables|Shared Variables]]- Shared variables are held in common by all rules working in some goal.
-   Chapter 7: Other Gadgets
    - [[inform/Table Columns (assertions)|Table Columns (assertions)]] - To manage the named columns which appear in tables.
    - [[inform/Tables (assertions)|Tables (assertions)]]- To manage and compile tables, which are two-dimensional arrays with associative look-up facilities provided at run-time.
    - [[inform/Equations (assertions)|Equations (assertions)]]- To manage and compile equations, which relate numerical quantities.
-   Chapter 8: Predicates
    - [[inform/Kind Predicates Revisited|Kind Predicates Revisited]] - To define how the kind predicates behave in the Inform language.
    - [[inform/The Adjectival Predicates|The Adjectival Predicates]]- To define the predicates connected to linguistic adjectives.
    - [[inform/The Creation Predicates|The Creation Predicates]] - To define the predicates causing instances to be created.
    - [[inform/The Equality Relation Revisited|The Equality Relation Revisited]]- To define how equality behaves in the Inform language.
    - [[inform/Quasinumeric Relations|Quasinumeric Relations]] - To define the binary predicates corresponding to numerical comparisons.
    - [[inform/The Universal Relation|The Universal Relation]] - To define the universal relation, which can apply and therefore subsumes all other relations.
    - [[inform/Explicit Relations|Explicit Relations]]- To draw inferences from the relations created explicitly by the source text.
    - [[inform/Listed-In Relations|Listed-In Relations]] - To define the binary predicates corresponding to table columns, and which determine whether a given value is listed in that column.
    - [[inform/Adjective Ambiguity|Adjective Ambiguity]] - Managing the multiple contextual meanings which a single adjective can have.
    - [[inform/Adjective Meanings|Adjective Meanings]] - One individual meaning which an adjective can have.
    - [[inform/Adjective Meaning Domains|Adjective Meaning Domains]] - What a single sense of an adjective can apply to: perhaps a kind or an instance.
    - [[inform/Adjectives by Phrase|Adjectives by Phrase]]- Adjectives defined by an I7 phrase written out longhand.
    - [[inform/Adjectives by Condition|Adjectives by Condition]] - Adjectives defined by a one-line I7 condition.
    - [[inform/Adjectives by Inter Function|Adjectives by Inter Function]] - Defining an adjective with an Inter function to test or make it true.
    - [[inform/Adjectives by Inter Condition|Adjectives by Inter Condition]] - Defining an adjective with an Inter condition.
    - [[inform/Calculus Utilities|Calculus Utilities]] - Utility functions for creating basic propositions using these predicates.
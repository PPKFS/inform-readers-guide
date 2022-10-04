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
	- [[Assertions Module|Assertions Module]] - Setting up the use of this module.
- Chapter 2: Declarations
	- [[Booting Verbs|Booting Verbs]] - In Inform even verbs are created with natural language sentences, but this process has to start somewhere.
	- [[Passes through Major Nodes|Passes through Major Nodes]] - To manage the overall process of traversing the parse tree for top-level declarations and assertion sentences.
	- [[Anaphoric References|Anaphoric References]] - To keep track of the current object and subject of discussion.
	- [[Classifying Sentences|Classifying Sentences]] - To work out the verbs used and to diagram sentences in the source.
	- [[Property Sentences|Property Sentences]] - To examine assertion sentences for property creation.
	- [[Imperative Subtrees|Imperative Subtrees]] - To tidy up blocks of rule and phrase definition in the syntax tree.
- Chapter 3: Requests
	- [[Debugging Log Requests|Debugging Log Requests]] - Special sentences for changing what goes into the debugging log.
	- [[Pluralisation Requests|Pluralisation Requests]] - Special sentences for setting exotic plural forms of nouns.
	- [[Translation Requests|Translation Requests]] - Three unrelated senses of "X translates into Y as Z" sentences.
	- [[New Use Option Requests|New Use Option Requests]] - Special sentences for creating new use options.
	- [[Use Options (assertions)|Use Options (assertions)]] - Special sentences for setting compilation options.
	- [[Test Requests|Test Requests]] - Special sentences for requesting unit tests or providing test scripts.
	- [[Define by Table Requests|Define by Table Requests]] - Special sentences declaring that tables amount to massed groups of assertions.
	- [[Rule Placement Requests|Rule Placement Requests]] - Special sentences for listing named rules in particular rulebooks.
	- [[New Activity Requests|New Activity Requests]] - Special sentences creating new activities.
	- [[New Literal Pattern Requests|New Literal Pattern Requests]] - Special sentences creating new notations for literal values.
	- [[New Relation Requests|New Relation Requests]] - Special sentences for creating new relations.
	- [[New Property Requests|New Property Requests]] - Special sentences creating new either/or properties.
	- [[New Verb Requests|New Verb Requests]] - Special sentences for creating new verbs.
	- [[New Adjective Requests|New Adjective Requests]] - Special sentences for creating new adjectives.
	- [[Intervention Requests|Intervention Requests]] - Special sentences for inserting low-level material written in Inform 6 notation.
- Chapter 4: Assertions
    - [[Name Resolution|Name Resolution]]https://ganelson.github.io/inform/assertions-module/4-nr.html - To resolve abbreviated or ambiguous nouns in context of their headings.
    - [[Refine Parse Tree|Refine Parse Tree]]https://ganelson.github.io/inform/assertions-module/4-rpt.html - To determine which subjects are referred to by noun phrases such as "the table" or "a paper cup" found in assertion sentences.
    - [[The Creator|The Creator]]https://ganelson.github.io/inform/assertions-module/4-tc.html - This is where all objects, kinds of object, named values, kinds of value and global variables are made.
    - [[inform/assertions|Assertions]]https://ganelson.github.io/inform/assertions-module/4-ass.html - To infer facts about the model world, or take other action, based on sentences asserted as being true in the source text.
    - [[New Property Assertions|New Property Assertions]]https://ganelson.github.io/inform/assertions-module/4-npa.html - When regular assertion sentences create properties.
    - [[Property Knowledge|Property Knowledge]]https://ganelson.github.io/inform/assertions-module/4-pk.html - This section draws inferences from assertions which seem to be about the properties of things, independent of their location.
    - [[Relation Knowledge|Relation Knowledge]]https://ganelson.github.io/inform/assertions-module/4-rk.html - This section draws inferences about the relationships between objects or values.
    - [[Assemblies|Assemblies]]https://ganelson.github.io/inform/assertions-module/4-ass2.html - To build the complex multi-object assemblies which result from allowing the source text to say things like "in every room is a vehicle".
    - [[Implications|Implications]]https://ganelson.github.io/inform/assertions-module/4-imp.html - To keep track of a dangerous form of super-assertion called an implication, which is allowed to generalise about properties.
-   Chapter 5: Imperative Code
    - [[Imperative Definitions|Imperative Definitions]]https://ganelson.github.io/inform/assertions-module/5-id.html - Each IMPERATIVE node in the syntax tree makes a definition using imperative code.
    - [[Imperative Definition Families|Imperative Definition Families]]https://ganelson.github.io/inform/assertions-module/5-idf.html - Different categories of imperative definition.
    - [[Adjectival Definition Family|Adjectival Definition Family]]https://ganelson.github.io/inform/assertions-module/5-adf.html - Imperative definitions of "Definition: X is Y: ..." adjectives.
    - [[To Phrase Family|To Phrase Family]]https://ganelson.github.io/inform/assertions-module/5-tpf.html - Imperative definitions of "To..." phrases.
    - [[Phrase Type Data|Phrase Type Data]]https://ganelson.github.io/inform/assertions-module/5-ptd.html - To create, manage, compare the logical specificity of, and assist excerpt parsing concerning, the type of a To phrase.
    - [[Parsing Type Data|Parsing Type Data]]https://ganelson.github.io/inform/assertions-module/5-ptd2.html - To parse the prototype text of a To... phrase into its type data.
    - [[Phrase Options|Phrase Options]]https://ganelson.github.io/inform/assertions-module/5-po.html - To create and subsequently parse against the list of phrase options with which the user can choose to invoke a To phrase.
    - [[Rule Family|Rule Family]]https://ganelson.github.io/inform/assertions-module/5-rf.html - Imperative definitions of rules.
    - [[Runtime Context Data|Runtime Context Data]]https://ganelson.github.io/inform/assertions-module/5-rcd.html - To store the circumstances in which a rule phrase should fire.
-   Chapter 6: Rules, Rulebooks and Activities
    - [[Rules (assertions)|Rules (assertions)]]https://ganelson.github.io/inform/assertions-module/6-rls.html - Rules contain imperative code which is executed when certain actions, activities or other processes are being followed.
    - [[Rule Bookings|Rule Bookings]]https://ganelson.github.io/inform/assertions-module/6-rb.html - Bookings are assignments of rules to rulebooks.
    - [[Booking Lists|Booking Lists]]https://ganelson.github.io/inform/assertions-module/6-bl.html - Booking lists are linked lists of rule bookings. The content of a rulebook is a booking list.
    - [[Rulebooks (assertions)|Rulebooks (assertions)]]https://ganelson.github.io/inform/assertions-module/6-rlb.html - Rulebooks collate rules and provide an organised way for them to collaborate on a larger task.
    - [[Focus and Outcome|Focus and Outcome]]https://ganelson.github.io/inform/assertions-module/6-fao.html - What a rulebook works on, and what it produces.
    - [[Activities (assertions)|Activities (assertions)]]https://ganelson.github.io/inform/assertions-module/6-act.html - To create and manage activities, which are bundles of rules for carrying out tasks.
    - [[Shared Variables|Shared Variables]]https://ganelson.github.io/inform/assertions-module/6-sv.html - Shared variables are held in common by all rules working in some goal.
-   Chapter 7: Other Gadgets
    - [[Table Columns (assertions)|Table Columns (assertions)]]https://ganelson.github.io/inform/assertions-module/7-tc.html - To manage the named columns which appear in tables.
    - [[Tables (assertions)|Tables (assertions)]]https://ganelson.github.io/inform/assertions-module/7-tbl.html - To manage and compile tables, which are two-dimensional arrays with associative look-up facilities provided at run-time.
    - [[Equations (assertions)|Equations (assertions)]]https://ganelson.github.io/inform/assertions-module/7-eqt.html - To manage and compile equations, which relate numerical quantities.
-   Chapter 8: Predicates
    - [[Kind Predicates Revisited|Kind Predicates Revisited]]https://ganelson.github.io/inform/assertions-module/8-kpr.html - To define how the kind predicates behave in the Inform language.
    - [[The Adjectival Predicates|The Adjectival Predicates]]https://ganelson.github.io/inform/assertions-module/8-tap.html - To define the predicates connected to linguistic adjectives.
    - [[The Creation Predicates|The Creation Predicates]]https://ganelson.github.io/inform/assertions-module/8-tcp.html - To define the predicates causing instances to be created.
    - [[The Equality Relation Revisited|The Equality Relation Revisited]]https://ganelson.github.io/inform/assertions-module/8-terr.html - To define how equality behaves in the Inform language.
    - [[Quasinumeric Relations|Quasinumeric Relations]]https://ganelson.github.io/inform/assertions-module/8-qr.html - To define the binary predicates corresponding to numerical comparisons.
    - [[The Universal Relation|The Universal Relation]]https://ganelson.github.io/inform/assertions-module/8-tur.html - To define the universal relation, which can apply and therefore subsumes all other relations.
    - [[Explicit Relations|Explicit Relations]]https://ganelson.github.io/inform/assertions-module/8-er.html - To draw inferences from the relations created explicitly by the source text.
    - [[Listed-In Relations|Listed-In Relations]]https://ganelson.github.io/inform/assertions-module/8-lr.html - To define the binary predicates corresponding to table columns, and which determine whether a given value is listed in that column.
    - [[Adjective Ambiguity|Adjective Ambiguity]]https://ganelson.github.io/inform/assertions-module/8-aa.html - Managing the multiple contextual meanings which a single adjective can have.
    - [[Adjective Meanings|Adjective Meanings]]https://ganelson.github.io/inform/assertions-module/8-am.html - One individual meaning which an adjective can have.
    - [[Adjective Meaning Domains|Adjective Meaning Domains]]https://ganelson.github.io/inform/assertions-module/8-amd.html - What a single sense of an adjective can apply to: perhaps a kind or an instance.
    - [[Adjectives by Phrase|Adjectives by Phrase]]https://ganelson.github.io/inform/assertions-module/8-abp.html - Adjectives defined by an I7 phrase written out longhand.
    - [[Adjectives by Condition|Adjectives by Condition]]https://ganelson.github.io/inform/assertions-module/8-abc.html - Adjectives defined by a one-line I7 condition.
    - [[Adjectives by Inter Function|Adjectives by Inter Function]]https://ganelson.github.io/inform/assertions-module/8-abif.html - Defining an adjective with an Inter function to test or make it true.
    - [[Adjectives by Inter Condition|Adjectives by Inter Condition]]https://ganelson.github.io/inform/assertions-module/8-abic.html - Defining an adjective with an Inter condition.
    - [[Calculus Utilities|Calculus Utilities]]https://ganelson.github.io/inform/assertions-module/8-cu.html - Utility functions for creating basic propositions using these predicates.
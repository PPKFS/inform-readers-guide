---
{"dg-publish":true,"permalink":"/inform/imperative/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# imperative
```ad-info
Link: [https://ganelson.github.io/inform/imperative-module/index.html]]https://ganelson.github.io/inform/imperative-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```



# Contents
- -   Chapter 1: Configuration and Control
    - [[Imperative Module|Imperative Module]]https://ganelson.github.io/inform/imperative-module/1-im.html - Setting up the use of this module.
-   Chapter 2: Values
    - [[Compile Values|Compile Values]]https://ganelson.github.io/inform/imperative-module/2-cv.html - To compile specifications of values into Inter value opcodes or array entries.
    - [[Compile Rvalues|Compile Rvalues]]https://ganelson.github.io/inform/imperative-module/2-cr.html - To compile rvalues into Inter value opcodes or array entries.
    - [[Compile Lvalues|Compile Lvalues]]https://ganelson.github.io/inform/imperative-module/2-cl.html - To compile storage references into Inter value opcodes.
    - [[Compile Conditions|Compile Conditions]]https://ganelson.github.io/inform/imperative-module/2-cc.html - To compile Inter code to test a condition.
    - [[Matching Action Patterns|Matching Action Patterns]]https://ganelson.github.io/inform/imperative-module/2-map.html - Testing whether the current action matches an action pattern means compiling a complicated multi-clause condition, which is what this section does.
    - [[Matching Going Action Patterns|Matching Going Action Patterns]]https://ganelson.github.io/inform/imperative-module/2-mgap.html - Tweaks to compiling APs for the going action.
-   Chapter 3: Functions
    - [[Stack Frames|Stack Frames]]https://ganelson.github.io/inform/imperative-module/3-sf.html - When Inform compiles imperative code, it does so in the context of a "stack frame".
    - [[Local Variable Slates|Local Variable Slates]]https://ganelson.github.io/inform/imperative-module/3-lvs.html - The collection of Inter locals belonging to a stack frame.
    - [[Local Variables|Local Variables]]https://ganelson.github.io/inform/imperative-module/3-lv.html - Local variables are used for call parameters, temporary values, and other ephemeral workspace.
    - [[Temporary Variables|Temporary Variables]]https://ganelson.github.io/inform/imperative-module/3-tv.html - When the runtime code needs to borrow a global variable for a while.
    - [[Local Parking|Local Parking]]https://ganelson.github.io/inform/imperative-module/3-lp.html - Like Free Parking in Monopoly, except that it is not free and has an overhead cost.
    - [[Code Blocks|Code Blocks]]https://ganelson.github.io/inform/imperative-module/3-cb.html - Blocks of code are used to give conditionals and loops greater scope, as in more traditional programming languages.
    - [[Functions|Functions]]https://ganelson.github.io/inform/imperative-module/3-fnc.html - To compile Inter functions.
    - [[Jump Labels|Jump Labels]]https://ganelson.github.io/inform/imperative-module/3-jl.html - Generating numbered families of identifier names to use as jump labels, and creating any associated array storage needed.
    - [[Phrase Requests|Phrase Requests]]https://ganelson.github.io/inform/imperative-module/3-pr.html - To store and later fill requests to compile To... phrases.
    - [[Closures|Closures]]https://ganelson.github.io/inform/imperative-module/3-cls.html - To provide the names of phrases as first-class values.
    - [[Compile Imperative Definitions|Compile Imperative Definitions]]https://ganelson.github.io/inform/imperative-module/3-cid.html - Compiling an Inter function from the body of an imperative definition.
-   Chapter 4: Propositions
    - [[Compile Schemas|Compile Schemas]]https://ganelson.github.io/inform/imperative-module/4-cs.html - Here we compile fragments of code from paraphrases written in Inform 6 notation, and use that ability to compile general predicate calculus terms.
    - [[Compile Atoms|Compile Atoms]]https://ganelson.github.io/inform/imperative-module/4-ca.html - Given an atom of a proposition we compile Inter code to test it, to make it henceforth true, or to make it henceforth false.
    - [[Compile Propositions|Compile Propositions]]https://ganelson.github.io/inform/imperative-module/4-cp.html - To compile a proposition within the body of the current function.
    - [[Compile Loops|Compile Loops]]https://ganelson.github.io/inform/imperative-module/4-cl.html - To compile loop headers from a range of values expressed by a proposition.
    - [[Deciding to Defer|Deciding to Defer]]https://ganelson.github.io/inform/imperative-module/4-dtd.html - To decide whether a proposition can be compiled immediately, in the body of the current function, or whether it must be deferred to a function of its own, which is merely called from the current function.
    - [[Cinders and Deferrals|Cinders and Deferrals]]https://ganelson.github.io/inform/imperative-module/4-cad.html - Cinders are constants in deferred propositions referring to values in the original stack frame.
    - [[Compile Deferred Propositions|Compile Deferred Propositions]]https://ganelson.github.io/inform/imperative-module/4-cdp.html - To compile the Inter functions needed to perform the tests or tasks deferred as being too difficult in their original contexts.
-   Chapter 5: Invocations
    - [[Compile Blocks and Lines|Compile Blocks and Lines]]https://ganelson.github.io/inform/imperative-module/5-cbal.html - Compiling a code block of lines from an imperative definition.
    - [[Compile Invocations|Compile Invocations]]https://ganelson.github.io/inform/imperative-module/5-ci.html - Generating code to perform an invocation.
    - [[Compile Invocations As Calls|Compile Invocations As Calls]]https://ganelson.github.io/inform/imperative-module/5-ciac.html - An invocation defined with Inform 7 source text is made with an Inter function call.
    - [[Compile Invocations Inline|Compile Invocations Inline]]https://ganelson.github.io/inform/imperative-module/5-cii.html - Here we generate Inter code to invoke a phrase from its inline definition.
    - [[Compile Solutions to Equations|Compile Solutions to Equations]]https://ganelson.github.io/inform/imperative-module/5-cste.html - To compile code to solve an equation involving numerical quantities.
    - [[Compile Arithmetic|Compile Arithmetic]]https://ganelson.github.io/inform/imperative-module/5-ca.html - To compile code performing an arithmetic operation.
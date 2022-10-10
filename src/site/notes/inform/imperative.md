---
{"dg-publish":true,"permalink":"/inform/imperative/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# imperative
```ad-info
Link: [https://ganelson.github.io/inform/imperative-module/index.html]] https://ganelson.github.io/inform/imperative-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```

# Contents
- -   Chapter 1: Configuration and Control
    - [[inform/Imperative Module|Imperative Module]] - Setting up the use of this module.
-   Chapter 2: Values
    - [[inform/Compile Values|Compile Values]] - To compile specifications of values into Inter value opcodes or array entries.
    - [[inform/Compile Rvalues|Compile Rvalues]] - To compile rvalues into Inter value opcodes or array entries.
    - [[inform/Compile Lvalues|Compile Lvalues]] - To compile storage references into Inter value opcodes.
    - [[inform/Compile Conditions|Compile Conditions]] - To compile Inter code to test a condition.
    - [[inform/Matching Action Patterns|Matching Action Patterns]] - Testing whether the current action matches an action pattern means compiling a complicated multi-clause condition, which is what this section does.
    - [[inform/Matching Going Action Patterns|Matching Going Action Patterns]] - Tweaks to compiling APs for the going action.
-   Chapter 3: Functions
    - [[inform/Stack Frames|Stack Frames]] - When Inform compiles imperative code, it does so in the context of a "stack frame".
    - [[inform/Local Variable Slates|Local Variable Slates]] - The collection of Inter locals belonging to a stack frame.
    - [[inform/Local Variables|Local Variables]] - Local variables are used for call parameters, temporary values, and other ephemeral workspace.
    - [[inform/Temporary Variables|Temporary Variables]] - When the runtime code needs to borrow a global variable for a while.
    - [[inform/Local Parking|Local Parking]] - Like Free Parking in Monopoly, except that it is not free and has an overhead cost.
    - [[inform/Code Blocks|Code Blocks]] - Blocks of code are used to give conditionals and loops greater scope, as in more traditional programming languages.
    - [[inform/Functions|Functions]] - To compile Inter functions.
    - [[inform/Jump Labels|Jump Labels]] - Generating numbered families of identifier names to use as jump labels, and creating any associated array storage needed.
    - [[inform/Phrase Requests|Phrase Requests]] - To store and later fill requests to compile To... phrases.
    - [[inform/Closures|Closures]] - To provide the names of phrases as first-class values.
    - [[inform/Compile Imperative Definitions|Compile Imperative Definitions]] - Compiling an Inter function from the body of an imperative definition.
-   Chapter 4: Propositions
    - [[inform/Compile Schemas|Compile Schemas]] - Here we compile fragments of code from paraphrases written in Inform 6 notation, and use that ability to compile general predicate calculus terms.
    - [[inform/Compile Atoms|Compile Atoms]] - Given an atom of a proposition we compile Inter code to test it, to make it henceforth true, or to make it henceforth false.
    - [[inform/Compile Propositions|Compile Propositions]] - To compile a proposition within the body of the current function.
    - [[inform/Compile Loops|Compile Loops]] - To compile loop headers from a range of values expressed by a proposition.
    - [[inform/Deciding to Defer|Deciding to Defer]] - To decide whether a proposition can be compiled immediately, in the body of the current function, or whether it must be deferred to a function of its own, which is merely called from the current function.
    - [[inform/Cinders and Deferrals|Cinders and Deferrals]] - Cinders are constants in deferred propositions referring to values in the original stack frame.
    - [[inform/Compile Deferred Propositions|Compile Deferred Propositions]] - To compile the Inter functions needed to perform the tests or tasks deferred as being too difficult in their original contexts.
-   Chapter 5: Invocations
    - [[inform/Compile Blocks and Lines|Compile Blocks and Lines]] - Compiling a code block of lines from an imperative definition.
    - [[inform/Compile Invocations|Compile Invocations]] - Generating code to perform an invocation.
    - [[inform/Compile Invocations As Calls|Compile Invocations As Calls]] - An invocation defined with Inform 7 source text is made with an Inter function call.
    - [[inform/Compile Invocations Inline|Compile Invocations Inline]] - Here we generate Inter code to invoke a phrase from its inline definition.
    - [[inform/Compile Solutions to Equations|Compile Solutions to Equations]] - To compile code to solve an equation involving numerical quantities.
    - [[inform/Compile Arithmetic|Compile Arithmetic]] - To compile code performing an arithmetic operation.
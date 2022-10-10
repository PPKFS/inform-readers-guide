---
{"dg-publish":true,"permalink":"/inform/final/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# final
```ad-info

Link: [https://ganelson.github.io/inform/final-module/index.html](https://ganelson.github.io/inform/final-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```

# Contents
- Chapter 1: Setting Up
    [[Final Module|Final Module]] - Setting up the use of this module.
Chapter 2: Mechanism
    [[Code Generation|Code Generation]] - To generate final code from intermediate code.
    [[Code Generators|Code Generators]] - To create the range of possible targets into which Inter can be converted.
    [[Vanilla|Vanilla]] - The plain-vanilla code generation strategy, provided for the use of generators to imperative languages such as Inform 6 or C.
    [[Vanilla Constants|Vanilla Constants]] - How the vanilla code generation strategy handles constants, including literal texts, lists, and arrays.
    [[Vanilla Functions|Vanilla Functions]] - How the vanilla code generation strategy declares functions.
    [[Vanilla Objects|Vanilla Objects]] - How the vanilla code generation strategy handles instances, kinds, and properties.
    [[Vanilla Code|Vanilla Code]] - How the vanilla code generation strategy handles the actual code inside functions.
    [[Vanilla IF|Vanilla IF]] - Constructing the dictionary, command verb and action tables when the target language is not Inform 6 (where such things are made automatically).
Chapter 3: Non-Vanilla Generators
    [[Final Textual Inter|Final Textual Inter]] - To create the range of possible targets into which Inter can be converted.
    [[Final Binary Inter|Final Binary Inter]] - To create the range of possible targets into which Inter can be converted.
    [[Final Inventory|Final Inventory]] - To print a summary of the contents of a repository.
Chapter 4: Inform 6
    [[Generating Inform 6|Generating Inform 6]] - To generate I6 code from intermediate code.
    [[Inform 6 Constants|Inform 6 Constants]] - To declare I6 constants and arrays.
    [[Inform 6 Global Variables|Inform 6 Global Variables]] - To declare global variables, using a mixture of I6 Globals and array entries.
    [[Inform 6 Objects|Inform 6 Objects]] - To declare I6 objects, classes, attributes and properties.
    [[Inform 6 Code|Inform 6 Code]] - To generate I6 routines of imperative code.
Chapter 5: C
    [[Final C|Final C]] - To generate ANSI C-99 code from intermediate code.
    [[C Namespace|C Namespace]] - How identifiers are used in the C code we generate.
    [[C References|C References]] - How changes to storage objects are translated into C.
    [[C Global Variables|C Global Variables]] - Global variables translated to C.
    [[C Memory Model|C Memory Model]] - How arrays of all kinds are stored in C.
    [[C Assembly|C Assembly]] - The problem of assembly language.
    [[C Arithmetic|C Arithmetic]] - Integer and floating-point calculations translated to C.
    [[C Program Control|C Program Control]] - Generating C code to effect loops, branches and the like.
    [[C Conditions|C Conditions]] - Evaluating conditions.
    [[C Literals|C Literals]] - Text and dictionary words translated to C.
   [[C Object Model|C Object Model]] - How objects, classes and properties are compiled to C.
    [[C Function Model|C Function Model]] - Translating functions into C, and the calling conventions needed for them.
    [[C Input-Output Model|C Input-Output Model]] - How C programs print text out, really.
    [[C Miniglk |C Miniglk ]]- Just enough of the Glk input/output interface to allow simple console text in and out, and no more.
    [[C Utility Functions|C Utility Functions]] - Rounding out the C library with a few functions intended for external code to use.

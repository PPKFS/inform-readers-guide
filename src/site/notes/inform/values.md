---
{"dg-publish":true,"permalink":"/inform/values/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# values
```ad-info
Link: [https://ganelson.github.io/inform/values-module/index.html](https://ganelson.github.io/inform/values-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```



# Contents
- Chapter 1: Configuration and Control
	- [[inform/Values Module|Values Module]] - Setting up the use of this module.
	- [[inform/Meaning Codes (values)|Meaning Codes (values)]] - The set of meaning codes used when Inform runs the excerpt parser.
- Chapter 2: Specifications
	- [[inform/Specifications|Specifications]] - To create, manage and compare specifications.
	- [[inform/Rvalues|Rvalues]] - Specific values which can be stored or used at run-time.
	- [[inform/Lvalues|Lvalues]] - Storage locations into which rvalues can be put at run-time.
	- [[inform/Conditions|Conditions]] - States of being which at any given point, at run-time, might be true or false.
	- [[inform/Descriptions|Descriptions]] - Descriptions such as "open door" or "number which is greater than 8" which may or may not be true of any given rvalue at run-time.
- Chapter 3: Literals
	- [[inform/Parsing Literals|Parsing Literals]] - To decide if an excerpt of text is a value referred to notationally rather than by name.
	- [[inform/Literal Patterns (values)|Literal Patterns (values)]] - To manage the possible notations with which literal values can be written.
	- [[inform/Literal Real Numbers|Literal Real Numbers]] - To parse real numbers written as decimal expansions, or in scientific or engineering notation.
	- [[inform/Times of Day|Times of Day]] - To make a built-in kind of value for times of day, such as "11:22 AM".
	- [[inform/Unicode Literals|Unicode Literals]] - To manage the names assigned to Unicode character values.
	- [[inform/Transcoding Text|Transcoding Text]] - To change the escape-character conventions used in text streams.
	- [[inform/Literal Lists|Literal Lists]] - Parsing and vetting the kinds of literal lists written in braces.
- Chapter 4: The S-Parser
	- [[inform/Enter the S-Parser|Enter the S-Parser]] - The top-level nonterminals of the S-parser, which turns text into specifications.
	- [[inform/Constants and Descriptions|Constants and Descriptions]] - To parse noun phrases in constant contexts, which specify values either explicitly or by describing them more or less vaguely.
	- [[inform/Type Expressions and Values|Type Expressions and Values]] - To parse two forms of noun: a noun phrase in a sentence, and a description of what text can be written in a given situation.
	- [[inform/Verbal and Relative Clauses|Verbal and Relative Clauses]] - To break down an excerpt into NP and VP-like clauses, perhaps with a primary verb (to make a sentence), perhaps only a relative clause (to make a more complex NP).
	- [[inform/Conditions and Phrases|Conditions and Phrases]] - To parse the text of To... phrases, say phrases and conditions.
	- [[inform/Invocation Lists|Invocation Lists]] - Invocation lists are lists of alternate readings of the same wording to invoke a phrase.
	- [[inform/Invocations|Invocations]] - Invocations are to phrases what function calls are to functions, though they do not always compile that way.
	- [[inform/Parse Invocations|Parse Invocations]] - To register phrases with the excerpt parser, and to provide the excerpt parser with help in putting invocations together.
- Chapter 5: Type Checking
	- [[inform/Dash|Dash]] - The part of Inform most nearly like a typechecker in a conventional compiler.


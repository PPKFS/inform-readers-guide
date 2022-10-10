---
{"dg-publish":true,"permalink":"/inform/words/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# words
```ad-info
Link: https://ganelson.github.io/inform/words-module/index.html
```
# Overview

# Contents
-   Chapter 1: Setting Up
    - [[inform/Words Module|Words Module]]- Setting up the use of this module.
-   Chapter 2: Words in Isolation
    - [[inform/Vocabulary|Vocabulary]] - To classify the words in the lexical stream, where two different words are considered equivalent if they are unquoted and have the same text, taken case insensitively.
    - [[inform/Word Assemblages|Word Assemblages]] - To manage arbitrary assemblies of vocabulary, if a little slowly.
    - [[inform/Numbered Words|Numbered Words]] - Some utilities for handling single words referred to by number.
-   Chapter 3: Words in Sequence
    - [[inform/Lexer|Lexer]] - To break down a stream of characters into a numbered sequence of words, literal strings and literal I6 inclusions, removing comments and unnecessary whitespace.
    - [[inform/Wordings|Wordings]] - To manage contiguous word ranges.
    - [[inform/Text From Files|Text From Files]] - This is where source text is read in, whether from extension files or from the main source text file, and fed into the lexer.
    - [[inform/Feeds|Feeds]] - Feeds are conduits for arbitrary text to flow into the lexer, and to be converted into wordings.
    - [[inform/Identifiers|Identifiers]] - To summarise wordings into alphanumeric identifiers of the kind used by standard programming languages.
-   Chapter 4: Parsing
    - [[inform/About Preform|About Preform]] - A brief guide to Preform and how to use it.
    - [[inform/Nonterminals|Nonterminals]] - The angle-bracketed terms appearing in Preform grammar.
    - [[inform/Loading Preform|Loading Preform]] - To read in structural definitions of natural language written in the meta-language Preform.
    - [[inform/The Optimiser|The Optimiser]] - To precalculate data which enables rapid parsing of source text against a Preform grammar.
    - [[inform/Length Extremes|Length Extremes]] - To precalculate data which enables rapid parsing of source text against a Preform grammar.
    - [[inform/Nonterminal Incidences|Nonterminal Incidences]] - To work out bitmaps of nonterminal incidences in grammar.
    - [[inform/Preform|Preform]] - To parse the word stream against a general grammar defined by Preform.
    - [[inform/Basic Nonterminals|Basic Nonterminals]] - A handful of bare minimum Preform syntax.
    - [[inform/Instrumentation|Instrumentation]] - To provide debugging and tuning data on the Preform parser's performance.
    - [[inform/Preform Utilities|Preform Utilities]] - Other uses for Preform grammar, including the generation of adaptive text, and word inflection.
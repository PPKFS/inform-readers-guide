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
    - [[inform/Words Module|Words Module]]https://ganelson.github.io/inform/words-module/1-wm.html - Setting up the use of this module.
-   Chapter 2: Words in Isolation
    - [[inform/Vocabulary|Vocabulary]]https://ganelson.github.io/inform/words-module/2-vcb.html - To classify the words in the lexical stream, where two different words are considered equivalent if they are unquoted and have the same text, taken case insensitively.
    - [[inform/Word Assemblages|Word Assemblages]]https://ganelson.github.io/inform/words-module/2-wa.html - To manage arbitrary assemblies of vocabulary, if a little slowly.
    - [[inform/Numbered Words|Numbered Words]]https://ganelson.github.io/inform/words-module/2-nw.html - Some utilities for handling single words referred to by number.
-   Chapter 3: Words in Sequence
    - [[inform/Lexer|Lexer]]https://ganelson.github.io/inform/words-module/3-lxr.html - To break down a stream of characters into a numbered sequence of words, literal strings and literal I6 inclusions, removing comments and unnecessary whitespace.
    - [[inform/Wordings|Wordings]]https://ganelson.github.io/inform/words-module/3-wrd.html - To manage contiguous word ranges.
    - [[inform/Text From Files|Text From Files]]https://ganelson.github.io/inform/words-module/3-tff.html - This is where source text is read in, whether from extension files or from the main source text file, and fed into the lexer.
    - [[inform/Feeds|Feeds]]https://ganelson.github.io/inform/words-module/3-fds.html - Feeds are conduits for arbitrary text to flow into the lexer, and to be converted into wordings.
    - [[inform/Identifiers|Identifiers]]https://ganelson.github.io/inform/words-module/3-idn.html - To summarise wordings into alphanumeric identifiers of the kind used by standard programming languages.
-   Chapter 4: Parsing
    - [[inform/About Preform|About Preform]]https://ganelson.github.io/inform/words-module/4-ap.html - A brief guide to Preform and how to use it.
    - [[inform/Nonterminals|Nonterminals]]https://ganelson.github.io/inform/words-module/4-nnt.html - The angle-bracketed terms appearing in Preform grammar.
    - [[inform/Loading Preform|Loading Preform]]https://ganelson.github.io/inform/words-module/4-lp.html - To read in structural definitions of natural language written in the meta-language Preform.
    - [[inform/The Optimiser|The Optimiser]]https://ganelson.github.io/inform/words-module/4-to.html - To precalculate data which enables rapid parsing of source text against a Preform grammar.
    - [[Length Extremes|Length Extremes]]https://ganelson.github.io/inform/words-module/4-le.html - To precalculate data which enables rapid parsing of source text against a Preform grammar.
    - [[Nonterminal Incidences|Nonterminal Incidences]]https://ganelson.github.io/inform/words-module/4-ni.html - To work out bitmaps of nonterminal incidences in grammar.
    - [[Preform|Preform]]https://ganelson.github.io/inform/words-module/4-prf.html - To parse the word stream against a general grammar defined by Preform.
    - [[Basic Nonterminals|Basic Nonterminals]]https://ganelson.github.io/inform/words-module/4-bn.html - A handful of bare minimum Preform syntax.
    - [[Instrumentation|Instrumentation]]https://ganelson.github.io/inform/words-module/4-ins.html - To provide debugging and tuning data on the Preform parser's performance.
    - [[Preform Utilities|Preform Utilities]]https://ganelson.github.io/inform/words-module/4-pu.html - Other uses for Preform grammar, including the generation of adaptive text, and word inflection.
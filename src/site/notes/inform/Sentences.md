---
{"dg-publish":true,"permalink":"/inform/sentences/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Sentences
```ad-info

Link: [https://ganelson.github.io/inform/syntax-module/3-snt.html](https://ganelson.github.io/inform/syntax-module/3-snt.html)
Up: [[syntax]]
```

# Contents
- Fairly straightforward. It takes a list of tokens from [[inform/Lexer|Lexer]] and breaks up at whatever delimiter.
- It has some handling for rules that can end in colons, and for skipping excess punctuation.
- It makes a bunch of [[inform/Headings|Headings]] in a basic syntax tree (see [[inform/Syntax Trees|Syntax Trees]]) so it can skip them if necessary.
- Need to find wherever [[structural-sentence|structural-sentence]] and [[dividing-sentence|dividing-sentence]] are defined. They seem to be important.
- There’s some special cases for the serial comma, so that “Some list of, things, or other, instead…” is correctly broken in two.
- Lots of [[inform/Node Annotations|Node Annotations]] but nothing fancy.

## Preform used here
- [[structural-sentence|structural-sentence]]
- [[dividing-sentence|dividing-sentence]]

## Preform defined here
- [[list-or-division|list-or-division]]
- [[if-start-of-source-text|if-start-of-source-text]]

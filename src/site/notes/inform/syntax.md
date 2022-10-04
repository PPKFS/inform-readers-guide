---
{"dg-publish":true,"permalink":"/inform/syntax/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# syntax
```ad-info
Link: https://ganelson.github.io/inform/syntax-module/index.html
```
# Contents
- Chapter 1 - Setting Up
	- [[Syntax Module|Syntax Module]] - Setting up the use of this module.
- Chapter 2 - The Parse Tree
	- [[Syntax Trees|Syntax Trees]] - To parse trees which decompose the meaning of excerpts of text, and which allow annotations to be made at each node.
	- [[Node Types|Node Types]] - Each node in a syntax tree has a type, which informs whether it can have child nodes, and what in general terms it means.
	- [[Parse Nodes|Parse Nodes]] - Syntax trees are made of single nodes, each representing one way to understand a given piece of text.
	- [[Node Annotations|Node Annotations]] - Attaching general-purpose data to nodes in the syntax tree.
	- [[Tree Verification|Tree Verification]] - Did we go wrong anywhere? This section is purely defensive, and tests whether Inform contains bugs of a kind which lead to malformed syntax trees: that should never happen even if the source text being compiled is a dumpster fire.
	- [[Simple Preform Cache|Simple Preform Cache]] - A simple way to speed up repeated Preform parses of the same text.
- Chapter 3 - Breaking into Sentences
	- [[Sentences|Sentences]] - To break up the stream of words produced by the lexer into English sentences, and join each to the parse tree.
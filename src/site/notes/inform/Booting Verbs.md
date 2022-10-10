---
{"dg-publish":true,"permalink":"/inform/booting-verbs/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Booting Verbs
```ad-info

Link: [https://ganelson.github.io/inform/assertions-module/2-bv.html](https://ganelson.github.io/inform/assertions-module/2-bv.html)
Up: [[inform/assertions|assertions]]
```

# Contents
- This is another key module that sort of hides away. A lot of sentences are not quite assertions or existentials and the only call in the [[inform/Compilation Flow|Compilation Flow]] is to [[inform/Passes through Major Nodes|Passes through Major Nodes]].
- The callback registry is in [[inform/Special Meanings|Special Meanings]].
- Each of these does a different thing based on the current task. When looking for a verb in [[inform/Verb Phrases|Verb Phrases]], this is always the `ACCEPT_SMFT` task.  Check [[inform/Special Meanings|Special Meanings]].
- So this is where all the various “X request” modules in [[assertions]] are hooked in.
- We also create `to be` and `to mean` via [[inform/Preform Utilities|Preform Utilities]], [[inform/Verb Conjugation|Verb Conjugation]] in [[inform/inflections|inflections]], and [[inform/Verb Usages|Verb Usages]] in [[inform/linguistics|linguistics]] 
- In no particular order:
	- [[inform/New Relation Requests|New Relation Requests]] 
		- `new-relation`
	- [[inform/Rule Placement Requests|Rule Placement Requests]] 
		- `rule-substitutes-for`
		- `rule-does-nothing`
		- `rule-does-nothing-if`
		- `rule-does-nothing-unless`
		- `rule-listed-in`
	- [[inform/Translation Requests|Translation Requests]]
		- `translates-into-unicode
		- `translates-into-i6`
		- `translates-into-language`
	- [[inform/Test Requests|Test Requests]]
		- `test-with`
	- [[inform/New Verb Requests|New Verb Requests]]
		- `new-verb`
	- [[inform/Pluralisation Requests|Pluralisation Requests]]
		- `new-plural`
	- [[inform/New Activity Requests|New Activity Requests]]
		- `new-activity`
	- [[inform/New Adjective Requests|New Adjective Requests]]
		- `new-adjective`
	- [[inform/New Property Requests|New Property Requests]]
		- `new-either-or`
		- `can-be`
		- `verb-means`
	- [[inform/Define by Table Requests|Define by Table Requests]]
		- `defined-by-table`
	- [[inform/New Literal Pattern Requests|New Literal Pattern Requests]]
		- `specifies-notation`
	- [[inform/New Use Option Requests|New Use Option Requests]]
		- `use-translates`
	- [[inform/Use Options (assertions)|Use Options (assertions)]]
		- `use`
	- [[inform/Debugging Log Requests|Debugging Log Requests]]
		- `include-in`
		- `omit-from`

## Preform defined here
- [[bootstrap-verb|bootstrap-verb]]
- [[relation-names|relation-names]]
---
{"dg-publish":true,"permalink":"/inform/compilation-flow/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Compilation Flow
- A vague overview of the flow because it’s too many links back and forth

## Build setup
- [[inform/Main|Main]] is the entry point
	- This then goes to [[inform/Inbuild Control|Inbuild Control]] for the setup of the project
		- Which creates objects from [[inform/Project File Manager|Project File Manager]] and [[inform/Project Bundle Manager|Project Bundle Manager]]
		- And all the various build skill/step modules
	- The [[inform/Inform7 Skill|Inform7 Skill]] is the final part of [[inform/supervisor|supervisor]] we use for now, which goes to [[inform/core|core]] via `Task::carry_out` in [[inform/What To Compile|What To Compile]] and then [[inform/How To Compile|How To Compile]] which has the actual passes.
## Reading and Lexing
- In [[inform/Project Services|Project Services]] there is `Projects::read_source_text_for` which does the lexing and sentence breaking
	- The lexing is through [[Source Text|Source Text]] → [[Text From Files|Text From Files]] → [[inform/Lexer|Lexer]]
	- The sentence breaking is just [[Sentences|Sentences]] directly
- Technically this is all *before* the Inform7 skill.

## Parsing

## Values

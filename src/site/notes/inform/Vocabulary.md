---
{"dg-publish":true,"permalink":"/inform/vocabulary/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Vocabulary
```ad-info
Link: [https://ganelson.github.io/inform/words-module/2-vcb.html](https://ganelson.github.io/inform/words-module/2-vcb.html)
Up: [[words]]
```



# Contents
- This covers basically everything about individual words themselves.
- There’s a handful of various `MC` ([[Meaning Codes|Meaning Codes]]) that are used everywhere. These seem self-explanatory.
- The `vocabulary_entry` struct:
| Field                               | Description                                                    |
| ----------------------------------- | -------------------------------------------------------------- |
| `flags`                             | [[Meaning Codes|Meaning Codes]], see above                                   |
| `literal_number_value`              | Shorthand evaluation of this word as a number                  |
| `exemplar`, `raw_exemplar`          | Examples of the vocabulary which I’ve still not found a use of |
| `hash`, `next_in_vocab_hash`        | Some hash table information                                    |
| `lower_case_form`,`upper_case_form` | For words where the surprise upper case might mean something   |
- [[Inform TODO list|Inform TODO list]] - find wherever these `exemplar` fields are used.
- A bunch of default punctuation is made first in [[inform/Words Module|Words Module]], I guess to ensure it’s at the start of the hash table bucket?
- `identify_word` is the [main entry point](https://ganelson.github.io/inform/words-module/2-vcb.html#SP3) of adding new words, which is called via the [[inform/Lexer|Lexer]] and apparently also in [[inform/Numbered Words|Numbered Words]]?
	- `entry_for_text` [either adds it or looks it up](https://ganelson.github.io/inform/words-module/2-vcb.html#SP15).
	- [And creates a new entry for it](https://ganelson.github.io/inform/words-module/2-vcb.html#SP5) .
	- If we are using the [[Excerpt Meanings|Excerpt Meanings]] then we have a callback here.
	- For the most part the `upper_case_form` seems to be unused, except by calling `Vocabulary::make_case_sensitive` which happens in [[Excerpt Meanings|Excerpt Meanings]] .
- Most of this module is creating their own hash table and access functions.

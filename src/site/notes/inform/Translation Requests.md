---
{"dg-publish":true,"permalink":"/inform/translation-requests/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Translation Requests
```ad-info

Link: [https://ganelson.github.io/inform/assertions-module/3-tr.html](https://ganelson.github.io/inform/assertions-module/3-tr.html)
Up: [[assertions]]
```

# Contents
This is actually 3 different sentences in a trenchcoat; translating into a language, into i6, and into unicode.
- into a language accepts it in the `ACCEPT_SMFT` phase and hands it to linguistics ([[Instances (knowledge)|Instances (knowledge)]] or [[inform/Kind Constructors|Kind Constructors]] and [[inform/Nouns|Nouns]]) after we have made kinds.
- The unicode translation is made into a proper noun [[inform/Nouns|Nouns]] and also given the `MISCELLANEOUS_MC` [[Meaning Codes|Meaning Codes]]. 
- The inter translation depends on which kind of inter translation; mostly handled in pass 1 and 2, but the `INTER_NAMING_SMFT` pass for nouns is the `Translations::late_naming_requests` from the compilation flow.
	- Properties go via [[inform/Properties (knowledge)|Properties (knowledge)]]
	- Rules go via [[inform/Rules (assertions)|Rules (assertions)]] in pass 1 and in pass 2 we check for additional responses for [[inform/Responses|Responses]]
	- Variables go via [[inform/Nonlocal Variables|Nonlocal Variables]]
	- Actions go via [[inform/Actions (if)|Actions (if)]]
	- Grammar tokens go via [[inform/Command Grammars (if)|Command Grammars (if)]]
	- Nouns go later because we need to have them existing in the model world, and we have [[inform/Noun Identifiers|Noun Identifiers]] and [[inform/Lexicon (lexicon)|Lexicon (lexicon)]] for lookups.

## Preform used here
- [[np-articled|np-articled]]
- [[k-kind|k-kind]]
- [[instance|instance]]
- [[cardinal-number-unlimited|cardinal-number-unlimited]]
- [[unicode-character-name|unicode-character-name]]
- [[quoted-text|quoted-text]]
- [[response-letter|response-letter]]
- [[rule-name|rule-name]]

## Preform defined here
- [[translation-target-language|translation-target-language]]
- [[translates-into-language-sentence-subject|translates-into-language-sentence-subject]]
- [[translation-target-unicode|translation-target-unicode]]
- [[translates-into-unicode-sentence-object|translates-into-unicode-sentence-object]]
- [[translates-into-unicode-sentence-subject|translates-into-unicode-sentence-subject]]
- [[translation-target-i6|translation-target-i6]]
- [[translates-into-i6-sentence-subject|translates-into-i6-sentence-subject]]
- [[translates-into-i6-sentence-object|translates-into-i6-sentence-object]]
- [[extra-response|extra-response]]
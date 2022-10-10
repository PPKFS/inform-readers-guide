---
{"dg-publish":true,"permalink":"/inform/new-use-option-requests/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# New Use Option Requests
```ad-info

Link: [https://ganelson.github.io/inform/assertions-module/3-nuor.html](https://ganelson.github.io/inform/assertions-module/3-nuor.html)
Up: [[assertions]]
```

# Contents
Mostly this is more technical, under the hood stuff. It appears that the codes are defined in [[inform/Compilation Settings|Compilation Settings]], but we also hook in to some compiler level stuff here as well ([[inform/Rvalues|Rvalues]] and [[inform/Use Options (runtime)|Use Options (runtime)]]).

If we cannot parse it - namely it’s not noted in [[inform/Lexicon (lexicon)|Lexicon (lexicon)]] - then it must be a new miscellaneous use option name. We apparently also make a new [[inform/Nouns|Nouns]] noun here? Though I’m not yet sure why.

Another simple case of accepting early and just shrugging and then doing the actual work in a later phase.

## Preform defined here
[[use-translates-as-sentence-subject|use-translates-as-sentence-subject]]
[[use-translates-as-sentence-object|use-translates-as-sentence-object]]

## Preform used here
[[np-unparsed|np-unparsed]]
[[notable-use-option-name|notable-use-option-name]]
[[use-setting|use-setting]]
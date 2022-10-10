---
{"dg-publish":true,"permalink":"/inform/special-meanings/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Special Meanings
```ad-info

Link: [https://ganelson.github.io/inform/linguistics-module/3-sm.html ](https://ganelson.github.io/inform/linguistics-module/3-sm.html )
Up: [[linguistics]]
```

# Contents
- - This is documenting the various `_SMFT` tasks.
	- `ACCEPT_SMFT` - called when trying to find a verb; each of the special meaning sentences defined in [[inform/Booting Verbs|Booting Verbs]] and it’s called in [[inform/Verb Phrases|Verb Phrases]]. For special meaning sentences it’s a maybe, but if we fall through to a “regular” meaning it’s always true (because at this point we have accepted a verb).
	- `PASS_1_SMFT` and `PASS_2_SMFT` are done for their corresponding passes in [[inform/Passes through Major Nodes|Passes through Major Nodes]].
	- `INTER_NAMING_SMFT` checks specifically for nouns defined in I6.
	- `ALLOW_IN_OPTIONS_FILE_SMFT` is set in [[inform/Classifying Sentences|Classifying Sentences]]. Oh, it’s for specifically [[inform/The Options File|The Options File]] 
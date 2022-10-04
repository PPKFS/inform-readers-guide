---
{"dg-publish":true,"permalink":"/inform/text-from-files/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Text From Files
```ad-info
Link: [https://ganelson.github.io/inform/words-module/3-tff.html](https://ganelson.github.io/inform/words-module/3-tff.html)
Up: [[words]]
```



# Contents
- This has the `source_file` struct, which is sort of the intermediary parse representation. 
- It feeds entire files into the [[inform/Lexer|Lexer]] (except for the generated source).
- It does some Unicode handling here to make characters neater.
- The word count is separate from the actual count of “words” because it considers quoted text as multiple words.
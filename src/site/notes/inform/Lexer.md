---
{"dg-publish":true,"permalink":"/inform/lexer/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Lexer
```ad-info
Link: [https://ganelson.github.io/inform/words-module/3-lxr.html](https://ganelson.github.io/inform/words-module/3-lxr.html)
Up: [[words]]
```

# Contents
- I wrote a bunch of this stuff for the blog post already, but this should probably be a shorter version.
- This module is fairly compartmentalised. It is given a text stream by [[inform/Text From Files|Text From Files]] (for actual source) and [[inform/Feeds|Feeds]] (for generated source) and therefore doesn’t need to hook into the build process more generally.
- The two places are in [feeding the lexer](https://ganelson.github.io/inform/words-module/3-lxr.html#SP17) where it creates a [[inform/Wordings|Wordings]] wording from the entire feed in, and then [the final identification of each word](https://ganelson.github.io/inform/words-module/3-lxr.html#SP27_5) by identifying it in [[inform/Vocabulary|Vocabulary]]
- I need to check where the external lexer flags are set - [[Inform TODO list|Inform TODO list]]
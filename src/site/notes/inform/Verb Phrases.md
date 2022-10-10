---
{"dg-publish":true,"permalink":"/inform/verb-phrases/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Verb Phrases
```ad-info

Link: [https://ganelson.github.io/inform/linguistics-module/4-vp.html ](https://ganelson.github.io/inform/linguistics-module/4-vp.html )
Up: [[linguistics]]
```

# Contents
- This is [[the big one|the big one]], in my opinion. This is where the verb is identified for each sentence.
There are two different sentence preform matches, one that avoids matching “for the first time” because the polymorphism of `time` causes problems. [[Inform TODO list|Inform TODO list]] - why is this? Either way, they’re both the same call followed by some neatening up.

https://ganelson.github.io/inform/linguistics-module/4-vp.html#SP4 has some example parses.
The first one, `beth is a sailor`, is straightforward.
The second one, `there is a ming vase which is on the table`, has 2 possible verbs (`is` and `is on`). The first one has a defective subject (`there`), which means we don’t get any information? from it. We instead look at the second clause and notice the `is on`. I’m not sure where the `existential_OP_edge` is set in this second one.
In the third one, `there is a ming vase on the table called the table of having` there are again 2 verbs (`is` and `of`) but this time we only search as far as `called` for some reason? [[inform/Wordings|Wordings]] `up_to` is inclusive.

This is in two halves, calculating the viability map and then looking for the usages.

### Viability map
- For every word, we check and see if it matches the [[nonimperative-verb|nonimperative-verb]] Preform. ([[inform/Verb Usages|Verb Usages]])
	- If it does, then we see if the sentence up until this point in some way via [[negated-noncopular-verb-present|negated-noncopular-verb-present]] . `pos` is the absolute word number, whereas `i` is the relative one. We are looking for the negated verb *starting* at `pos`. We then…skip ahead that many words, and then skip back 1 word?
- If we do find something, then we break the wording in half, except in the case of [[pre-verb-rc-marker|pre-verb-rc-marker]]

### Finding usages
## Preform defined here
[[sentence|sentence]]
[[sentence-without-occurrences|sentence-without-occurrences]]
[[pre-verb-certainty|pre-verb-certainty]]
[[post-verb-certainty|post-verb-certainty]]
[[rc-marker|rc-marker]]
[[pre-verb-rc-marker|pre-verb-rc-marker]]
[[phrase-with-calling|phrase-with-calling]]
[[np-x-of-y|np-x-of-y]]

## Preform used here
[[nonimperative-verb|nonimperative-verb]]
[[negated-noncopular-verb-present|negated-noncopular-verb-present]]
[[np-existential|np-existential]]
[[np-as-object|np-as-object]]
[[np-as-subject|np-as-subject]]
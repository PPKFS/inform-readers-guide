---
{"dg-publish":true,"permalink":"/inform/kinds/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# kinds
```ad-info

Link: [https://ganelson.github.io/inform/kinds-module/index.html](https://ganelson.github.io/inform/kinds-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```

# Contents
- Chapter 1: Starting Up
	- Kinds Module - Setting up the use of this module.

- Chapter 2: Kinds
	- [[inform/kinds|Kinds]] - To build tree structures which represent Inform's universe of kinds.
	- [[Familiar Kinds|Familiar Kinds]] - To recognise certain kind names as familiar built-in ones.
	- [[The Lattice of Kinds|The Lattice of Kinds]] - Placing a partial order on kinds according to whether one conforms to another.
	- [[Describing Kinds|Describing Kinds]] - Translating kinds to and from textual descriptions.
	- [[Using Kinds|Using Kinds]] - To determine the characteristics of different kinds, enabling them to be used in practice.
- Chapter 3: Arithmetic
	- [[Dimensions|Dimensions]] - To keep a small database indicating the physical dimensions of numerical values, and how they combine: for instance, allowing us to specify that a length times a length is an area.
	- [[Floating-Point Values|Floating-Point Values]] - To cope with promotions from integer to floating-point arithmetic.
	- [[Scaled Arithmetic Values|Scaled Arithmetic Values]] - To manage the scalings and offsets used when storing arithmetic values at run-time, and/or when using scaled units to refer to them.
- Chapter 4: Constructors
    - [[A Brief Guide to Neptune|A Brief Guide to Neptune]] - A manual for the mini-language used in Neptune files.
    - [[Neptune Files|Neptune Files]] - To read in details of built-in kind constructors from so-called Neptune files, setting them up ready for use.
    - [[Neptune Syntax|Neptune Syntax]] - To parse individual commands from Neptune files.
    - [[Macros|Macros]] - Neptune supports named macros, though they are only lists of kind commands.
    - [[Star Templates|Star Templates]] - Allowing Neptune files to generate additional source text.
    - [[Kind Commands|Kind Commands]] - To apply a given command to a given kind constructor.
    - [[inform/Kind Constructors|Kind Constructors]] - The mechanism by which Inform records the characteristics of different kinds.

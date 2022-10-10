---
{"dg-publish":true,"permalink":"/inform/bytecode/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# bytecode
```ad-info

Link: [https://ganelson.github.io/inform/bytecode-module/index.html](https://ganelson.github.io/inform/bytecode-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```

# Contents
- Chapter 1: Setting Up
    Bytecode Module - Setting up the use of this module.
    The Inter Version - The semantic version number for the current definition of Inter bytecode.
- Chapter 2: The Trees
    Inter Trees - To manage tree structures of inter code, and manage the movement of nodes within these trees.
    Inter Nodes - To create nodes of inter code, and manage everything about them except their tree locations.
    Bookmarks - Write positions for inter code being generated.
    Node Placement - Moving nodes in a tree, adding them to a tree, removing them from a tree.
    The Warehouse - To manage the memory storage of inter code.
    Packages - To manage packages of inter code.
    Inter Node Lists - Utility functions to store lists of nodes, either as linked lists or flexibly-sized arrays.
    Symbols Tables - To manage searchable tables of named symbols.
    Symbols - To manage named symbols in inter code.
    Annotations - To mark symbols up with metadata.
    The Wiring - Wiring symbols in one package to meanings in another, and via plugs and sockets even to packages in trees not yet loaded in.
    Transmigration - The act of moving a package from one Inter tree to another.
- Chapter 3: Their Instructions
    Inter Constructs - There are around two dozen constructs in textual Inter source code, with each instruction in bytecode being a usage of one of them.
    Inter in Binary Files - To read or write inter between memory and binary files.
    Inter in Text Files - To read a tree from a file written in the plain text version of Inter.
    Verifying Inter - Verifying that a new Inter instruction is correct and consistent.
    Inter Value Pairs - Two consecutive bytecode words are used to store a single value in binary Inter.
    Inter Data Types - A primitive notion of data type, below the level of kinds.
    Metadata - Looking up metadata in special constants.
    Inter Errors - To issue error messages arising from loading incorrect Inter code from files.
- Chapter 4: Void Constructs
    The Comment Construct - Defining the comment construct.
    The Constant Construct - Defining the constant construct.
    The Insert Construct - Defining the insert construct.
    The Instance Construct - Defining the instance construct.
    The Nop Construct - Defining the nop construct.
    The Package Construct - Defining the package construct.
    The PackageType Construct - Defining the packagetype construct.
    The Permission Construct - Defining the permission construct.
    The Pragma Construct - Defining the pragma construct.
    The Primitive Construct - Defining the primitive construct.
    The Property Construct - Defining the property construct.
    The PropertyValue Construct - Defining the propertyvalue construct.
    The Typename Construct - Defining the typename construct.
    The Variable Construct - Defining the variable construct.
- Chapter 5: Code Constructs
    The Assembly Construct - Defining the assembly construct.
    The Cast Construct - Defining the cast construct.
    The Code Construct - Defining the Code construct.
    The Evaluation Construct - Defining the Evaluation construct.
    The Inv Construct - Defining the inv construct.
    The Lab Construct - Defining the Lab construct.
    The Label Construct - Defining the label construct.
    The Local Construct - Defining the local construct.
    The Ref Construct - Defining the ref construct.
    The Reference Construct - Defining the Reference construct.
    The Splat Construct - Defining the splat construct.
    The Val Construct - Defining the val construct.
- Chapter 6: Pseudo-Constructs
    The Plug Construct - Defining the symbol construct.
    The Socket Construct - Defining the socket construct.
    The Version Construct - Defining the version construct.


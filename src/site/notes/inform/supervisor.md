---
{"dg-publish":true,"permalink":"/inform/supervisor/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# supervisor
```ad-info
Link: https://ganelson.github.io/inform/supervisor-module/index.html
```
# Overview
- Mostly just driving the compilation.
# Contents
-   Chapter 1: Setting Up
    - [[inform/Supervisor Module|Supervisor Module]]- Setting up the use of this module.
    - [[inform/Inbuild Control|Inbuild Control]]- Who shall supervise the supervisor? This section of code will.
-   Chapter 2: Conceptual Framework
    - [[inform/Genres|Genres]] - The different sorts of work managed by inbuild.
    - [[inform/Works|Works]] - To store, hash code and compare title/author pairs used to identify works.
    - [[inform/Editions|Editions]] - An edition is a numbered version of a work.
    - [[inform/Copies|Copies]] - A copy is an instance in the file system of a specific edition of a work.
    - [[inform/Copy Errors|Copy Errors]] - A copy error is attached to a copy when scanning it reveals some malformation.
    - [[inform/Requirements|Requirements]]- A requirement is a way to specify some subset of works: for example, those with a given title, and/or version number.
    - [[inform/Nests|Nests]] - Nests are repositories of Inform-related resources.
    - [[inform/Registries|Registries]] - Registries are nests provided with metadata and intended to be presented as an online source from which Inform resources can be downloaded.
    - [[inform/JSON Metadata|JSON Metadata]] - Managing JSON-encoded metadata files for resources such as kits.
-   Chapter 3: Incremental Builds
    - [[inform/Build Graphs|Build Graphs]] - Graphs in which vertices correspond to files or copies, and edges to dependencies between them.
    - [[inform/Build Methodology|Build Methodology]]- Whether to run tasks internally in some merged tool, or run via the shell, or simply trace to the standard output what we think ought to be done.
    - [[inform/Incremental Building|Incremental Building]]- Deciding what is the least possible amount which needs to be built, in what order, to arrive at a working version of a copy.
    - [[inform/Build Scripts|Build Scripts]] - Scripts are nothing more than lists of build steps.
    - [[inform/Build Steps|Build Steps]]- A build step is a task which exercises one of the build skills.
    - [[inform/Inter Skill|Inter Skill]] - The skills of kit building and of code generation from Inter.
    - [[inform/Inform7 Skill|Inform7 Skill]] - The skill of turning source text into Inter code.
    - [[inform/Inform6 Skill|Inform6 Skill]] - The skill of compiling Inform 6 into a story file for the target VM.
    - [[inform/Inblorb Skill|Inblorb Skill]] - The skill of packaging a story file and associated resources into a blorb.
-   Chapter 4: Genre Management
    - [[inform/Extension Manager|Extension Manager]] - Claiming and creating copies of the extension genre: used for Inform 7 extensions.
    - [[inform/Kit Manager|Kit Manager]] - Claiming and creating copies of the kit genre: used for kits of precompiled Inter code.
    - [[inform/Language Manager|Language Manager]] - Claiming and creating copies of the language genre: used for bundles of natural language metadata in the Inform 7 compiler.
    - [[inform/Pipeline Manager|Pipeline Manager]]- Claiming and creating copies of the pipeline genre: used for pipelines of code-generation stages.
    - [[inform/Project Bundle Manager|Project Bundle Manager]]- Claiming and creating copies of the projectbundle genre: used for Inform 7 projects as created by the GUI apps.
    - [[inform/Project File Manager|Project File Manager]] - Claiming and creating copies of the projectfile genre: used for Inform 7 source texts stored as stand-alone plain text files, outside the GUI apps.
    - [[inform/Template Manager|Template Manager]]- Claiming and creating copies of the template genre: used for website and interpreter templates when releasing an Inform project.
-   Chapter 5: Genre Services
    - [[inform/Extension Services|Extension Services]] - Behaviour specific to copies of the extension genre.
    - [[inform/Kit Services|Kit Services]]- Behaviour specific to copies of the kit genre.
    - [[inform/Language Services|Language Services]] - Behaviour specific to copies of the language genre.
    - [[inform/Pipeline Services|Pipeline Services]] - Behaviour specific to copies of the pipeline genre.
    - [[inform/Project Services|Project Services]] - Behaviour specific to copies of either the projectbundle or projectfile genres.
    - [[inform/Template Services|Template Services]] - Behaviour specific to copies of the template genre.
-   Chapter 6: Inform Source Text
    - [[inform/Source Text|Source Text]]- Using the lexer and syntax analysis modules to read in Inform 7 source text.
    - [[inform/Headings|Headings]]- To keep track of the hierarchy of headings and subheadings found in the source text.
    - [[inform/The Options File|The Options File]] - The optional file of Options applied to all of the user's projects.
    - [[inform/Inclusions|Inclusions]]- To fulfill requests to include extensions, adding their material to the parse tree as needed, and removing INCLUDE nodes.
    - [[inform/Control Structures|Control Structures]]- To specify the syntax of control structures such as repeat, if and otherwise.
    - [[inform/Virtual Machine Grammar|Virtual Machine Grammar]] - Grammar for parsing natural language descriptions of a virtual machine.
-   Chapter 7: Extension Indexing
    - [[inform/The Mini-Website|The Mini-Website]]- To refresh the mini-website of available extensions presented in the Inform GUI applications.
    - [[inform/Dictionary|Dictionary]] - To maintain a database of names and constructions in all extensions so far used by this installation of Inform, and spot potential namespace clashes.
    - [[inform/Census|Census]] - To conduct a census of all installed extensions installed.
    - [[inform/Index Pages|Index Pages]] - To generate the two top-level pages in the extension mini-website.
    - [[inform/Individual Pages|Individual Pages]]- To generate the individual pages on extensions in the extension mini-website.
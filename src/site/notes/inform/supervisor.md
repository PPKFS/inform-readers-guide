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
    - [[Supervisor Module|Supervisor Module]]https://ganelson.github.io/inform/supervisor-module/1-sm.html - Setting up the use of this module.
    - [[inform/Inbuild Control|Inbuild Control]]- Who shall supervise the supervisor? This section of code will.
-   Chapter 2: Conceptual Framework
    - [[Genres|Genres]]https://ganelson.github.io/inform/supervisor-module/2-gnr.html - The different sorts of work managed by inbuild.
    - [[Works|Works]]https://ganelson.github.io/inform/supervisor-module/2-wrk.html - To store, hash code and compare title/author pairs used to identify works.
    - [[Editions|Editions]]https://ganelson.github.io/inform/supervisor-module/2-edt.html - An edition is a numbered version of a work.
    - [[inform/Copies|Copies]] - A copy is an instance in the file system of a specific edition of a work.
    - [[Copy Errors|Copy Errors]]https://ganelson.github.io/inform/supervisor-module/2-ce.html - A copy error is attached to a copy when scanning it reveals some malformation.
    - [[Requirements|Requirements]]https://ganelson.github.io/inform/supervisor-module/2-rqr.html - A requirement is a way to specify some subset of works: for example, those with a given title, and/or version number.
    - [[Nests|Nests]]https://ganelson.github.io/inform/supervisor-module/2-nst.html - Nests are repositories of Inform-related resources.
    - [[Registries|Registries]]https://ganelson.github.io/inform/supervisor-module/2-rgs.html - Registries are nests provided with metadata and intended to be presented as an online source from which Inform resources can be downloaded.
    - [[JSON Metadata|JSON Metadata]]https://ganelson.github.io/inform/supervisor-module/2-jm.html - Managing JSON-encoded metadata files for resources such as kits.
-   Chapter 3: Incremental Builds
    - [[Build Graphs|Build Graphs]]https://ganelson.github.io/inform/supervisor-module/3-bg.html - Graphs in which vertices correspond to files or copies, and edges to dependencies between them.
    - [[Build Methodology|Build Methodology]]https://ganelson.github.io/inform/supervisor-module/3-bm.html - Whether to run tasks internally in some merged tool, or run via the shell, or simply trace to the standard output what we think ought to be done.
    - [[inform/Incremental Building|Incremental Building]]- Deciding what is the least possible amount which needs to be built, in what order, to arrive at a working version of a copy.
    - [[inform/Build Scripts|Build Scripts]] - Scripts are nothing more than lists of build steps.
    - [[inform/Build Steps|Build Steps]]- A build step is a task which exercises one of the build skills.
    - [[Inter Skill|Inter Skill]]https://ganelson.github.io/inform/supervisor-module/3-is.html - The skills of kit building and of code generation from Inter.
    - [[inform/Inform7 Skill|Inform7 Skill]]https://ganelson.github.io/inform/supervisor-module/3-is2.html - The skill of turning source text into Inter code.
    - [[Inform6 Skill|Inform6 Skill]]https://ganelson.github.io/inform/supervisor-module/3-is3.html - The skill of compiling Inform 6 into a story file for the target VM.
    - [[Inblorb Skill|Inblorb Skill]]https://ganelson.github.io/inform/supervisor-module/3-is4.html - The skill of packaging a story file and associated resources into a blorb.
-   Chapter 4: Genre Management
    - [[Extension Manager|Extension Manager]]https://ganelson.github.io/inform/supervisor-module/4-em.html - Claiming and creating copies of the extension genre: used for Inform 7 extensions.
    - [[Kit Manager|Kit Manager]]https://ganelson.github.io/inform/supervisor-module/4-km.html - Claiming and creating copies of the kit genre: used for kits of precompiled Inter code.
    - [[Language Manager|Language Manager]]https://ganelson.github.io/inform/supervisor-module/4-lm.html - Claiming and creating copies of the language genre: used for bundles of natural language metadata in the Inform 7 compiler.
    - [[Pipeline Manager|Pipeline Manager]]https://ganelson.github.io/inform/supervisor-module/4-pm.html - Claiming and creating copies of the pipeline genre: used for pipelines of code-generation stages.
    - [[inform/Project Bundle Manager|Project Bundle Manager]]- Claiming and creating copies of the projectbundle genre: used for Inform 7 projects as created by the GUI apps.
    - [[inform/Project File Manager|Project File Manager]] - Claiming and creating copies of the projectfile genre: used for Inform 7 source texts stored as stand-alone plain text files, outside the GUI apps.
    - [[Template Manager|Template Manager]]https://ganelson.github.io/inform/supervisor-module/4-tm.html - Claiming and creating copies of the template genre: used for website and interpreter templates when releasing an Inform project.
-   Chapter 5: Genre Services
    - [[Extension Services|Extension Services]]https://ganelson.github.io/inform/supervisor-module/5-es.html - Behaviour specific to copies of the extension genre.
    - [[Kit Services|Kit Services]]https://ganelson.github.io/inform/supervisor-module/5-ks.html - Behaviour specific to copies of the kit genre.
    - [[Language Services|Language Services]]https://ganelson.github.io/inform/supervisor-module/5-ls.html - Behaviour specific to copies of the language genre.
    - [[Pipeline Services|Pipeline Services]]https://ganelson.github.io/inform/supervisor-module/5-ps.html - Behaviour specific to copies of the pipeline genre.
    - [[inform/Project Services|Project Services]] - Behaviour specific to copies of either the projectbundle or projectfile genres.
    - [[Template Services|Template Services]]https://ganelson.github.io/inform/supervisor-module/5-ts.html - Behaviour specific to copies of the template genre.
-   Chapter 6: Inform Source Text
    - [[inform/Source Text|Source Text]]- Using the lexer and syntax analysis modules to read in Inform 7 source text.
    - [[Headings|Headings]]https://ganelson.github.io/inform/supervisor-module/6-hdn.html - To keep track of the hierarchy of headings and subheadings found in the source text.
    - [[The Options File|The Options File]]https://ganelson.github.io/inform/supervisor-module/6-tof.html - The optional file of Options applied to all of the user's projects.
    - [[Inclusions|Inclusions]]https://ganelson.github.io/inform/supervisor-module/6-inc.html - To fulfill requests to include extensions, adding their material to the parse tree as needed, and removing INCLUDE nodes.
    - [[Control Structures|Control Structures]]https://ganelson.github.io/inform/supervisor-module/6-cs.html - To specify the syntax of control structures such as repeat, if and otherwise.
    - [[Virtual Machine Grammar|Virtual Machine Grammar]]https://ganelson.github.io/inform/supervisor-module/6-vmg.html - Grammar for parsing natural language descriptions of a virtual machine.
-   Chapter 7: Extension Indexing
    - [[The Mini-Website|The Mini-Website]]https://ganelson.github.io/inform/supervisor-module/7-tm.html - To refresh the mini-website of available extensions presented in the Inform GUI applications.
    - [[Dictionary|Dictionary]]https://ganelson.github.io/inform/supervisor-module/7-dct.html - To maintain a database of names and constructions in all extensions so far used by this installation of Inform, and spot potential namespace clashes.
    - [[Census|Census]]https://ganelson.github.io/inform/supervisor-module/7-cns.html - To conduct a census of all installed extensions installed.
    - [[Index Pages|Index Pages]]https://ganelson.github.io/inform/supervisor-module/7-ip.html - To generate the two top-level pages in the extension mini-website.
    - [[Individual Pages|Individual Pages]]https://ganelson.github.io/inform/supervisor-module/7-ip2.html - To generate the individual pages on extensions in the extension mini-website.
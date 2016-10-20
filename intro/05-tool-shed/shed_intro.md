# The Galaxy Tool Shed
intro to 'shed'

.footnote[\#usegalaxy / @galaxyproject]

---

## Please Interrupt!

We are here to answer your questions!

---

Tool Shed is to Galaxy as App Store is to iPhone (plus some more).

It is a free service that hosts repositories containing Galaxy Tools.

--

MTS runs at http://toolshed.g2.bx.psu.edu and serves all Galaxies worldwide.

Every repository is public including the whole history.

Local sheds can be run e.g. for private or custom-licensed tools.
---
## Vocabulary

* `wrapper` or `tool definition file` - The XML file that describes to Galaxy how the underlying software works, thus allowing Galaxy to render UI and execute the software in the right way.
--

* `repository` - A versioned code archive with tool(s) in Tool Shed. Mercurial is used.
--

* `revision` vs `installable revision` - Every TS repo update generates a new revision but only certain (reproducibility-affecting) changes generate a new revision installable to Galaxy.
--

* `metadata` - TS generates and stores a set of data for every installable revision of the repo.

---
## Galaxy's Configuration

List of available sheds is defined in `tool_sheds_conf.xml` and Galaxy comes with the Main Tool Shed enabled.
```
<?xml version="1.0"?>
<tool_sheds>
    <tool_shed name="Galaxy Main Tool Shed" url="https://toolshed.g2.bx.psu.edu/"/>
<!-- Test Tool Shed should be used only for testing purposes.
    <tool_shed name="Galaxy Test Tool Shed" url="https://testtoolshed.g2.bx.psu.edu/"/>
-->
</tool_sheds>
```
---
## Overview

* Tool Shed is a host (not a development) platform.
??
* Tool Development repository should be linked from the TS repository.
--

* Tool Shed allows administrators to pick any installable revision
--

* Multiple installable revisions of any repository can be present in Galaxy


---

## Dependency Handling



---



---
---
title: Building the HMT editing environment locally
---

(rough notes)

## Basics

-   git:  <https://git-scm.com/>
-   bash shell.  Built in if you are on a POSIX system like OS X, Linux or UNIX.  If on a Windows operating system, you can use the bash shell that is installed with git.


## Editing with Atom


### Overview

1.  Install atom from <https://atom.io/>.  If on OS X, open atom and choose from the Atom menu, "Install Shell Commands"
2.  Install atom packages used in HMT editing for XML and delimited text files.
3.  Configure TEI validation using `atomic-tei`.


### Details

**Installing atom packages**.  From a bash shell, use the atom package manager `apm` to install the following packages:


    apm install intentions
    apm install busy-signal
    apm install linter
    apm install linter-ui-default
    apm install linter-autocomplete-jing
    apm install atom-xsltransform
    apm install tablr
    apm install xml-formatter


Download (from somewhere...  temporarily here: <https://raw.githubusercontent.com/homermultitext/editors-vm/summer2017/system/atom-tablr-conf.cson> ) the file `atom-tablr-conf.cson`, and

    cp atom-tablr-conf.cson $HOME/.atom/config.cson


**Installing plugin for TEI validation**.

1.  Clone or download the `atomic-tei` github repository at <https://github.com/neelsmith/atomic-tei>
2.  In a bash shell, `cd` into the cloned/downloaded repository, and run `apm link`



## Validation with MOM

For partial validation (used in 2017 summer seminar):

-   java.  You need a full Java SDK (software development kit).  With luck, you can find that at <http://www.oracle.com/technetwork/java/javase/downloads/index.html>
-   scala. <http://www.scala-lang.org/>.  (OS X users: make sure `scala/bin` is on your CLASSPATH.)
-   sbt. <http://www.scala-sbt.org/>  (OS X users: make sure `sbt/bin` is on your CLASSPATH.)

To add morphological validation:

-   SFST: <http://www.cis.uni-muenchen.de/~schmid/tools/SFST/>

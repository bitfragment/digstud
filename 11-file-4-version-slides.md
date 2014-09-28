![150%](http://www.quorumcentral.com/layout/images/tour_doc_icon6.png)

^
* File: document, program... now version
* Common to both document composition, software programming
* You're familiar with multiple drafts: first, second, third

----

![150%](http://www.bbc.co.uk/accessibility/images/guides/which_system/which_os_mac_fig1.jpg)

^
* You're familiar with software version numbering too

----

        engl401paper.doc

        engl401paper-revision.doc

^
* I bet some of you do primitive, ad-hoc version control

----


        engl401paper-version1.doc

        engl401paper-version2.doc

----

![fit](http://micahcapstone.files.wordpress.com/2010/07/001.jpg)

^
* Before book printing, scribes copied manuscripts by hand for distribution
* Tried to make each copy identical, but hand-copying → inevitable variation
* Scholarship studying mss. → concept of ms. *variant*

----

![fit](http://nzetc.victoria.ac.nz/etexts/Har04Typo/Har04Typo178.jpg)

^ 
* Printed books: able to print identical copies
* But corrections of errors; revisions and updates
* → concept of printed *edition*
* First edition (collectors collect them), second, revised, etc.

----

![175%](http://www.gapsystems.net/wp-content/uploads/version-control-lrg.png)

^ 
* Software programmers: very sophisticated concept of *version* of program
* Beginning at "version 1"

----

![fit](http://www.cs.colorado.edu/~kena/classes/3308/f06/lectures/12/version-numbering.png)

^
* ...and developing in what are called branches from a trunk

----

![fit](http://redstack.files.wordpress.com/2013/05/version-control.png)

^ 
* Just like a tree

----

![fit](http://www.zipgenius.com/wp-content/uploads/2014/07/current_versioning.png)

^
* Sophisticated schema
* [Explain]

----

![fit](https://www.linode.com/docs/assets/1204-image_versioning_intro_1.jpg)

^ 
* Software development management software: version control

----

![fit](http://wiki.bizagi.com/en/images/0/0d/BizagiWiki_Home_Image019.jpg)

^
* Software version control → incorporated back into document prep
* Wiki: have you tried one
* [Demo with a Wikipedia page]

----

![125%](http://blog.codinghorror.com/content/images/uploads/2009/02/6a0120a85dcdae970b012877707d6a970c-pi.gif)

^
* Both software dev and wiki editing: multiple authors
* VCS allow that without confusion
* Doc edited by multiple authors in multiple revisions

----

![fit](https://www.research.ibm.com/visual/projects/history_flow/images/calculus1.gif)

^
* IBM History Flow project, Wikipedia edits
* Here, "Calculus"
* [Open page and look at history]

----

![fit](https://www.research.ibm.com/visual/projects/history_flow/images/calculus2.gif)

^
Another view of "Calculus"

----

![fit](http://cdn1.mos.techradar.futurecdn.net//Review%20images/PC%20Plus/PCP%20300/PCP300.helpdesk.document_comparison-580-90.jpg)

^
* Fundamental to concept of *version* is concept of *comparison*
* Version requires comparison to be meaningful

----

![fit](http://www.teilin.net/content/images/2014/Jul/difftoolvs.png)

^
* Comparison tools developed in pre-GUI CLI era

----

## [fit] `diff` (1970s)

^
* File comparison utility to show changes between two versions of a text file
* [Create file1, file1, write poem, change 1 word]
* [Run diff, diff -c, diff -u, diff -y]
* Line in file 1 / code / Line in file 2
* "a": added, "d": deleted, "c": changed

----

## [fit] GUI `diff` utilities

^
[ksdiff the two files]

----

## [fit] `patch` (1970s)

^
* File updating utility that uses output of diff
* Used to update software using emailed patches
* [diff -u > differences.diff]
* [open and look at differences.diff]
* [patch < differences.diff]

----

## [fit] History of version control systems

----

## History of version control systems

Three generations, 1970s-2000s

----

## History of version control systems

### First generation

* Source Code Control System (SCCS), 1972
* Revision Control System (RCS), 1982
* Concurrent Versions System (CVS), 1990

^
* Before Internet
* Designed for use on a single machine
* After 1994, CVS modified for network usage

----

## History of version control systems

### Second generation

* Subversion (SVN), 2004

^
* [Logo is on next slide]

----

![fit](http://aragost.com/static/subversion.png)

^
* Widely adopted in place of CVS

----

## History of version control systems

### Third generation

* BitKeeper (BK), early 2000s

^
[Logo is on next slide]

----

![175%](http://open-tube.com/wp-content/uploads/2009/03/bitkeeper.png)

^
BK adopted by Linus Torvalds for Linux kernel

----

## History of version control systems

### Third generation

* Git (2005)

^
[Logo is on next slide]

----

![100%](http://git-scm.com/images/logos/downloads/Git-Logo-2Color.png)

^
Git designed by Linus Torvalds as a non-proprietary alternative to BitKeeper

----

![800%](http://2.bp.blogspot.com/-Yqd0z4K94B0/TfSS8OXf89I/AAAAAAAABJA/fGLt-N9ti2s/s200/bazaar.png)

^
* Other 3G VCS include Bazaar...
* [Flip back] Notice the trunk-branch imagery in product logos

----

![200%](http://www.selenic.com/hg-logo/logo-droplets-200.png)

^
Mercurial...

----

![fit](http://upload.wikimedia.org/wikipedia/commons/thumb/c/c6/Fossil_SCM_logo.svg/745px-Fossil_SCM_logo.svg.png)

^
Fossil...

----

![200%](http://darcs.net/releases/branch-2.3/doc/logos/plain_logo.png)

^
DARCS.

----

## [fit] Three important capabilities of a VCS (Raymond)

----

## Three important capabilities of a VCS (Raymond)

1. Reversibility
2. Concurrency
3. Annotation

----

![fit](https://www.udemy.com/blog/wp-content/uploads/2014/05/shutterstock_123711823-300x366.jpg)

^
* Reversibility
* All VCSs include sophisticated "undo" features
* Since you have a complete record of versions...
* You can revert, or go back to any previous version whenever you need to

----

![fit](https://www.dropbox.com/s/s3v5y3syqnqfh6q/iscp_icon_collaborative_editing_process.png?dl=1)

^
* Concurrency
* Multiple authors working simultaneously
* Ability to reconcile all those separate changes

----

![fit](http://i.stack.imgur.com/BZKMh.jpg)

^
* Annotation
* Automated record-keeping of history of changes

----

## [fit] Elements of a version control system

----

## Elements of a version control system

1. Repository
1. Master copy
1. Working copy “checked out” (copied) for work
1. Change history

----

![fit](http://upload.wikimedia.org/wikipedia/commons/c/ce/Documents_stacks_in_a_repository_at_The_National_Archives.jpg)

^
* Repository
* Concept adopted from domain of paper documents: National Archives

----

![200%,inline,left](http://upload.wikimedia.org/wikipedia/commons/c/ce/Documents_stacks_in_a_repository_at_The_National_Archives.jpg)![inline,right](http://www.computerworld.in/sites/default/files/feature/2012/05/hp-a-big-data-394.jpg)

^
* Data structure representing a storage space

----

![fit](http://www.medcomsoft.com/wp-content/uploads/slide026_r.jpg)

^
* A storage space shared by multiple machines operated by multiple writers or software developers

----

## [fit] Elements of a VCS repository

----

## Elements of a VCS repository

1. Files and directories
2. Descriptions of changes to files and directories
3. Data objects representing changes to files and directories

----

## [fit] Branching

----

<!-- trunk with branches -->
![fit](http://img2.wikia.nocookie.net/__cb20111205043919/runescape/images/0/0b/Willow_branch_detail.png)

^
* Essential feature: branching
* Uses metaphor taken from form of most trees
* ?(How many trunks?)
* ?(How many branches?)
* ?(Difference between trunk and branch)

----

![fit](http://1.bp.blogspot.com/-cUACFjdQAhk/UC0x4WbN2tI/AAAAAAAABUM/doO1eVIklZY/s1600/LivingCodeBase.png)

^
* Think of the series of major versions (1.0...) as a trunk
* Software you actually release
* Branches for experimental feature
* Documents too: experimental extra paragraph
* Your VCS keeps track of versions along both paths

----

![fit](http://rogerdudler.github.io/git-guide/img/branches.png)

^
Later, you can merge if you want, or not

----

![fit](http://www.clipartoday.com/_thumbs/069/batch_01/autumnleaves1-trina_branch1_tnb.png)

^
* Branches will always be “smaller” than the trunk
* May or may not become structurally significant
* Some branches grow large
* Others remain small

<!-- 
![fit](http://redstack.files.wordpress.com/2013/05/version-control.png)

^
* What enables a VCS to keep track of different development paths?
* Version IDs, usually numerical

----

![fit](http://upload.wikimedia.org/wikipedia/commons/thumb/0/00/VersionNumbers.svg/192px-VersionNumbers.svg.png)

----

![fit](http://upload.wikimedia.org/wikipedia/commons/thumb/0/07/Software_dev2.svg/484px-Software_dev2.svg.png)

----

![fit](http://i.stack.imgur.com/aoN7v.png) -->

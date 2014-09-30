---
title:        'File: Version'
subtitle:     
version:      $version$
embed-vcs:    true
date:         $date$
description:  Course notes on the 'file' subtopic 'version'
published:    true
license:      > 
              This work is licensed under a Creative Commons 
              Attribution-NonCommercial-ShareAlike 4.0 International License.
url:          
note:         
author:       Brian Lennon
email:        blennon@cesgnalintelligence.net
affiliation:  | 
              | Departments of English and Comparative Literature
              | Pennsylvania State University
              | University Park, PA 16801 USA
id_:          '$Id$'    # git
archive_:     '$Format:%h %ci$' # 'git archive'
project:      digstud
category:     notes
subcategory:  teaching
tags:         # [tag1, tag2] for Pandoc
created:      2014-06-23
layout:       page # for Jekyll
bibliography: /Users/blennon/sync/lib/bib/dummy.bib
biblio-title: 'Works Cited' # for Pandoc
csl:          /Users/blennon/sync/lib/csl/modern-language-association.csl
css:          # filepath
Marked CSS:   # filepath
Marked Style: # style sheet
Custom Preprocessor: false # Marked.app
abstract:     
---

* toc
{:toc}

## Readings

{% bibliography --file 11-file-4-version %}



## What is a version?

* A concept common to both literary composition and software programmers
* Philology and literary studies developed the concepts of manuscript *variant* and printed *edition*
* Software programmers have developed especially sophisticated *version control* or *revision control* concepts, utilities, and workflows
* These have been incorporated into software for producing new kinds of documents, such as wiki software
    - Wikipedia: [Revision history page for article "Wiki"](http://en.wikipedia.org/w/index.php?title=Wiki&action=history)
    - [Sample visualization](http://blog.codinghorror.com/content/images/uploads/2009/02/6a0120a85dcdae970b012877707d6a970c-pi.gif) of a wiki page edited by three different people at different points in time
* IBM [History Flow](https://www.research.ibm.com/visual/projects/history_flow/index.htm) project, ca. 2004
    - Visual representation of time-series of versions of a document
        + Wikipedia
            * [Calculus](https://www.research.ibm.com/visual/projects/history_flow/images/calculus1.gif) (by versions)
            * [Calculus](https://www.research.ibm.com/visual/projects/history_flow/images/calculus2.gif) (by date)



## Everyday ad-hoc version control: file naming

### For example:

        engl401paper.doc
        engl401paper-revision.doc


### For example:

        engl401paper-version1.doc
        engl401paper-version2.doc



File comparison, `diff`, and `patch`
------------------------------------

* Review text editor and word processor, in [File: Document]({{site.baseurl/11-file-2-document/}})
* [File comparison](http://en.wikipedia.org/wiki/File_comparison)
    - Comparison of text files (documents or programs)
* [diff](http://en.wikipedia.org/wiki/Diff), early 1970s
    - Unix file comparison utility to show changes between two versions of a text file
* [patch](http://en.wikipedia.org/wiki/Patch_(computing))
    - Unix file updating utility that uses output of `diff`



`diff`
------

### `file1`:

        This is a poem
        about a bear
        who got lost
        in State College
        and ate a dog.

### `file2`:

        This is a poem
        about a bear 
        who got lost
        in State College
        and ate a professor.

### Output of `diff file1 file2`

        5c5
        < and ate a dog.
        ---
        > and ate a professor.

### Output of `diff -c file1 file2`

        *** file1   2014-09-28 12:29:40.000000000 -0400
        --- file2   2014-09-28 12:29:51.000000000 -0400
        ***************
        *** 2,5 ****
          about a bear
          who got lost
          in State College
        ! and ate a dog.
        --- 2,5 ----
          about a bear
          who got lost
          in State College
        ! and ate a professor.

### Output of `diff -y file1 file2`

        This is a poem                   This is a poem
        about a bear                     about a bear
        who got lost                     who got lost
        in State College                 in State College
        and ate a dog.                 | and ate a professor.


### Using a GUI application

![diff in Kaleidoscope.app]({{site.baseurl}}/public/images/diff-kaleidoscope.png)

* [HTML example](http://phatness.com/wp-content/uploads/2011/01/Screen-shot-2011-01-12-at-1.06.26-PM.png) using Kaleidoscope.app
* [Prose example](https://raw.githubusercontent.com/caseyg/bylaws/master/img/kaleidoscope-screenshot.png) using Kaleidoscope.app




`patch`
-------

### Output of `diff -u file1 file2`

        --- file1   2014-09-28 12:29:40.000000000 -0400
        +++ file2   2014-09-28 12:29:51.000000000 -0400
        @@ -2,4 +2,4 @@
         about a bear
         who got lost
         in State College
        -and ate a dog.
        +and ate a professor.

### Patching `file1`

`file2` is a newer, "updated" version of the poem. We want everyone we know to update the older version of the poem (in `file1`) to the new version. So we distribute the output of `diff` (with the `-u` flag) as a "patch file" named `bear-poem-update`:

        $ diff -u file1 file2 > bear-poem-update.diff

Individual users can then use the `patch` utility to update their copies of the poem using the patch file `bear-poem-update`:

        $ patch < bear-poem-update.diff
        patching file file1

`file1` has now been updated to contain the new version of the poem:

        $ cat file1
        This is a poem
        about a bear
        who got lost
        in State College
        and ate a professor.



## Version control concepts

Three important capabilities  {% cite raymond_understanding_2008 --file 11-file-4-version %}:

1. **Reversibility**: "the ability to back up to a saved, known-good state when you discover that some modification you did was a mistake or a bad idea"
    * Sophisticated "undo" features
    * You have a complete record of versions, so you can *revert*, or go back to any previous version whenever you need to

1. **Concurrency**: "the ability to have many people modifying the same collection of code or documents knowing that conflicting modifications can be detected and resolved"
1. **Annotation**: the ability to attach "explanatory comments about the intention behind each change to it and a record of who was responsible for each change"

 

## Elements of a version control system

1. Repository
    * A concept borrowed from the domain of paper documents
    * Data structure representing a storage space
    * Elements of a version control repository
        + Files and directories
        + Descriptions of changes to files and directories
        + Data objects representing changes to files and directories
1. Master copy
1. Working copy "checked out" (copied) for work
1. Change history



## Change history and branching

* Tree structure: trunk and branch
* Trunk
    - Like the trunk of a tree
    - Series of authoritative versions
        + Versions of software actually released
* Branch
    - Like the branch of a tree
    - Will always be "smaller" than the trunk
    - May or may not become structurally significant
        + Some branches grow large
        + Others remain small



## History of version control systems

### Centralized first generation systems

* Centralized architectures
    - Before Internet
    - Designed for use on a single machine

* Source Code Control System (SCCS), 1972
* Revision Control System (RCS), 1982
    - Individual files only
    - Local only
* Concurrent Versions System (CVS), 1990
    - Groups of files simultaneously
    - Centralized client-server architecture: a single master repository retains master copies, serves and receives working copies
    - After 1994, modified to accommodate networked (Internet) usage

### Centralized second generation systems

* Subversion (SVN), 2004
    - Was widely adopted in place of CVS
    - Last widely adopted centralized VCS

### Decentralized third generation systems

* Decentralized architectures
    - Each developer can work independently on a complete *copy* of the "master" repository for a project
    - Branching and merging changes is generally easier than in centralized systems

* BitKeeper (BK), early 2000s
    - Adopted by Linus Torvalds for development of Linux kernel
    - Unlike most other VCSs, proprietary (rather than "open source") software
* Git (2005)
    - Designed by Linus Torvalds as a non-proprietary alternative to BitKeeper



## Version ID numbering

* SCCS style: 1.1 = major version + "." + minor version
* Many other variations, but `major.minor` is very popular
* Apple OS X
    - Major versions: `10.0` ("Cheetah") ... `10.10` ("Yosemite")
    - Minor versions: `10.9.0` ("Mavericks") ... `10.9.5` ("Mavericks," version 5)
* Microsoft Windows
    - Major versions using `major.minor`: `1.0` ... `3.0` (1981-1992)
    - Major individual consumer versions using dates: `95`, `98`, `ME` (Millennium) (1995-2000)
    - Major versions using brand names: `XP`, `Vista` (2001-2006)
    - Major versions using `major.minor`: `7.0`, `8.0` (2009-)



## Software release lifecycle

1. "Alpha" and "beta" versions
    - Preliminary versions for testing purposes only, not full release or "shipping"
    - Borrowed from Greek alphabet: Α α alpha, Β β beta
    - Best Buy "beta tested" ad campaign [example](http://www.ispot.tv/ad/72AT/best-buy-blue-shirt-beta-test-verizon-htc-one)
2. Sequence of released versions
3. End of life stage: no further development or support
    - Deliberately discontinued
    - Abandoned ("abandonware")



## Version control with RCS

We are going to edit the poem, changing the line "ate a dog" to "ate a professor" and using RCS to keep track of that change.

First, we "check in" the file to beging tracking its versions:

        $ ci file1
        file1,v  <--  file1
        enter description, terminated with single '.' or end of file:
        NOTE: This is NOT the log message!
        >> Poem about bear.
        initial revision: 1.1
        done

RCS asks us for a description of the file. Notice also that RCS automatically provides our first version number, `1.1`.

This creates a file named `file1,v` (the `v` marks it as a version control file). Here's what that file looks like:

        head    1.1;
        access;
        symbols;
        locks; strict;
        comment @# @;

        1.1
        date    2014.09.28.17.00.25;    author blennon; state Exp;
        branches;
        next    ;

        desc
        @Poem about bear.
        @

        1.1
        log
        @Initial revision
        @
        text
        @This is a poem
        about a bear
        who got lost
        in downtown State College
        and ate a dog.
        @

Now we "check out" a working copy of the file so we can edit it.

        $ co -l file1

We open an editor and change the line "ate a dog" to "ate a professor." Then we check the file back in, this time providing a description of the change we made:

        $ ci file1
        file1,v  <--  file1
        new revision: 1.2; previous revision: 1.1
        enter log message, terminated with single '.' or end of file:
        >> Change "ate a dog" to "ate a professor"
        done

Notice also that RCS automatically increments our version number from `1.1` to `1.2`. Here's what the file `file1,v` looks like now:

        head    1.2;
        access;
        symbols;
        locks; strict;
        comment @# @;

        1.2
        date    2014.09.28.17.01.49;    author blennon; state Exp;
        branches;
        next    1.1;

        1.1
        date    2014.09.28.17.00.25;    author blennon; state Exp;
        branches;
        next    ;

        desc
        @Poem about bear.
        @

        1.2
        log
        @Change "ate a dog" to "ate a professor"
        @
        text
        @This is a poem
        about a bear
        who got lost
        in downtown State College
        and ate a professor.
        @

        1.1
        log
        @Initial revision
        @
        text
        @d5 1
        a5 1
        and ate a dog.
        @

We can also look at the log (history) of versions and changes made to the file:

        $ rlog file1

        RCS file: file1,v
        Working file: file1
        head: 1.2
        branch:
        locks: strict
        access list:
        symbolic names:
        keyword substitution: kv
        total revisions: 2; selected revisions: 2
        description:
        Poem about bear.
        ----------------------------
        revision 1.2
        date: 2014/09/28 17:01:49;  author: blennon;  state: Exp;  lines: +1 -1
        Change "ate a dog" to "ate a professor"
        ----------------------------
        revision 1.1
        date: 2014/09/28 17:00:25;  author: blennon;  state: Exp;
        Initial revision

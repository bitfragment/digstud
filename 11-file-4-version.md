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



Readings
--------

{% bibliography --file 11-file-4-version %}



What is a version?
------------------

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



Everyday ad-hoc version control: file naming
--------------------------------------------

### For example:

        engl401paper.doc
        engl401paper-revision.doc


### For example:

        engl401paper-version1.doc
        engl401paper-version2.doc



Version control topics and concepts
-----------------------------------

* Review text editor and word processor, in [File: Document]({{site.baseurl/11-file-2-document/}})
* [File comparison](http://en.wikipedia.org/wiki/File_comparison)
    - Comparison of text files (documents or programs)
* [diff](http://en.wikipedia.org/wiki/Diff), early 1970s
    - Unix file comparison utility to show changes between two versions of a text file
* [patch](http://en.wikipedia.org/wiki/Patch_(computing))
    - Unix file updating utility that uses output of `diff`
* Three important capabilities  {% cite raymond_understanding_2008 --file 11-file-4-version %}
*   <http://www.catb.org/esr/writings/version-control/version-control.html>
    1. Reversibility
    2. Concurrency
    3. Annotation



diff
----

### file1:

        This is a text file. 
        It contains some text.

### file2:

        This is a text file. 
        It contains quite a bit of text.

        Text text text text text 
        text text text text text text!

### Output of `diff file1 file2`

        2c2,5
        < It contains some text.
        ---
        > It contains quite a bit of text.
        > 
        > Text text text text text 
        > text text text text text text!

### Output of `diff -y file1 file2`

        This is a text file.              This is a text file. 
        It contains some text.            | It contains quite a bit of text.
                                          >
                                          > Text text text text text 
                                          > text text text text text text!

* [HTML example](http://phatness.com/wp-content/uploads/2011/01/Screen-shot-2011-01-12-at-1.06.26-PM.png) using Kaleidoscope.app
* [Prose example](https://raw.githubusercontent.com/caseyg/bylaws/master/img/kaleidoscope-screenshot.png) using Kaleidoscope.app




patch
-----

### Output of `diff -u file1 file2`

        --- file1  2014-09-23 16:13:00.000000000 -0400
        +++ file2 2014-09-23 16:13:14.000000000 -0400
        @@ -1,2 +1,5 @@
         This is a text file. 
        -It contains some text.
        +It contains quite a bit of text.
        +
        +Text text text text text 
        +text text text text text text!

### Patching `file1`

        $ diff -u file1 file2 > diff_output.diff
        $ patch < diff_output.diff
        patching file file1



History of revision control systems
-----------------------------------

<http://en.wikipedia.org/wiki/Revision_control>

* Source Code Control System (SCCS), 1972


<!-- software dev cycle: alpha, beta, version numbering -->
<!-- demo vc in ms word -->
<!-- demo using git -->

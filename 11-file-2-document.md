---
title:        "File: Document"
subtitle:     
version:      $version$
embed-vcs:    true
date:         $date$
description:  "Course notes on the topic file: document"
published:    true
license:      > 
              This work is licensed under a Creative Commons 
              Attribution-NonCommercial-ShareAlike 4.0 International License.
url:          
note:         
author:       $author$ # git
email:        $email$  # git
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
created:      2014-06-24
layout:       page # for Jekyll
bibliography: /Users/blennon/sync/digstud/11-file-2-document.bib
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

{% bibliography --file 11-file-2-document %}



## File as document

* A digital file meets the most basic definition of *document*: a written representation
* In consumer computing, a document usually describes a file containing text data



## Plain text

* `DO`: Review character display and character encoding, in [Bit]({{site.baseurl/10-bit/}})
* [Plain text](http://en.wikipedia.org/wiki/Plain_text): content with (what is ostensibly) a minimum of form
    - [Command line interface](http://en.wikipedia.org/wiki/Command-line_interface) vs. [graphical user interface](http://en.wikipedia.org/wiki/Graphical_user_interface)
        - [Javascript PC Emulator](http://bellard.org/jslinux/)
    - [DarkCopy: Simple, full screen text editing](http://darkcopy.com/)
    - [Writer: the internet typewriter](https://writer.bighugelabs.com/)
* Plain text with [markup](http://en.wikipedia.org/wiki/Markup_language)
* Content and form are combined, yet distinguishable
    


## Formatted or "rich" or "styled" text

* [WYSIWYG](http://en.wikipedia.org/wiki/WYSIWYG)
* Markup is hidden
* Content and form are combined, but not easily distinguished



## Text editors vs. word processors

* Text editors
    * `ed` in [Javascript PC Emulator](http://bellard.org/jslinux/)
    * `vi` and `emacs` in [Javascript PC Emulator](http://bellard.org/jslinux/)
    * Emacs
        * [Ymacs demo](http://www.ymacs.org/demo/)
    * vi, vim
        * [jsvi](http://gpl.internetconnection.net/vi/)
* Desktop word processors
    - Plain text interfaces (before 1984-1985)
        + MS-DOS operating system, 1981
        - Plain text with formatting characters added to text and visible to user
            - Electric Pencil, 1976: [illustration](http://www.trs-80.org/electric-pencil/)
            - WordStar, 1978
            - WordPerfect, 1980
            - Microsoft Word, 1983
    - Graphical user interfaces
        + Mac OS operating system, 1984
        + Microsoft Windows operating system, 1985
        - Rich text with formatting codes added to text and hidden from user
        - WordPerfect "reveal codes" feature
        - WYSIWYG: screen display mimics, and produces, printed document
            + [Ted Nelson Google Tech Talk, 4:15](http://www.youtube.com/watch?v=ohiKTVVtDJA): "simulations of paper under glass"



## Markup

* Processing markup
    - Producing printed or printable documents
* Semantic markup
    - Describing the structure of documents
* Presentation markup
    - Presenting documents on a screen



## Markup history: typesetting

* [Designers Insights](http://www.designersinsights.com/wp-content/uploads/2012/03/Big-Type-Capitals.png)
* [Handwritten typesetting markup (Dennis G. Watson, Brief History of Document Markup)](http://www.technical-expressions.com/layout/markup/images/Typesetting-markup-eg50.gif)
* [Handwritten typesetting markup (Mark Simonson)](http://www.marksimonson.com/assets/content/notebook/markup001.jpg)
* [Handwritten typesetting markup (Janet Giampietro)](http://www.j-giampietro.com/blog/wp-content/uploads/2010/02/gblog_manuscript_markup.jpg)



## Markup history: text processing

* `roff`-type utilities
    - `TYPSET` and `RUNOFF` on MIT Compatible Time-Sharing System (CTSS), 1964
    - `runoff` on MIT Multiplexed Information and Computing Service (Multics), after 1964
    - `roff` on Bell Labs UNiplexed Information and Computing Service (UNICS, then UNIX/Unix), after 1970
    - `nroff` ("new `roff`") on Unix, after 1973, for line printers and terminals
    - `troff` ("typesetter `roff`") on Unix, after 1973, for phototypesetters
        * Unix Seventh Edition Manual (Bell Labs)
            * [troff source](http://cm.bell-labs.com/7thEdMan/vol1/man0.bun)
            * [PDF](http://cm.bell-labs.com/7thEdMan/v7vol1.pdf)
        * [A dictionary of troff commands](http://www.lemoda.net/unix/troff-dictionary/index.html)
* TeX (1978) and LaTeX (1984)
    - Designed for typesetting mathematics, among other functions
    - [writeLaTeX](https://www.writelatex.com)



## Markup history: semantics

* IBM Generalized Markup Language (GML) {% cite goldfarb_roots_1996 --file 11-file-2-document %}

        :h1.Chapter 1:  Introduction
        :p.GML supported hierarchical containers, such as
        :ol
        :li.Ordered lists (like this one),
        :li.Unordered lists, and
        :li.Definition lists
        :eol.
        as well as simple structures.
        :p.Markup minimization (later generalized and formalized in SGML),
        allowed the end-tags to be omitted for the "h1" and "p" elements.

* SGML (Standard Generalized Markup Language)

        <h1>Chapter 1: Introduction</h1>
        <p>GML supported hierarchical containers, such as
        <ol>
        <li>Ordered lists (like this one),
        <li>Unordered lists, and
        <li>Definition lists
        </ol>
        as well as simple structures.
        <p>Markup minimization (later generalized and formalized in SGML),
        allowed the end-tags to be omitted for the "h1" and "p" elements.



## Markup history: text presentation

* HTML (HyperText Markup Language)

        <h1>Chapter 1: Introduction</h1>
        <p>GML supported hierarchical containers, such as
        <ol>
        <li>Ordered lists (like this one),
        <li>Unordered lists, and
        <li>Definition lists
        </ol>
        as well as simple structures.
        <p>Markup minimization (later generalized and formalized in SGML),
        allowed the end-tags to be omitted for the "h1" and "p" elements.

* "…many desktop publishing methods were in vogue: SGML, Interleaf, LaTeX, Microsoft Word, and Troff among many others. Commercial hypertext packages were computer-specific and could not easily take text from other sources; besides, they were far too complicated and involved tedious compiling of text into internal formats to create the final hypertext system… What was needed was something very simple, at least in the beginning" {% cite raggett_history_1998 --file 11-file-2-document %}
* "The HTML that Tim [Berners-Lee] invented was strongly based on SGML (Standard Generalized Mark-up Language), an internationally agreed upon method for marking up text into structural units such as paragraphs, headings, list items and so on… What SGML does not include, of course, are hypertext links: the idea of using the anchor element with the HREF attribute was purely Tim [Berners-Lee]'s invention" {% cite raggett_history_1998 --file 11-file-2-document %}
* [View HTML source of this page](view-source:data.html)
* [Tryit Editor v2.0](http://www.w3schools.com/html/tryit.asp?filename=tryhtml_basic)



## The front-end Web development "stack"

* HTML + CSS
    - [CSSDesk - Online CSS Sandbox](http://www.cssdesk.com/)
* HTML + CSS + JavaScript
    - JavaScript in browser
    - [Dabblet](http://dabblet.com)
* Client-side (browser) vs. server-side
* PHP (server-side)
    - [Execute PHP Script Online](http://www.compileonline.com/execute_php_online.php)



## Standardization and its discontents

* XML
    * <q>Although it took off like wildfire, HTML is where things began to go horribly wrong</q> [@anderson_introducing_2004]
    * [Sample XML document (Microsoft Developer Network)](http://msdn.microsoft.com/en-us/library/ms762271(v=vs.85).aspx)
* XHTML
* HTML 5
* Markdown
    * [Markdown processors online]
    * [Markdown editors: Stackedit, Dillinger.io, Markable.in]

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


[Slide version](11-file-2-document-slides-revealjs.html)

Readings
--------

{% bibliography --file 11-file-2-document %}


## File as document

* A digital file meets the basic definition of *document*



## Plain text

* Review text encoding
* Plain text: content "only"
    - CLI interface: [Javascript PC Emulator](http://bellard.org/jslinux/)
    - http://darkcopy.com
    - https://writer.bighugelabs.com
* Plain text with markup
* Content *and* form
* Content and form co-present but easily distinguished
    


## Formatted or "rich" or "styled" text

* WYSIWYG
* "Invisible" markup
* Content and form co-present but not easily distinguished



## Text editors vs word processors

* ed in [Javascript PC Emulator](http://bellard.org/jslinux/)
* vi and emacs in [Javascript PC Emulator](http://bellard.org/jslinux/)
* Emacs
    * Ymacs: http://www.ymacs.org/demo/
* vi, vim
    * jsvi: http://gpl.internetconnection.net/vi/
* Word processors [illustrations/emulators]
    - History to 1976
    - Electric Pencil
        + Illustrations: http://www.trs-80.org/electric-pencil/
    - WordStar
    - WordPerfect
    - Microsoft Word


## Markup

* Processing markup
* Semantic markup
* Presentation markup



## Markup: HTML

* Presentation markup
* `DO`: plain text file with HTML, rendered by browser



## Markup history: typesetting

* [Designers Insights](http://www.designersinsights.com/wp-content/uploads/2012/03/Big-Type-Capitals.png)
* [Handwritten typesetting markup (Dennis G. Watson, Brief History of Document Markup)](http://www.technical-expressions.com/layout/markup/images/Typesetting-markup-eg50.gif)
* [Handwritten typesetting markup (Mark Simonson)](http://www.marksimonson.com/assets/content/notebook/markup001.jpg)
* [Handwritten typesetting markup (Janet Giampietro)](http://www.j-giampietro.com/blog/wp-content/uploads/2010/02/gblog_manuscript_markup.jpg)



## Markup history: text processing

* Unix Seventh Edition Manual (Bell Labs)
    * [troff source](http://cm.bell-labs.com/7thEdMan/vol1/man0.bun)
    * [PDF](http://cm.bell-labs.com/7thEdMan/v7vol1.pdf)
* [A dictionary of troff commands](http://www.lemoda.net/unix/troff-dictionary/index.html)
* LaTeX
    + [writeLaTeX](https://www.writelatex.com)



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

* "…many desktop publishing methods were in vogue: SGML, Interleaf, LaTex, Microsoft Word, and Troff among many others. Commercial hypertext packages were computer-specific and could not easily take text from other sources; besides, they were far too complicated and involved tedious compiling of text into internal formats to create the final hypertext system… What was needed was something very simple, at least in the beginning" {% cite raggett_history_1998 --file 11-file-2-document %}
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



* markup history from previous notes: working on markup3
* markdown processor online
* markdown editors: stackedit, dillinger.io, markable.in

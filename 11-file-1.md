---
title:        File
subtitle:     
version:      $version$
embed-vcs:    true
date:         $date$
description:  Course notes on the topic "file"
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
bibliography: /Users/blennon/sync/digstud/11-file-1.bib
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


[Slide version](11-file-1-slides-revealjs.html)

Readings
--------

{% bibliography --file 11-file-1 %}


## File as abstraction

* *File* is another layer of abstraction on top of *byte* and *word*
* In memory addressing, *word* and *word size* are adapted from the domain of natural (human) language
* *File* is adapted from the domain of paper documents
* A linear array (indexed sequence) of bytes stored on a durable medium



## File contents: data

* Illustration: [viewing a file with a hex viewer](http://upload.wikimedia.org/wikipedia/commons/2/2c/Hexedit-screenshot.png)
* Center columns: sixteen two-digit hex numbers arranged in four groups of four columns each
    - Each two-digit hex number represents a byte
    - Here, the code for an ASCII character
    - `DO`: Enter the first two-digit hex number into the hexadecimal text field at [ASCII to Hex - Free text conversion tools](http://www.asciitohex.com/)
* Rightmost column: ASCII characters
* Leftmost column: hexadecimal memory address of the first byte in the row
    - `DO`: Enter the first hexadecimal memory address into the hexadecimal text field at [ASCII to Hex - Free text conversion tools](http://www.asciitohex.com/)
    - Hex `00000000` = decimal `0`
    - Hex `00000010` = decimal `16`
* `DO`: [Javascript PC Emulator](http://bellard.org/jslinux/)

        # mkdir temp
        # cd temp
        # echo "Foo, bar, foobarbarous" > foo.txt
        # hexdump foo.txt
        # hexdump -C foo.txt
        # xxd -b foo.txt

(If Javascript PC Emulator provided the utility `xxd`, this final command would display output in bits: that is, in binary notation)


## File as container of data

* The OS represents memory storage in durable media in (*pages* and) *blocks*
* The OS keeps track of blocks via a [page table](http://en.wikipedia.org/wiki/Page_table)
* If it is larger than the size of one block, a file may be distributed over more than one block
    - Illustration: [User perspective vs. SSD perspective](https://cdn.tutsplus.com/mac/uploads/2014/01/TRIM-ExplanationOff-1.jpg)
    * A file is (almost always) *distributed* over multiple blocks
    * A file is *arbitrarily bounded* within a matrix of blocks



## File elements

1. An identifier data structure, usually with a numeric identifier
    * Unix-types OSs track files by their *index nodes* (*inodes*)
        - Contains memory block address of the file, plus file attribute metadata (modification date, owner, access permissions, etc.)
    * An *inode table* associates *inode numbers* with their inodes, for reference
1. A filename
    * A name given to the file either by the OS or by the user
    * Must be unique within a directory
    * The filesystem records a relationship between the inode and the filename
    * This relationship is represented as a file *directory* or folder containing both filename and inode number
1. The file contents



## Viewing file elements

* `DO`: [Javascript PC Emulator](http://bellard.org/jslinux/)

        # mkdir temp
        # cd temp
        # echo "Foo, bar, foobarbarous" > foo.txt
        # ls -li foo.txt
        # cat foo.txt



## Binary data

* *All* data stored or transmitted by a computer
* Not "human-readable" unless interpreted as text
* Image files; audio files
* Compiled executable program files (which may *also* contain ASCII or Unicode text)



## Text data

* Binary data that *happens to be interpreted* as text
* ASCII or Unicode codes assigned to represent a certain character
* "Human-readable"



## Text file

* Text file as container of the content *text data*
* [POSIX definition](http://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_397)
    1. "A file that contains [text] characters organized into zero or more lines" (terminated by a newline character)
    1. "The lines do not contain NUL characters" (used in data formats and programming languages to mark the end of a string)



## Program as text file

    #include <stdio.h>

    main()
    {
        printf("hello, world!\n");
    }



## Compiling a program text file

* `DO`: [Javascript PC Emulator](http://bellard.org/jslinux/)

        # cat hello.c
        # tcc hello.c
        # hexdump a.out
        # hexdump -C a.out

(Javascript PC Emulator provides the file `hello.c` in its root directory; you don't need to create it. `tcc` is a substitute for the `gcc` compiler, which Javascript PC Emulator provides, but which is slow)



## Filesystem elements

1. File
2. Directory (or folder)
3. Metadata



## Filesystem elements: directory (folder)

* Also an abstraction: a kind of *user interface*
* Like *file*, the concept of a *folder* is adapted from the domain of paper documents
    - [Representation of hierarchical file system design for the Electronic Recording Machine Accounting (ERMA) Mark 1](http://i.stack.imgur.com/r7Ahq.png) as labeled manila folders in an enclosing folder (Fig. 3)
* In a hierarchical file system, directories can contain subdirectories
* A directory or folder is a filesystem concept
* A [folder icon](https://upload.wikimedia.org/wikipedia/commons/2/2e/Crystal_folder.png) is a GUI metaphor that represents that concept



## Filesystem elements: metadata

* File attribute metadata for individual files
* Directory tables that store the names of the files in a directory
* Memory and storage media attributes



## Filesystem history: Bush's memex

* Social benefits of science
    1. Material: food, clothing, shelter, physical health
    1. Immaterial: knowledge

* Conditions of modern progress
    1. Knowledge requires *specialization*
    1. Specialization is necessary for *progress*

* Problems with specialization 
    1. *Fragments* knowledge, and
    1. Produces knowledge *in excess*

* "A transformation in scientific records"
    1. "Mechanical aids"
    1. "Mature," "creative" thought



## Indexing systems: arbitrary linear sequences

* 1, 2, 3, 4, 5, 6, 7, 8, 9, 10...
* A, B, C, D, E, F, G, H, I, J, K, L...
* "The human mind does not work that way. [Rather,] It operates by association" {% cite bush_as_1945 --file 11-file-1 %}



## Bush: Associative indexing

* "This is the essential feature of the memex" {% cite bush_as_1945 --file 11-file-1 %}
* "Building a trail": [Dynamic Diagrams: Macromedia Director “Memex” application](http://www.youtube.com/watch?v=c539cK58ees) (1995)



## Douglas Engelbart, NLS ("oN Line System") demo (1968)

[Full video and annotated segments](http://sloan.stanford.edu/MouseSite/1968Demo.html), MouseSite, Stanford University

* Clip #2, introduction
* Clip #3, Word processing and file creation



## Engelbart: File as "symbol structure"

> Any file is a symbol structure whose purpose is to represent a variety of concepts and concept structures in a way that makes them maximally available and useful to the needs of the human's mental-structure development [...] The Memex adds a factor of speed and convenience to ordinary filing-system (symbol-structuring) processes that would encourage new methods of work by the user, and it also adds speed and convenience for processes not generally used before. {% cite engelbart_background_1962 --file 11-file-1 %}



## Ted Nelson: A "dream file"

* "The kinds of file structures required if we are to use the computer for personal files and as an adjunct to creativity are wholly different in character from those customary in business and scientific data processing" {% cite nelson_complex_1965 --file 11-file-1 %}
* "...the *dream* file: the file system that would have every feature a novelist or absent-minded professor could want, holding everything he wanted in just the complicated way he wanted it held, and handling notes and manuscripts in as subtle and complex ways as he wanted them handled" {% cite nelson_complex_1965 --file 11-file-1 %}



## Nelson: a file structure for change

* "The physical universe is not all that decays. So do abstractions and categories. Human ideas, scholarship, and language are constantly collapsing and unfolding. ... While [this process] may be erratic, it never stops; and the meaning of all this for information retrieval should be clear" {% cite nelson_complex_1965 --file 11-file-1 %}
* "To the extent that information retrieval is concerned with seeking *true* or *ideal* or *permanent* codes and categories... [it] seems to me to be fundamentally mistaken. *The* categories are chimerical (or temporal) and our categorization systems must evolve as they do. ... [T]he only ultimate structure is change itself" {% cite nelson_complex_1965 --file 11-file-1 %}

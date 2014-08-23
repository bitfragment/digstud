---
title:        'File: Program'
subtitle:     
version:      $version$
embed-vcs:    true
date:         $date$
description:  Course notes on the 'file' subtopic 'program'
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

[Slide version](11-program-slides-revealjs.html)


Readings
--------

{% bibliography --file 11-file-3-program %}



What is a program?
------------------

* `DO`: Hello world! in Ruby (use [Codecademy Labs](http://labs.codecademy.com/))

      def hello
          puts 'hello world!'
      hello

* `DO`: Hello world! in Python (use [Codecademy Labs](http://labs.codecademy.com/))

      def hello():
          print 'hello world!'

      hello()



The double life of programs: three doubles
------------------------------------------

* Semantic
    1. As instructions
    2. As data

* Ontological
    1. A static text artifact or product
    2. When executed, a dynamic computational process

* Legal
    1. Text, therefore protected by copyright
    2. Mechanism, therefore patentable



Layers of abstraction
---------------------

"…the whole history of computer science has seen the careful construction of layer upon layer of **distancing abstractions** upon the basic foundation of zeros and ones. Each time a programmer writes and executes a high-level program, these layers are stripped away one by one in elaborate translations from talk of, say, chat rooms, to talk of windows, to talk of matrices, to talk of variables, registers, and memory addresses too, finally, zeros and ones. As an abstraction, this  translation is complete and flawless. {% cite colburn_software_1999 -l 16 --file 11-file-3-program %}



Algorithm
---------

* Colloquial usage
    - A byproduct of contemporary digital culture
    - Any specification of steps in a procedure
        + Example: [An Algorithm: Baking a Cake](http://www.wiley.com/college/busin/icmis/oakman/outline/chap05/slides/algor.htm)
* More precise usage in computing
    - Mathematical or logical operations
* [Euclid's algorithm](http://en.wikipedia.org/wiki/Euclidean_algorithm)



Exercise: algorithm
-------------------

Write an algorithm that will help someone find her or his way to our classroom.

TODO: ANGEL Assessment: write an algorithm for making the perfect sandwich (or the perfect lunch, if you don't like sandwiches)



Algorithm as abstraction
------------------------

* An *algorithm* is an abstract computational method that exists "apart from any programming language." {% cite knuth_algorithm_1966 --file 11-file-3-program %}

* A *program* is a representation and a concrete "embodiment" of an algorithm in a particular language {% cite knuth_algorithm_1966 --file 11-file-3-program %}



Pseudocode
----------

* An algorithm can be expressed *informally* in a natural language like English
    - Your algorithm for locating our classroom
* An algorithm can be expressed *formally* in an artificial programming language



Pseudocode example
------------------

    If it is a weekday, then:
        If it is a weekday when this class meets, then:
            Get up
            For each cup in three cups of coffee:
                Drink cup
            Walk to campus
            Walk to the building where this class meets
            Walk to the classroom where this class meets
        Else
            Do something else
    Else
        Stay in bed


TODO: Assessment: write pseudocode

WORKINGHERE: remainder of proglang-notes on program

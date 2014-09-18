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



Readings
--------

{% bibliography --file 11-file-3-program %}



What is a program?
------------------

* `DO`: Hello world! in Ruby (use [Codecademy Labs](http://labs.codecademy.com/))

      def hello
          puts 'hello world!'
      end


      hello()

* `DO`: Hello world! in Python (use [Codecademy Labs](http://labs.codecademy.com/))

      def hello():
          print 'hello world!'


      hello()



Execution
---------

       javascript:alert("Hello world!");



The double life of a program: three doubles
-------------------------------------------

* Ontological
    1. A static text artifact or product
    2. When executed, a dynamic computational process

* Semantic
    1. As data
    1. As instructions

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
        * [Example]()![fit](https://jurnalpelajarbodoh.files.wordpress.com/2013/09/alg-dilbert.gif)
    - Any specification of steps in a procedure
        + Example: [An Algorithm: Baking a Cake](http://www.wiley.com/college/busin/icmis/oakman/outline/chap05/slides/algor.htm)
* More precise usage in computing
    - Mathematical or logical operations
* [Euclid's algorithm](http://en.wikipedia.org/wiki/Euclidean_algorithm)



Exercise: algorithm
-------------------

* Write an algorithm that will help someone find her or his way to our classroom
* Write an algorithm for making the perfect sandwich (or the perfect lunch, if you don't like sandwiches)



Algorithm as abstraction
------------------------

* An *algorithm* is an abstract computational method that exists "apart from any programming language." {% cite knuth_algorithm_1966 --file 11-file-3-program %}

* A *program* is a representation and a concrete "embodiment" of an algorithm in a particular language {% cite knuth_algorithm_1966 --file 11-file-3-program %}



Pseudocode
----------

* An algorithm can be expressed *informally* in a natural language like English
    - Your algorithm for locating our classroom
* An algorithm can be expressed *formally* in an artificial programming language
    - [Greatest common divisor - Rosetta Code: BASIC](http://rosettacode.org/wiki/Greatest_common_divisor#BASIC)
    - [Greatest common divisor - Rosetta Code: JavaScript](http://rosettacode.org/wiki/Greatest_common_divisor#JavaScript)
    - [Greatest common divisor - Rosetta Code: Python](http://rosettacode.org/wiki/Greatest_common_divisor#Python)
    - [Greatest common divisor - Rosetta Code: Ruby](http://rosettacode.org/wiki/Greatest_common_divisor#Ruby)



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

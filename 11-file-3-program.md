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

Plain text that can be interpreted as instructions to perform a computational process



Hello world
-----------

The simplest program is a single instruction:

    print "Hello world!"




Functions
---------

    def hello
        print 'Hello world!'
    end

* Here, a separate *function*
* Like a dictionary definition



…and function calls
-------------------

    def hello
        print 'Hello world!'
    end

    hello()

* Calling a function is like looking up and reading a dictionary definition
* A programming language interpreter reads the definition and executes the instructions it contains



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
        * [Example](https://jurnalpelajarbodoh.files.wordpress.com/2013/09/alg-dilbert.gif)
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



From "computer" to "programmer"
-------------------------------

The word "computer" originally denoted a human occupation:

> During the war, BRL [U.S. Army Ballistic Research Laboratory] recruited approximately two hundred women to work as computers, hand-calculating firing tables for rockets and artillery shells. {% cite light_when_1999 --file 11-file-3-program %}
 
During and after WWII, the denotation of "computer" shifted to the electromechanical or electronic machine that automated and replaced that human occupation:

> During World War II, a "computer" was a person who calculated artillery firing tables using a desk calculator. Six women "computers" were assigned to serve as ENIAC's original programming group. Although most were college graduates, the "girls" were told that only "men" could get professional ratings. Finally, in November 1946, many of the women received professional ratings. {% cite moye_eniac:_1996 --file 11-file-3-program %}

> ENIAC's first application was to solve an important problem for the Manhatten [*sic*] Project. Involved were Nicholas Metropolis and Stanley Frankel from the Los Alamos National Laboratory, who worked with Eckert, Mauchly, and the women programmers. Captain (Dr.) Goldstine and his wife, Adele, taught Metropolis and Frankel how to program the machine, and the "girls" would come in and set the switches according to the prepared program. {% cite moye_eniac:_1996 --file 11-file-3-program %}

* [Early NACA human computers at work](http://www.dfrc.nasa.gov/Gallery/Photo/People/Small/E49-0053.jpg)
* [ENIAC, 1946 (Penn Engineering)](http://www.seas.upenn.edu/images/about-seas/eniac-home.jpg)
* [ENIAC tube change](http://s7.computerhistory.org/is/image/CHM/500004289-03-01?$re-zoomed$)
* [ENIAC being set up (Computer History Museum)](http://s7.computerhistory.org/is/image/CHM/102622742-03-01?$re-zoomed$)
* [ENIAC programmers (Computer History Museum)](http://s7.computerhistory.org/is/image/CHM/102618640-03-01?$re-story-hero$)
* [Programming the ENIAC (Columbia University Computing History)](http://www.columbia.edu/cu/computinghistory/eniac1.jpg)
* [Programming the ENIAC (Columbia University Computing History)](http://www.columbia.edu/cu/computinghistory/eniac7.gif)
* [Jean Bartik: ENIAC's Programmers (Computer History Museum)](http://www.computerhistory.org/revolution/birth-of-the-computer/4/78/2258)



Stored program computing
------------------------

* Advantages of stored program computing architecture
    1. Preparing the program in advance and storing it as data enables faster execution
    1. Ability to treat program as data and modify it when you want to
        * Ability to operate on program data itself
        * Example: storing commonly used subroutines in advance and calling them from a program when they were needed
        * Such subroutines could be written in binary operation codes, then "called" by a program written in a higher-level code: for example, a code using words from the English language ("set," "get," "goto", "print"), which are easier for humans to read and write

This is really the beginning of the history of what we now call "programming languages":

> By storing a program and data in a common high-speed memory, not only could programs be executed at electronic speeds; the programs could also be operated on as if they were data — the ancestor of today’s high-level languages compiled inside modern computers. {% cite ceruzzi_stored_2012 --file 11-file-3-program %}

Ceruzzi: the "stored program principle" was so influential that the referent of the word "computer" shifted once again. Now, it described electromechanical or electronic machines designed with a stored program architecture, rather than other designs:

> The definition of *computer* thus changed, and to an extent it remains the one used today, with the criterion of programmability now extended to encompass the internal storage of that program in high-speed memory. {% cite ceruzzi_stored_2012 --file 11-file-3-program %}



Assemblers and alphanumeric assembly codes
------------------------------------------

[EDSAC (University of Cambridge, 1949)](http://www.cl.cam.ac.uk/relics/jpegs/edsac_wilkes.jpg)

* EDSAC provided a hard-wired assembler program stored in ROM, allowing the programmer to enter brief alphanumberic codes instead of coding in binary notation
* The assembler performed the "translation" of those alphanumberic codes into binary code
* This assembler program was called "initial orders" (it had two versions)
* "Hello World" for EDSAC initial orders 1, from [EDSAC Programming Tutorial](http://www.cl.cam.ac.uk/events/EDSAC99/simulators/echo/flat.html):

        T56F
        ZF 
        TF 
        O43F 
        A34F 
        A41F 
        U34F 
        S42F 
        G33F 
        ZF 
        P1F O56F 
        *F HF EF LF LF OF 
        !F WF OF RF LF DF &F


* These are the alphanumeric assembler codes for a "Hello world!" program written for EDSAC's "initial orders" assembler 1
* The first two lines are preparatory codes, stopping any prior process and clearing the memory
* The remainder of the program directs the machine's teleprinter to print a series of alphabetic charaters, the string "Hello world!"
* They tell it to retrieve one character at a time from the character codes on the last two lines of the program, store them in memory, and then print them using the teleprinter



Compilers
---------

> ...a special kind of program, later called a compiler, would take as its input instructions written in a form that was familiar to human programmers and easy to grasp, and its output would be another program, this one written in the arcane codes that the hardware was able to decode. {% cite ceruzzi_stored_2012 --file 11-file-3-program %}

* Terminology was in flux, and its took time for the meaning of the word "compiler" to stabilize
* A compiler performed the same function as what was earlier sometimes called an "assembler": translating higher-level codes that were easy for the programmer to write into lower-level machine codes
* This amounts to writing in a "programming language," instead of entering such <a href="#/hello-world-for-edsac-initial-orders-1">operation codes</a>

### "Hello world!" written in the C programming language

    #include<stdio.h>

    main()
    {
        printf("Hello World");

    }

### Compiling the plain text file `hello.c`

    $ gcc -v hello.c

### Executing the object code produced by the compiler

    $ ./a.out
    Hello world!



From "compiler" to "programming language"
-----------------------------------------

Eventually, the term "compiler" came to refer to a software program that performed that translation, while "programming language" came to refer to the particular code used by the programmer to write for the compiler

> It was also around this time that these codes came to be called “languages,” because they shared many, though not all, characteristics with spoken languages. {% cite ceruzzi_stored_2012 --file 11-file-3-program %}

* The *analogy* was based on the fact that natural languages and programming languages shared *a few restricted attributes,* such as syntactic rules
* Programming languages have rules of syntax just as natural languages do, though in the case of programming languages the rules are deliberately designed, whereas in natural languages, we become aware of those rules only *after* learning to use them


FORTRAN (FORmula TRANslation), 1957
-----------------------------------

* Compare the below with a more "direct" programming using EDSAC's operation codes:

       PRINT *, "Hello World!"
       END

* This is a "Hello world!" program written in FORTRAN, the first higher-level programming language
* Much more like English than the operation codes used to program EDSAC's assembler


COBOL (COmmon Business-Oriented Language), 1958
-----------------------------------------------

* Designed as a common business programming language
* Used an even more extensively English-like syntax



FORTRAN and COBOL: algebraic notation vs. English-language prose
----------------------------------------------------------------

### FORTRAN

Conditional (if) statement that is true if value of a is larger than value of b:

    IF A > B



### COBOL

    IF EMPLOYEE-HOURS IS GREATER THAN MAXIMUM

* In COBOL programming one might deliberately use use long value or variable names (`EMPLOYEE-HOURS`) instead of simple letter symbols (`A`, `B`)
* One can use English prose expressions (`GREATER THAN`, `MAXIMUM`) rather than algebraic symbols



Clumsiness of the analogy between language and code
---------------------------------------------------

This is the beginning of a certain confusion caused by the analogy between *code* and *human language*

> In the years that followed, researchers explored the relationship between machine and human language, and while COBOL was a significant milestone, it gave the illusion that it understood English better than it really did. (Paul Ceruzzi, *A History of Modern Computing*)

> The word “language” turned out to be a dangerous term, implying much more than its initial users foresaw. The English word is derived from the French *langue,* meaning tongue, implying that it is spoken. Whatever other parallels there may be with natural language, computer languages are not spoken but written, according to a rigidly defined and precise syntax. (Paul Ceruzzi, *A History of Modern Computing*)



Natural languages
-----------------

Downey, Elkner & Meyers, "Formal and Natural Languages" {% cite downey_formal_2013 --file 11-file-3-program %}

1. Are *spoken*
2. Were not *designed*
3. Can be *ambiguous* and *context-dependent* in usage
4. Are *redundant* and *verbose* or "noisy" as a result



Formal languages
----------------

Downey, Elkner & Meyers, "Formal and Natural Languages" {% cite downey_formal_2013 --file 11-file-3-program %}

1. Are *not* spoken
2. *Were* designed
3. Were designed to be *unambiguous* in usage
4. Are *concise* as a result


Programming languages
---------------------

Downey, Elkner & Meyers, "Formal and Natural Languages"  {% cite downey_formal_2013 --file 11-file-3-program %}

Programming languages are *formal* languages that were "designed to express computations"

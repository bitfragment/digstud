## What is a program?

Plain text that can be interpreted as instructions to perform a computational process

----

## Hello world

        print "Hello world!"

^ 
* Simplest program is a single instruction
* Here, in 2 langs = the same syntax
* Demo in JavaScript using console.log() and alert()

----

## Functions

    def hello
        print 'Hello world!'
    end

^
* Slightly longer
* Separate function (like a dictionary definition)…
* [Open Codecademy Labs/ Ruby, explain interface, demo both simple and function versions: function doesn't execute; why]

----

## …and function calls

        def hello
            print 'Hello world!'
        end

        hello()

^
* Function call (like a dictionary lookup)
* The function call reads the definition and executes the instructions in contains
* [Demo how it runs now]

----

## The double life of a program

* Ontological
* Semantic
* Legal

^
* Even after 50 years of programming, programs are objects with an ambiguous status
* Three ways in which a program live a "double life"
* Ontological: what kinds of objects they are
* Semantic: what the word "program" means
* Legal: how legal system views programs

---

## The double life of a program

* Ontological
    1. A static text artifact or product
    2. When executed, a dynamic computational process

^
* Ambiguity is in the executability of program text
* [Demo again with JavaScript alert()]

----

## The double life of a program

* Semantic
    1. As data
    2. As instructions

^ 
* Program text is indistinguishable from any other kind of ASCII text, when stored as data
* A special kind of data that produces a computational process
* You can't execute a text file that is not written in a programming language

----

## The double life of a program

* Legal
    1. Text, therefore protected by copyright
    2. Mechanism, therefore patentable

^
* Two divisions of US IP law:
* Text (and later, visual art forms): protected by copyright
* Machines: protected by patents
* Law is still "confused" on this issue

----

Colburn, "Software, Abstraction, and Ontology"

> …the whole history of computer science has seen the careful construction of layer upon layer of **distancing abstractions** upon the basic foundation of zeros and ones.

^ 
* This fundamental, unresolvable ambiguity of programs (for now):
* Consequence of their place in the layers of abstraction that make up a computer system

----

Colburn, "Software, Abstraction, and Ontology"

> Each time a programmer writes and executes a high-level program, these layers are stripped away one by one in elaborate translations from talk of, say, chat rooms, to talk of windows, to talk of matrices, to talk of variables, registers, and memory addresses too, finally, zeros and ones. As an abstraction, this  translation is complete and flawless.

-----

## What is a program?

### Concrete definition

Plain text that can be interpreted as instructions to perform a computational process

### Abstract definition

An algorithm

^
* Concrete or material definition
* Conceptual definition
* Algorithm: sequence of instructions
* (From mathematics)

----

![fit](https://jurnalpelajarbodoh.files.wordpress.com/2013/09/alg-dilbert.gif)

^
* We often use "algorithm" in a loose sense today
* ?(What's the joke here?)

----

![125%](https://www.coastal.edu/mathcenter/HelpPages/GCD/img002.GIF)

^
* Euclid (300 BC): wrote *Elements*; early geometry & other math
* Devised an algorithm for mathematically calculating the greatest common divisor of two numbers
* A sequence of instructions for performing calculations
* [Read this]

----

![125%](http://i.ytimg.com/vi/AJn843kplDw/hqdefault.jpg)

^
* Following those prose instructions…
* Do the calculations
* Obtain the desired result

----

![125%](http://image.tutornext.com/cms/files/u59/Pictures%20for%20tv2_229.gif)

^
* [More elaborate representation]

----

## Following "prose" instructions…

## …to perform a mathematical computation

^
* When you use Euclid's algo…
* …you are doing what a computer does, executing a program

----

![](http://www.wiley.com/college/busin/icmis/oakman/outline/chap05/images/f5_01.gif)

^
* Other daily activities other than math might be called "algorithms"
* Following a recipe
* [Read the steps]
* Follow steps to produce a particular result

---

![fit](http://pad2.whstatic.com/images/thumb/f/ff/Give-Directions-Step-4.jpg/670px-Give-Directions-Step-4.jpg)

^
* ?(What's this)
* Again, follow steps to produce a desired result

----

## (Just) reading

## Reading AND executing

^
* As with a computer program…
* Recipes and directions are text instructions that are not JUST read…
* …the way a newspaper article is read
* The goal is to produce an ACTION

----

## Exercises

1. Write an algorithm that will help someone find her or his way to our classroom from College Avenue

1. Write an algorithm for making the perfect sandwich (or the perfect lunch, if you don’t like sandwiches)

----

Knuth, Donald E. “Algorithm and Program; Information and Data”:

1. An algorithm is an abstract computational method that exists “apart from any programming language”

1. A program is a representation and a concrete “embodiment” of an algorithm in a particular language

^
* Here's how computer scientists have defined "algorithm" and "program"
* Algorithm: instructions that can be implemented in various ways
* Program: particular implementation of a particular algorithm

----

![125%](https://www.coastal.edu/mathcenter/HelpPages/GCD/img002.GIF)

^
* Algorithm expressed in "prose" instructions…
* That is, in human language

----

## Euclid's algorithm implemented in programming languages

http://rosettacode.org/wiki/Greatest_common_divisor

^
* BASIC
* JavaScript
* Python
* Ruby

----

## Pseudocode

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

^
* Programmers actually write out "prose" instructions in human language
* Before they actually write the code in a specific language's syntax
* Use general programming language syntax
* Conditionals: If ... then ... else
* Loops (iteration): For ... each
* Indentation and nesting to indicate sequence

----

![fit](http://www.dfrc.nasa.gov/Gallery/Photo/People/Small/E49-0053.jpg)

^
* A little history, now
* [Read caption]
* ?(What does caption mean)
* The English word "computer" in the 1940s referred to these women
* Who were doing a particular job

----

Light, "When Computers Were Women":

> During the war, BRL [U.S. Army Ballistic Research Laboratory] recruited approximately two hundred women to work as computers, hand-calculating firing tables for rockets and artillery shells.

----

Moye, "ENIAC: The Army-Sponsored Revolution"

> During World War II, a “computer” was a person who calculated artillery firing tables using a desk calculator. 

----

![fit](http://www.seas.upenn.edu/images/about-seas/eniac-home.jpg)

^
* ENIAC (Electronic Numerical Integrator and Computer), 1946
* Built University of Pennsylvania
* Financed by the US Army Ballistics Research Laboratory
* Designed to do the job those women were doing: calculate artillery firing tables
* That is, to replace the human computers

----

![fit](http://s7.computerhistory.org/is/image/CHM/500004289-03-01?$re-zoomed$)

^
* ENIAC took up an entire room
* It used ~17,500 vacuum tubes for performing [decimal] calculations
* Here's a pic of a tube being changed

----

![fit](http://s7.computerhistory.org/is/image/CHM/102622742-03-01?$re-zoomed$)

^
* Here you can also see a lot of wires
* ENIAC was "programmed" not using a programming language, but by setting switches and connecting components using plugs and wires
* A manual process

----

Moye, "ENIAC: The Army-Sponsored Revolution"

> During World War II, a “computer” was a person who calculated artillery firing tables using a desk calculator. Six women “computers” were assigned to serve as ENIAC’s original programming group.

^
* So, what happened to the women "computers" who were replaced by machines like ENIAC
* Some of them lost the opportunity to work
* But some of them, once they were no longer the first "computers," became the first "programmers"

----

![fit](http://www.columbia.edu/cu/computinghistory/eniac2.gif)

----

![fit](http://s7.computerhistory.org/is/image/CHM/102618640-03-01?$re-story-hero$)

----

![fit](http://www.columbia.edu/cu/computinghistory/eniac1.jpg)

----

![150%](http://www.columbia.edu/cu/computinghistory/eniac7.gif)

---

## Jean Bartik: ENIAC's Programmers

^
* One of the original six ENIAC programmers

----

## Stored program computing

^
* The original design for ENIAC required manual "programming" for each task
* Laborious
* In all these pictures [flick back], a physical activity
* Nothing like sitting at a keyboard typing, today
* That labor-intensive nature → idea of "preprogramming" the machine
* In other words, storing programs in advance and then calling them

----

## Programming languages

Ceruzzi, *Computing: A Concise History*:

> By storing a program and data in a common high-speed memory, not only could programs be executed at electronic speeds; the programs could also be operated on as if they were data — the ancestor of today’s high-level languages compiled inside modern computers.

^
* New designs abandoned ENIAC's manual set-up
* Designed with memory that could store programs in advance
* Storing programs in memory meant they could be executed more quickly
* Also meant that programs were stored as data, like any other data
* Beginning of the ontological ambiguity of the program: static text data that can be interpreted as a dynamic computational process

----

![fit](http://www.cl.cam.ac.uk/relics/jpegs/edsac_wilkes.jpg)

^
* EDSAC, University of Cambridge, 1949
* A stored-program computer

----

![125%](http://www.dspguide.com/graphics/T_4_3.gif)

^
* Remember that the “verbosity” of binary notation was a problem for human beings
* A microprocessor (hardware) instruction set is represented in a "machine code" or "machine language" specified in binary notation
* [describe image]

----

![150%](http://2.bp.blogspot.com/-pclOIGp0F0E/UBqOQHCXZcI/AAAAAAAAAKk/FRR2VdNum6g/s1600/AssemblyLanguage.png)

^
* Alphanumeric codes were devised as shorthand for the binary notation
* Symbolic assembly codes/languages
* This is what was "stored" in a stored-program computer

----

![fit](http://cdn1.raywenderlich.com/wp-content/uploads/2013/05/SpeakAssembly.png)

^
* Think of machine code, in binary notation, as a computer's "native" language
* Assembly code stored in the computer is like a foreign language taught to the computer so it can communicate with humans more easily
* It's also taught how to translate from assembly to machine code

----

## "Hello world!" in EDSAC "initial orders 1" assembly code

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

^
* Characters are stored in last two lines
* Previous is a set of instructions to retrieve and print them
* This is compressed alphanumeric notation
* Less verbose than binary notation, but still hard to read

----

![150%](http://trycatch22.com/blog/wp-content/uploads/2012/10/ProgrammingToolchain.png)

^
* Stored-program architecture is like a pyramid
* [Explain]

----

## FORTRAN (FORmula TRANslation), 1957

		 PRINT *, "Hello World!"
		 END

^ 
* Next step: design of programming languages that looked more like human language
* “Hello world!” in FORTRAN, the first higher-level programming language
* Much more like English than the operation codes used to program EDSAC’s assembler [flip back]

----

## COBOL (COmmon Business-Oriented Language), 1958

^
* Designed as a common business programming language
* Used an even more extensively English-like syntax

----

## FORTRAN and COBOL: algebraic notation vs. English-language prose

### FORTRAN

		IF A > B

### COBOL

		IF EMPLOYEE-HOURS IS GREATER THAN MAXIMUM

^
* FORTRAN: Conditional (if) statement that is true if value of a is larger than value of b:
* COBOL: longer value or variable names instead of simple letter symbols
* COBOL: English prose expressions rather than algebraic symbols

----

![150%](http://trycatch22.com/blog/wp-content/uploads/2012/12/ProgrammingToolchain2.png)

^
* English-like proglangs needed software compilers to translate them into assembly code (or directly into machine code)

----

## “Hello world!” in the C programming language

		#include<stdio.h>
		
		main()
		{
		    printf("Hello World");
		
		}

----

## Compiling the plain text file hello.c

		$ gcc -v hello.c

^
* [Cat the file in my CLI and compile it]

----

## Executing the object code produced by the compiler

		$ ./a.out
		Hello world!

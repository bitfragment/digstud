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













    







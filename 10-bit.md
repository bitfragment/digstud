---
title:        Bit
subtitle:     
version:      $version$
embed-vcs:    true
date:         $date$
description:  Course notes on the topic 'bit'
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

[Slide version](10-bit-slides-revealjs.html)

Readings
--------

{% bibliography --file 10-bit %}


Digital: etymology and history
------------------------------

* *OED*: [digital, n. and adj.](http://www.oed.com.ezaccess.libraries.psu.edu/view/Entry/52611)
    - English *digital* < classical Latin *digitalis,* "measuring a finger's breadth"
    - In post-classical Latin, a broader meaning: "of or relating to the finger" (*digitus,* finger)
    - Also used to describe the whole numbers from 1-9 ("single digits")
    - In domain of electronics and computing, used to denote representation by *discrete* values, usually in *binary* form
    - In domain of electronics and computing, used in contrast with *analog*

* "Digital paradigm" {% cite ceruzzi_introduction_2012 --file 10-bit %}
    - "…the notion of coding information, computation, and control in binary form, that is, a number system that uses only two symbols, 1 and 0, instead of the more familiar decimal system that human beings, with their ten fingers, have used for millennia" {% cite ceruzzi_introduction_2012 --file 10-bit -l x %}
    - "It is not just the use of binary arithmetic, but also the use of binary logic to control machinery and encode instructions for devices, and of binary codes to transmit information" {% cite ceruzzi_introduction_2012 --file 10-bit -l xi %}

* Catachrestic and/or ideological usage
    - As equivalent of *new* (novelty, progress)
    - As equivalent of *inevitable*
    - Example: [Change Ahead: Our digital future is inevitable. But, then, it always has been](http://expandiverse.com/files/2013/02/Blog-1-Artwork-4Feb20131-300x300.png) ([source](http://expandiverse.com/2013/02/11/our-digital-future-is-inevitable-but-then-it-always-has-been/))


Binary numeration
-----------------

* [Binary digit](http://en.wikipedia.org/wiki/Bit) or "bit"
    - Find an ordinary "toggle" light switch (not a dimmer)
        + Flip the switch. Is the lamp on, or is it off?
        + Flip the switch again. Is the lamp on, or is it off?
        + Flip the switch one more time. Is the lamp on, or is it off?
        + The lamp controlled by the switch has only two *states*
    - [Illustration](http://www.cambridgedigital.com/mooc/html/jan14/31_Activity1/31_Activity1.html) (navigate forward to second panel titled "On and Off")
    - A device with two *states* can represent a binary digit with only two *values*
* [Counting in binary](http://en.wikipedia.org/wiki/Binary_number#Counting_in_binary)
    - 0, 1, 10, 11, 100, 101, 110, 111, 1000, 1001
    - [Illustration](http://britton.disted.camosun.bc.ca/binary_count.gif)
    - [Another illustration](http://www.homofaciens.de/bilder/technik/computer_024a.gif)
* A [binary number](http://en.wikipedia.org/wiki/Binary_number) consists of groups of bits
    - [Illustration](http://www.cambridgedigital.com/mooc/html/jan14/31_Activity1/31_Activity1.html) (navigate forward to third panel titled "Groups of bits")


Bit storage: history
--------------------

* [Punched cards](http://en.wikipedia.org/wiki/Punched_card) and [punched tape](http://en.wikipedia.org/wiki/Punched_tape) (19C-20C)
    - Punched/not punched
    - [Illustration](http://content.answcdn.com/main/content/img/CDE/_PUNCHCD.GIF)
* [Electrical relays](http://en.wikipedia.org/wiki/Relay) (19C-20C)
    - Open/closed states
    - [Illustration](http://www.electronics-tutorials.ws/io/io24.gif), from [Electrical Relay and Solid State Relays for Relay Switching](http://www.electronics-tutorials.ws/io/io_5.html)
* [Vacuum tubes](http://en.wikipedia.org/wiki/Vacuum_tube) (19C-20C)
    - Polarity of electrical charge
    - [Illustration](http://media.bestofmicro.com/,P-X-302901-3.jpg), from [From Tubes To Transistors - Computer History 101: The Development of the PC](http://www.tomshardware.com/reviews/upgrade-repair-pc,3000-2.html)
* [Magnetic tape](http://en.wikipedia.org/wiki/Magnetic_tape), [drum](http://en.wikipedia.org/wiki/Magnetic_drum), and [disk](http://en.wikipedia.org/wiki/Disk_storage) (1950s–)
    - Polarity of magnetization
* [Integrated circuits](http://en.wikipedia.org/wiki/Integrated_circuit) (silicon microchips) (1960s–)
    - Polarity of electrical charge (capacitor)


Binary representation
---------------------

* Binary representation as "lowest layer" of abstraction
    - "All information in a system — including disk files, programs stored in memory, user data stored in memory, and data transferred across a network — is represented as a bunch of bits" {% cite bryant_tour_2011 --file 10-bit %}
    - Bits are *grouped* into data objects, providing *context* for their *interpretation* {% cite bryant_tour_2011 --file 10-bit %}
* Bit and byte
    - A binary number has a [bit length](http://en.wikipedia.org/wiki/Bit-length)
    - In computing, a standard [byte](http://en.wikipedia.org/wiki/Byte) is a grouping of eight bits, or bit string


Memory addressing
-----------------

* Virtual memory
    - An abstraction of physical memory capacity in RAM, disk storage, other hardware, and OS operations
        + Illustration: [IBM PC motherboard with memory area highlighted](http://www.jbcs.co.za/ham_radio/Memory_files/image006.gif), from [Memory, memory addressing & structure](http://www.jbcs.co.za/ham_radio/Memory.htm)
    - Represented by a [page table](http://en.wikipedia.org/wiki/Page_table)
        + Illustration: [representation of system memory addresses](http://www.jbcs.co.za/ham_radio/Memory_files/image023.gif), from [Memory, memory addressing & structure](http://www.jbcs.co.za/ham_radio/Memory.htm)
* [Byte addressing](http://en.wikipedia.org/wiki/Byte_addressing) and word size
    - The "smallest addressable unit of memory" is not the bit, but the byte {% cite bryant_tour_2011 --file 10-bit %}
    - In the same context, the largest addressable unit of memory is the [word](http://en.wikipedia.org/wiki/Word_(computer_architecture))
        + **First of the *transpositions of linguistic concepts* that we will encounter in the history of computing**
        + 32-bit computer systems have a word size of 4 bytes
        + 64-bit computer systems have a word size of 8 bytes
    - Different data types are allocated different quantities of memory
        + An ASCII alphanumeric character is allocated one byte
        + Integers and floating point numbers might be allocated two or four bytes


Character display
-----------------

* Binary representation of human writing systems
    - "What makes personal computers useful to the majority of people is not that they can process numerical data [...] but that they can process textual data" {% cite searle_brief_2004 --file 10-bit %}
    - "[T]here are many people who are unaware of the fact that to a computer textual data are also numerical data. In modern computer systems, the individual characters of the scripts that humans use to record and transmit their languages are encoded in the form of binary numerical codes, just as are the Arabic numerals used in calculation programs" {% cite searle_brief_2004 --file 10-bit %}
    - "This is because the circuitry of the microprocessor that lies at the heart of a modern computer system can only do two things — calculate binary arithmetic operations and perform Boolean (i.e., true or false) logic operations." {% cite searle_brief_2004 --file 10-bit %}

* Character display is not inscription
    - The letter "A" is not *impressed* onto your screen
    - Nor is it *impressed* into a storage medium
    - "…when a personal computer records the letter 'A' onto a floppy disk, for instance, it does not create an image of the letter 'A' with tiny magnetic dots, rather it records a binary number (made up of zeroes and ones) that represents the letter 'A' in a character code table" {% cite searle_brief_2004 --file 10-bit %}

* Character display process
    1. Hardware keyboard provides options for input
    2. Each hardware key is assigned an internal numeric key code
    3. That key code is assigned to a specific character in a specific character set and its international [code page](http://en.wikipedia.org/wiki/Code_page)
    4. That character is displayed on the screen in a particular [display font](http://en.wikipedia.org/wiki/Typeface)


Character encoding: Babel
-------------------------

> As long as the processing of information from end to end occurs only in a single machine, there is no need for a standardized character encoding. Early computers up to the beginning of the 1960s thus simply used whatever ad-hoc convention to represent characters internally seemed appropriate; some distinguished upper- and lowercase letters, most did not. {% cite schreibman_character_2004 --file 10-bit %}


Character encoding: ASCII
-------------------------

* Illustration: [USASCII code chart](http://upload.wikimedia.org/wikipedia/commons/thumb/8/85/ASCII_Code_Chart-Quick_ref_card.jpg/1280px-ASCII_Code_Chart-Quick_ref_card.jpg)
* A standard binary encoding of 95 written symbols in U.S. English
    - Numerals `0`-`9`
    - Letters `a`–`z` and `A`–`Z`
    - Basic punctuation symbols
* Plus 33 non-printing [control characters](http://en.wikipedia.org/wiki/Control_character)
* ASCII provides a one-byte (8-bit) encoding for each character
* A byte (8 bits) is represented as an eight-bit binary number


Binary and hexadecimal notation
-------------------------------

* Binary notation is "verbose" {% cite bryant_representing_2011 --file 10-bit %}
* Binary notation is "tedious" to convert to and from decimal notation {% cite bryant_representing_2011 --file 10-bit %}
* Hexadecimal (base 16) or "hex" notation
    - `0`–`9` plus `A`–`F`
* Illustration: [Hexadecimal numbering](http://www.highteck.net/images/227-Ethernet-exadecimal-numbering.jpg), from [Ethernet](http://www.highteck.net/EN/Ethernet/Ethernet.html)
* [ASCII to Hex... and other free text conversion tools](http://www.asciitohex.com)


Symbolic assembly language
--------------------------

* Another situation in which the "verbosity" of binary notation was a problem: early computer programming
* A microprocessor (hardware) instruction set is represented in a "machine language" of (here, 6-bit) binary notation:

        011011 000000 000000 000000 000001 000000
        +----+ +--------------------------------+
               ^data
        ^instruction

{% cite sammet_machine_1969 -l 2 --file 10-bit %}

* The same expression, using an alphanumeric mnemonic code for the instruction (example from Sammet, "Symbolic Assembly Language Programming"):

        CLA    000000 000000 000000 000001 000000
        +----+ +--------------------------------+
               ^data
        ^instruction

{% cite sammet_machine_1969 -l 2 --file 10-bit %}

* Systems of such mnemonic codes came to be called *symbolic assembly language*, the earliest forms of what we now call "programming languages"

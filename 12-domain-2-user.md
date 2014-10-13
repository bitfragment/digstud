---
title:        User
subtitle:     
version:      $version$
embed-vcs:    true
date:         $date$
description:  Course notes on the 'domain' subtopic 'user'
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
created:      2014-10-09
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

## Readings

{% bibliography --file 12-domain-2-user %}


## User login

* A "login" is the act or procesure of "logging in" or "logging on" to a computer system
* One "logs in" as a *user*
* A user is *identified* and *authenticated* by the system using:
    1. A text *user name*
    2. A text password
        * There is significant pressure on the convention of text password security, today, and biometric alternatives are entering the everday consumer market (e.g., Apple's TouchID); but in 2014 text password security remains the most common form of authentication in consumer computing
* This information is entered by the user into a login console or window
* The system records this information in an *access log*



## User account

**An *account* is a specific example of the general concept of a *domain,* in computing**

* Today, one "logs in" to an *account* assigned to oneself as a *user*
* Fundamental form of your relationship with any computing device

* Accounts in banking
    - *Not* a physical space set aside exclusively for your use
        + Contrast with safe deposit box
    - An abstraction or virtual space containing your assets

* An account is defined by:
    1. A configuration of access privileges, for access to computing resources
    2. A demarcation and assignment of virtual space in memory, for the storage and manipulation of data objects: the **home directory**



## Password security

* Two steps:
    1. First, identify someone as a legitimate user. Identification answers the question, *Who am I?*
    1. Second, authenticate that user. Authentication answers the question, *Are you really who you say you are?*

* Why do we need to ensure that the user is who she says she is?
    * A digital *domain* is a simulated, virtual environment
    * Easy to simulate or *masquerade* as something or someone else

* In so far as text password authentication uses forms of written language, it comprises an important part of the linguistic history of computing
    - A use of human language for a purpose beyond the usual purpose of writing or communication
* It's a part of the history of computing where the linguistic and mathematical fundamentals of computing have often been pitted against each other

* Precedents in literary history
    - The [folktale of Ali Baba and the forty thieves](http://www.youtube.com/watch?v=czro0qB72Ng)
    - Speaking the password "Open, Sesame!" grants access to cave

* From batch processing to time-sharing operating systems: one mainframe, many "dumb" terminals

* Dictionary attacks
    - In 2012, "password" was still the most popular password!
    - Why are actual words, like "password," bad passwords? Because you can find them in a dictionary, and you can write a program to try every word in a dictionary as a password
        + Also easy-to-remember sequences of numerals, like "12345"

* Why care if your password is guessed and your account hacked?
    - Mischief: vandalizing of your account
    - Identity theft and other modes of fraud
        + [NBC News broadcast August 14, 2014](http://videodelivery.nbcnews.com/now/bypass/mp4/3aaae01e-e0f4-439d-aa7a-8d5e3e774105/00000000-0000-0000-0000-000000000000/3a41c6e4-93a3-4108-8995-64ffca7b9106/555436fc-d35d-4365-acc2-192d0bf4cc18/0/0/115/406215722/content.mp4?sid=128)
        + Password system as "broken"
        + Turn to biometric authentication
* [How Secure is My Password?](https://howsecureismypassword.net)

* Biometric authentication methods represent the end of an era in the *linguistic history of computing*, as text passwords are abandoned
* Biometric alternatives
    - Fingerprints
    - Palm veins
    - Finger veins
    - Hand geometry
    - Eye veins
    - Iris of the eye
    - Walking gait
    - Voice print
    - Keystroke dynamics (typing patterns)



## Kernel space and user space ("userland")

* Once you've been identified and authenticated, an operating system grants you access to a restricted domain defined for you
* This *user space* is segregated from the operating system's *kernel space*
* The first layer of user space is the *shell*
    - A plain text *command line interface*

* Interacting with a shell: a *prompt* signals readiness to accept a command

    

## Home directory

Your home directory is user space assigned to you for file storage, but it is rarely located near or at the root of the filesystem tree

- Filesystem root
    + "Top" (or bottom) of filesystem tree
    + In Unix, one root for the entire filesystem
    + In Windows, one root for each storage device and/or partition of a storage device
- Filesystem tree
    + Stylized illustrations
        * [Windows](http://zhangjianyuan.net/wp-content/uploads/2014/04/05fig03_alt.gif)
        * [Linux](http://zhangjianyuan.net/wp-content/uploads/2014/04/05fig05.gif)
        * [Linux](http://www.csee.umbc.edu/wp-content/uploads/2012/07/linux_tree.jpg) (2)
    + Schematic illustrations
        * [Unix](http://www.openbookproject.net/tutorials/getdown/unix/images/lesson2/UnixDirectoryTree.png)
        * [Unix](http://www.cs.miami.edu/~geoff/Courses/CSC322-11S/Content/UNIXUse/Pictures/Hierarchy.GIF)



## User profile and avatars

* User profile: another form of user space
* May represent you using an avatar
    * From Sanskrit *avatāra*
    * In Hinduism, a deity (e.g., Vishnu) incarnated on Earth

* [Second Life](http://secondlife.com/), 2003

> The proliferation of *avatar*’s second meaning [in digital culture] can be traced to Second Life, a multiplayer online virtual world, where players fashion their own online personae called *avatars*. {% cite britt_language:_2008 --file 12-domain-2-user %}

* Other places you may find avatars
    - Blog comment threads
        + [Gravatar](https://en.gravatar.com/)
    - Customer service chat
    - Video games
        + [Maze War](http://en.wikipedia.org/wiki/Maze_War), 1974
        + Xbox console et al.

* 2009 film *[Avatar](http://www.avatarmovie.com/index.html)*

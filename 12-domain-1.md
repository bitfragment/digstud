---
title:        Domain
subtitle:     
version:      $version$
embed-vcs:    true
date:         $date$
description:  Course notes on the topic 'domain'
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
created:      2014-10-02
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

{% bibliography --file 12-domain-1 %}


## User login

* A "login" is the act or procesure of "logging in" or "loggin on" to a computer system
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

* Accounts in banking
    - *Not* a physical space set aside exclusively for your use
        + Contrast with safe deposit box
    - An abstraction or virtual space containing your assets

* An account is defined by:
    1. A configuration of access privileges, for access to computing resources
    2. A demarcation and assignment of virtual space in memory, for the storage and manipulation of data objects: the **home directory**



## Home directory

* Tree structure
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

<!-- 
Leave these to elaborate in topic 'User'
Continue with 1-day overviews of Network and Game
...and elaborate each in 

## Session (a temporal concept)

* A *session* begins at login and ends (usually) at logout

## From mainframe computing to the time-sharing OS

* (user space vs root) v kernel space
* permissions
 -->

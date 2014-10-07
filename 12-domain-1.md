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



## Abstract concept of network

* A concept of space defined not by boundaries as much as by *relations*
* Generic elements of a network are often called *nodes*, especially in telecommunications and computing
* Often does not have an *obvious* single center, though it will almost always include *clusters*

* "Networking": an adaptation to describe a social process ([example](http://www.atariarchives.org/deli/computer_networking1.jpg))



## Networked computing

* A *network* includes any two or more individual computer systems connected by a telecommunications link
* The telecommunications link may be a "tube" (hardware wire or cable), or a radio wave (transmitted and received by other hardware components)
* When the two or more systems occupy the same relatively local space (for example, a company office or a college campus), we call the network a Local Area Network (LAN)
* When the two or more systems are located on separate Local Area Networks, they may be linked by the Internet, a "ubiquitous" network-of-networks



## Prehistory of today's *ubiquitous* networked computing

* Earliest commercial telecommunications infrastructure: telegraph and telephone wires
* Earliest form of remote (non-LAN) desktop PC networking: via telephone lines, using an [acoustic coupler modem](http://en.wikipedia.org/wiki/Acoustic_coupler)



## Representations of networked computing

* Focus is not on individual nodes, but on *relations* between nodes
    - [Example](http://cdn3.computerworlduk.com/cmsdata/news/3246271/networking_iStock_000007517489Small.jpg)
    - [Example](http://www.12ahead.com/sites/default/files/styles/article_top_image/public/network.computer.300.fotolia.jpg?itok=t8ZFJQDx)

* Often represented as "overlay" on geographic space
    - [Example](http://thumbs.dreamstime.com/z/worldwide-computer-network-23344093.jpg)
    - [Example](https://sharmainemercado04.files.wordpress.com/2013/02/computer-network-technology.jpg?w=1200)


* Representations of the Internet often include image of globe/planet
    - [Example](http://photo.elsoar.com/wp-content/images/Laptops-and-earth-globe-computer-network.jpg)
    - [Example](http://telecomsolutions4u.co.uk/images/it.jpg)
    - [Example](http://www.freestockphotos.name/wallpaper-original/wallpapers/systems-internet-connectivity-to-download-5722.jpg)
* Sometimes that globe itself is imagined as a network you can plug into
    - [Example](http://www.danpontefract.com/wp-content/uploads/2014/05/internet2.jpg)
    - [Example](http://www.xpertcomputers.com.au/images/network-consultancy.jpg)

* [The Opte Project](http://dev2.opte.org/)
    - [Internet in 2003](http://dev2.opte.org/wp-content/uploads/2014/04/about-img-2.png)
    - [Internet in 2010](http://dev2.opte.org/wp-content/uploads/2014/04/home-page-pic.png)



## Layered domains

* Your user account is a "small" domain, which you log into
* Your user account grants you access to computing resources like processing time and storage space for your files
* It also serves as a portal to a larger domain: a LAN
* And also as a portal to an even larger domain: the Internet



## Game as constraint

* Also a representation of space, a virtual space
* Whereas a network is often imagined as boundless, a game is embraced as a system of constraint: that's often precisely why we enjoy it
* A game represents constrained choices for a human player's avatar
    - For many of us, often more constrained than many of even our most quotidian life choices: for example, what to eat for lunch
* Example: tic-tac-toe
    - Nine possibilities for placing your mark, from the start
    - Limited number of combinations of marks
    - Limited number of possible outcomes

* *All* games are systems of constraint
* Computer games (video games) are *programmed*
* The human player is less free to break the rules than she or he is in games played outside simulated environments



## Early computer games

### Graphical (video) games

* *Spacewar!* (1962)

### Text ("adventure") games

 * Terminal-based
 * Sometimes incorporated "graphics" composed with ASCII characters, rather than painted with screen pixels
 * Narrative form: an environment is described, choices are offered
 * Very explicitly algorithmic: if choice A, consequence B
 * Early examples
     - Colossal Cave Adventure, 1976
     - Zork (1977)



## Constraint

* Paradigmatic form of a programmed game: the maze
* Maze as map of programmed space

* Programming as determination of outcomes
* Algorithmic expression of "choice"



## Mass-produced consumer games: history

* "Primitive" games, extreme constraint
* Often only one or two courses of action
    1. Move an avatar through a representation of space
    2. Make or cause impact with objects

### Mimicry of sports pastimes

* Pong (1972)
* Breakout (1976)

### Fictional worlds and scenarios

* Space Invaders (1978)
* Asteroids (1979)



## Evolution of visual representation of space of constraint

1. "Flat" (two-dimensional), with player avatar at center
1. Three-dimensional, depicted from point of view of player avatar
    * Mid-1980s: exploration of "3D" or first-person navigational perspectives
        - Maze War (1985)
    * Early 1990s: developed into later generation of games, "first person," usually shooter
        - Depicted space primarily or exclusively from player's subjective POV
        - Map overlay as secondary feature
        - General increase in graphical detail and speed (hardware advances)
        - Construction of objects: polygons (3D)
        - Outdoor landscapes
        - Vertical navigation: moving up and down in space
        - Expansion of navigable space for avatar ("rails" vs. roaming)



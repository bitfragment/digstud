---
title:        Network
subtitle:     
version:      $version$
embed-vcs:    true
date:         $date$
description:  Course notes on the 'domain' subtopic 'network'
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
created:      2014-10-14
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

{% bibliography --file 12-domain-3-net %}



## Graph

* A mathematical representation of objects and links, which models *relation*
* L. *graphicus* < *γραϕικός* < *γραϕή*, drawing or writing
* When you draw or write, you are linking points in space
* Any two points can be connected



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

* Telecommunication: τῆλε afar, far off, distant
* Communication at a distance

* Optical telegraphy or semaphore
* Smoke signals and fire beacons
    - Homer, *Iliad* book 18, ca. 1240-1260 BC: "Like the beacons that one by one flare out at sunset from an island besieged by an enemy, its city cloaked all day by smoke rising to high heaven, for whose safety men fought from the battlements all day in bitter conflict; like those beacons, whose light shines out on high for all their neighbours to see, in hopes they might send their ships to the rescue..."
    - Aeschylus, *Agamemnon*, ca. 458 BC: "I’m still looking for that signal flare, the fiery blaze from Troy, announcing it’s been taken. These are my instructions from the queen."
* Buildings: spotter huts, lighthouses
* Claude Chappe's semaphore, France, 1790s
    - Military communication system for French army and government
    - Towers topped with bar structures that could be seen from a distance
    - Could be arranged in various shapes to transmit messages

* Semaphore replaced by telegraph systems beginning in the 1830s
* Then by telephone systems beginning in the 1870s
* Followed railroad construction
* Infrastructure buried underground in cities like New York, after the 1888 blizzard
* Cables run under the Atlantic Ocean, then other major bodies of water

* ARPANET, predecessor of Internet was built over and around telephone infrastructure, starting in the late 1960s

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



## How the Internet works

### Three kinds of networks

1. Centralized
2. Decentralized
3. Distributed

* U.S. planning for surviving a Soviet nuclear strike
* How to ensure that as much telecommunication infrastructure as possible could survive an attack, enabling the U.S. to respond?

* A *centralized* network has one single hub. If that hub is destroyed, so is the network
* A *decentralized* network has mutiple hubs. Destruction of a hub destroyed a subnetwork
* A *distributed* network has no hubs. Nodes are connected to each other by multiple channels
    - If one node is destroyed, there is always another path

### Packet-switching

* Each item of data (document, image) divided up into multiple "packets" and transmitted separately along different paths
* Reassembled at destination
* Efficient: allowed for all paths to be used simultaneously, for multiple messages
* Could survive destruction of nodes of the network: if a packet encountered an obstacle, it could be routed around it

* [National Physical Laboratory: The Story of Packet Switching](http://www.youtube.com/watch?v=tT4AaelwvV4)
    * Analogy: photocopying one page of the Bible at a time and mailing them to someone else, who uses page numbers to reassemble it

### Namespaces

#### IP (Internet Protocol) address

* Serves as an identifier for the point of connection of any device to the Internet
* Laptop, smart phone, smart toaster, etc.
* [What is my IP?](https://www.google.com/search?q=what%20is%20my%20IP%20address)
* [Trace My IP](http://www.tracemyip.org)

* Because an IP address encodes the connection point of any device to the internet, it provides information about your geographic location, at least in relation to telecommunications hardware
* It's nearly impossible for an unskilled person to successfully obscure that information
* That information can often be narrowed to a specific physical location, especially with a stationary device (e.g., a home desktop computer)

* An IP address is a 32-bit number represented in decimal notation for human-readability 
* Most of us don't normally encounter numeric IP addresses
* But we do deal with the linguistic layer added "on top of" the IP address system, to make it more convenient for us to use


#### DNS (Domain Name System)

* You can enter an IP address into a browser window (e.g., [http://146.186.15.17](http://146.186.15.17)) — but why would you?
* DNS is a *translation* allowing humans to use easily memorized units of human language, instead of numbers

* Something or someone has to translate the human language you type into the browser bar into numerical IP addresses: the DNS server
    * A computer whose job is to translate human language into numerical addresses
    * Like a phone book/ contact directory: you submit a name, get a contact number and/or address in response

* Domain names have a syntax (like other units of human language)
* The part you're most familiar with is the **top-level domain**: e.g., `.com`; `.org`, `.edu`, `.net`, `.gov`


##### Domain "hacks"

Creative linguistic "abuse" of the top-level domain, especially of [country code domains](http://en.wikipedia.org/wiki/Country_code_top-level_domain)

* [The Weird World of Country-Specific Web Domains](http://mentalfloss.com/article/30583/weird-world-country-specific-web-domains)

* Examples:
    - [`instagr.am`](http://instagr.am)
    - [`bit.ly`](http://bit.ly)



## The World Wide Web (WWW)

One domain of the Internet, not its entirety

### History of the Web browser

* [WorldWideWeb](http://en.wikipedia.org/wiki/WorldWideWeb), 1990
* [Erwise](http://en.wikipedia.org/wiki/Erwise), 1992
* [ViolaWWW](http://en.wikipedia.org/wiki/ViolaWWW), 1992
* [Lynx](https://en.wikipedia.org/wiki/Lynx_(web_browser)), 1992
* [Cello](http://en.wikipedia.org/wiki/Cello_(web_browser)), 1993

* [Mosaic](http://en.wikipedia.org/wiki/Mosaic_(web_browser)), 1993

> ...in the 18 months since it was released, Mosaic has incited a rush of excitement and commercial energy unprecedented in the history of the Net. {% cite wolfe_second_1994 --file 12-domain-3-net %}

* [Netscape Navigator](https://en.wikipedia.org/wiki/Netscape_Navigator), 1994
* [Microsoft Internet Explorer](https://en.wikipedia.org/wiki/Internet_Explorer), 1995
* [Apple Safari](https://en.wikipedia.org/wiki/Safari_(web_browser)), 2003
* [Mozilla Firefox](https://en.wikipedia.org/wiki/Firefox), 2004
* [Google Chrome](https://en.wikipedia.org/wiki/Google_Chrome), 2003

### Browser emulation (in a browser!)

[Deja Vu: (re-)creating web history](http://www.dejavu.org/)

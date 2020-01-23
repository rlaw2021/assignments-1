**CMSI 355** Networks, Spring 2020

# Assignment 0204
This first assignment is all about knowing your way around the network, particularly the parts that most users never see.

## Background Reading
Most of the information needed can be found in the [Internet Basics](https://cs.lmu.edu/~ray/notes/introinternet/) page from Dr. Toal’s website. Not included in this page is information on _arp_, the Address Resolution Protocol command. There’s a bunch of documentation available on the web for this, though at varying levels of detail. [This one](https://www.geeksforgeeks.org/arp-command-in-linux-with-examples/) is example-oriented and is likely the best fit for what we’re doing, but don’t hesitate to look for other sources if you want more detail.

Deeper background and details can be found in Chapters 20, 21, 23, and 26 of the Comer book (chapter 27 if you are on the 5th edition). Don’t be alarmed that we jumped from Chapter 3 to Chapter 20—there are whole sections on data communication basics and hardware-level network technologies that are elided for this course.

## For Submission: A Network Exploration Log and Map
Getting to know a network at a technical level for the first time feels (to me) a lot like pioneering exploration: you encounter strange new names and places, make discoveries about how information gets around, and gain some insight on how environments that you take for granted are actually set up. This assignment adapts this “exploration theme” as a way for you to introduce yourself to networks by having you look around the very networks that you use frequently.

### Step 1: Explore and Record
For the following network environments…
* LMU
* Private network outside LMU (apartment, office [when appropriate], house)
* Public network (coffee shop, shopping area, restaurant)

…and on at least _two_ distinct occasions per environment (“distinct” meaning that you leave/disconnect from that environment at least once between sessions), perform the following explorations:
1. Note your computer’s IP address, subnet mask, router, and domain name server(s)
2. Examine your computer’s full routing table
3. Use _arp_ to discover hosts that are on the same network
4. Use _ping_ to make contact with:
    * A host you discovered via _arp_
    * The default router
    * One of your domain name servers
    * www.lmu.edu
    * A host on the Internet (most likely a website, but for more variety, see if you can find a different kind of public host, such as a game server, mail server, chat server, or cloud storage)
5. Use _traceroute_ to discover the path taken to these same hosts
6. For www.lmu.edu and the chosen Internet host, use _dig_ to discover their IP addresses
7. Use _nmap_ to see what ports are open on these hosts
8. Use _nmap_ to see what ports are open on one of the intermediate “stops” discovered by _traceroute_ to any host outside of your network

Take screenshots of each of these activities and look for what’s common or consistent and what changes either across networks or across different sessions. Take note of when an operation fails as well.

### Step 2: Journal/Log
Gather these screenshots and provide commentary on them to form a coherent “explorer’s log” of sorts, to serve as a record of your explorations and discoveries.

### Step 3: Map
Based on the information you gather, try to sketch out a “map” of the networks and hosts that you explored. Where are they connected? What do the IP addresses in each environment look like? How do each of them get to www.lmu.edu and your chosen Internet host?

Think of this map as similar to one that early seafarers and explorers might have drawn: admittedly just a small part of the world (Internet), but as accurate and grounded as you can figure, based on the commands that you used.

### Optional: Work with a Friend or Classmate
Embarking on this exploration with a friend or classmate can give you some additional insight on how different computers on the same network are set up and may feel more comfortable when doing an _nmap_ (i.e., so that you aren’t doing _nmap_ on some random person’s computer—it’s still a pretty harmless exercise but you may still feel more comfortable if you’re _nmap_-ing somewhat that you know). However, if doing this with a classmate, each of you must still submit individual, distinct logs and maps: no sharing of work or screenshots.

### Overall: Imagine
Add a dash of fancy and imagination to your explorations by giving your log and map a fanciful theme that befits an exploration. Examples include:
* A starship captain’s log and charts
* A fantasy world such as Westeros or Middle Earth
* A certain popular monster game with its many regions and leagues
* Alternate dimensions or universes

In a way, you _are_ playing the role of an explorer, and the amazing thing is that you will be encountering places and paths that are all around us and yet are virtually unseen by nearly everyone, except at the very surface where websites and applications dwell.

### How to Turn it In
* Commit your journal/log to your allocated repository as a [Markdown](https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax) file. Make sure to embed your screenshots in this file alongside your fanciful (but technically accurate!) commentary. Call this file _log.md_.
* Your map may use any visual medium, ranging from something that is legibly hand-drawn then scanned/photographed to something made with a drawing tool—whichever approach you choose, upload the final result to the allocated repository as well. Name this file _map.*_ where _*_ indicates the format of the map file (e.g., _map.pdf_, _map.jpg_, etc.).

## Specific Point Allocations
This assignment covers outcomes _1a_–_1c_ and _2a_ as described in the [syllabus](http://dondi.lmu.build/spring2020/cmsi355/cmsi355-spring2020-syllabus.pdf).

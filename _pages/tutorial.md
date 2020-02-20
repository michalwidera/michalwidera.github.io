---
layout: single
permalink: /tutorial/
title: "Tutorial"
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/IMG_0758.JPG
  caption: "Photo credit: Tomasz Widera"
excerpt: "RetractorDB is the open source time series database"
toc: true
toc_sticky: false
---

Jump Start
==========
This is first and fast use case. Use tmux for switching tasks. There is a sequence of commands under Linux shell  that compiles example query, starts query processor and shows results.

```
sudo apt-get -y install gcc cmake libboost-all-dev make build-essential tmux
git clone https://github.com/michalwidera/retractordb.git
cd retractordb
cmake CMakeLists.txt; make
./build/xcompiler -q test/query-lnx.txt
tmux
./build/xabracadabra
[ctrl+B %]
./build/xqry -d
./build/xqry -s str1
[ctrl+B "]
./build/xqry -s str2
```

Video Tutorials
===============

Here you can find some video tutorials about RetractorDB Time Series Database system. I suggest to start from Session Record. Math basis are hard to understand for start but at the end everyone who intends to use that system should touch this. Apologies for low quality of these tutorials but this is only a side job for me. I did my best to spread that idea. Hope it will be enough.

Session Record
--------------

This is record of my session with computer. This takes about 18 minutes of presentation how acutually system works and how I handle with it. This presentation should go at first. Because there is no math jargon and we can see real data flowing and processing. I'm strongly suggest to start from this point. Note: you require some additional programs installed like: graphviz, feh, tmux. Use apt get install to get them.

{% include video id="I-nd5m7KSK4" provider="youtube" %}

Query Language
--------------

This presentation covers area of basic implemented query language. This is mandatory to see if we want to start coding and using this system.  

{% include video id="opVlhm-K5Mw" provider="youtube" %}

Operator Mechanics
------------------

Operator mechanics is presentation that try to show how different operators from introduced algebra works without mathematical jargon. Is it still quite hard to understand but I did my best. Hope this effort will be helpful.

{% include video id="fRW0sg9EgVM" provider="youtube" %}

Math Basics
-----------

This presentation show math basics required to undersand core behaviour of algebraic operators used in this system. This is quite hard to adapt. I suggest to skip this and return to this data at the end of course.

{% include video id="McT_HoBElCM" provider="youtube" %}

Papers
======

M.Widera. Deterministic method of data sequence processing. Annales Universitatis Mariae Curie-Skłodowska, Sectio AI, Informatica, Vol. 4 (2006), pages 314-331  [Link][det-method]

A. S. Fraenkel. The bracket function and complementary sets of integers. Canad. J.Math, 21:6–27, 1969. [Link][fraenkel]

S. Beatty. Problem 3173. Amer. Math. Monthly, 33:159, 1926.

[det-method]: https://journals.umcs.pl/ai/article/view/3066/2262
[fraenkel]: https://www.cambridge.org/core/journals/canadian-journal-of-mathematics/article/bracket-function-and-complementary-sets-of-integers/923DC20720CE446932EDBED7F348DF65

---
layout: post
title: Viper - Python on bare metal
---

>The [Hackend Project](http://deepakkarki.github.io/blog/2015/08/08/The-Hackend-Project/) - Week 1

For my very first "Hackend" I combined two of my most favourite things - Embedded systems and Python! This weekend I dived through [VIPER](http://www.viperize.it/) - Viper is Python Embedded in Realtime (A funky recursive acronym).

<!--more-->

#What is it?
Viper is a suite of software components that enable you, the developer to quickly develop embedded systems and IoT prototypes using Python. While it is surprising to find someone coding a micro-controller in python, they have really done a great job - seemingly better than earlier efforts such as [Micro Python](https://github.com/micropython/micropython) and [PyMite](https://github.com/jsnyder/python-on-a-chip). The system is portable - works seamlessly on ARM M0-M4 MCUs and easily portable across most other MCUs. It's extremely easy to get started -

* Download the browser based IDE for your OS.
* Open the IDE and connect the board - My Arduino Due automatically got listed.
* Burn the Viper VM (one of the components that make up the suite) onto the target board.
* Clone any of the available examples and execute them on your board.

![Viper IDE UI](https://lh3.googleusercontent.com/GXxFENWTcnSOeJIpAlFMRqOEqwr1ZUbqg4JAFkdmjQU=w2560-h1406-no "Viper IDE")

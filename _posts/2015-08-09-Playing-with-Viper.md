---
layout: post
title: Viper - Python on bare metal
---

<div class="message">
The <a href="http://deepakkarki.github.io/blog/2015/08/08/The-Hackend-Project/">Hackend Project</a> - Week 1
</div>

For my very first "Hackend" I combined two of my most favourite things - Embedded systems and Python! This weekend I dived through [VIPER](http://www.viperize.it/) - Viper is Python Embedded in Realtime (A funky recursive acronym).

<!--more-->

#What is it?
Viper is a suite of software components that enable you, the developer to quickly develop embedded systems and IoT prototypes using Python. While it is surprising to find someone coding a micro-controller in python, they have really done a great job - seemingly better than earlier efforts such as [Micro Python](https://github.com/micropython/micropython) and [PyMite](https://github.com/jsnyder/python-on-a-chip). The system is portable - works seamlessly on ARM M0-M4 MCUs and easily portable across most other MCUs. It's extremely easy to get started -

* Download the browser based IDE for your OS.
* Open the IDE and connect the board - My Arduino Due automatically got listed.
* Burn the Viper VM (one of the components that make up the suite) onto the target board.
* Clone any of the available examples and execute them on your board.

![Viper IDE UI](https://lh3.googleusercontent.com/GXxFENWTcnSOeJIpAlFMRqOEqwr1ZUbqg4JAFkdmjQU=w2560-h1406-no "Viper IDE")

#How it works?
It's really intriguing how someone could support a huge subset of python on a micro-controller system. Looking into their system design and code base, you can easily tell the effort that has gone behind this. Looking at it from an engineering perspective, there are two key components that make the magic happen -

1. The compiler that runs on the PC
2. The VM that runs on the embedded system.

The compiler is written in python - and compiles the python (that you intend to execute on your micro-controller) into efficient byte code. This byte code is then streamed to to the micro-controller running the viper VM. The viper VM is built over ChibiOS (A realtime embedded OS) and is written in C. One thing I liked about this is the support for threads (priority based and premptive) - built over the ChibiOS threading system.

#What I learnt
To be honest, I just got a high level overview of how things worked. I went through the source code of the components which run on the PC side, viz. the IDE and python byte code compiler, nothing too convoluted here. What I really wanted to do was play with the source code of the VM - but alas, that was not to be! The current code documentation is quite abysmal and good just for reference, I'd have to spend over a week before I figure *what is what* in the source code!

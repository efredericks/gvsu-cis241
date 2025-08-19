---
marp: true
theme: marp-black-white
# _class: invert
paginate: true
header: CIS241 // Erik Fredericks // Fall 2025
size: 4K
---

# CIS241

## System-Level Programming and Utilities

Erik Fredericks, frederer@gvsu.edu
Fall 2025

> Based on material provided by Erin Carrier and Austin Ferguson

---

# The Plan (approximately)

First half: Linux
Second half: C

<style scoped>
    img {position:absolute;top:20px;right:20px; }
</style>
<img src="https://i.ytimg.com/vi/a6iW-8xPw3k/mqdefault.jpg" />

---

# About Me (or, the relevant things)

## Office: MAK D2-235

**Office Hours**: TR, X-Ypm

## Discord: 

Join the `#241` channel for async help

- I'll also keep an eye on the CIS Discord as well

![bg right:50% w:500](img/ErikFredericks.jpg)

---

# Also

I've completely dumped Windows for Linux

* Arch (EndeavorOS) at home
* pop_os! (Debian) on this machine

## Why?

Too much baggage to unpack without a therapist, but the Windows Recall thing was the final straw

## What does this mean for me?

I don't have a Windows or a Mac to fix your issues for you...


---

# Lab Environments

EOS is where all your assignments will be tested on, so **make sure it works there before submitting anything**

All material can be tested on your own computers

* Windows: WSL!

* Linux: Linux!

* Mac: Also Linux!

---

# Syllabus Time

Important things:

## Grading

## Late Policy

Assignments are due **on time**.  
You can turn it in up to **three days** late - it is 10% off each day and a 0 afterwards. 
  * If there are extenuating circumstances talk to me **early** - if you ask me the night something is due I will most likely say no.

---

# AI Use

My preference is for you not to use it for this class.  Try things first, watch how things break, **fail often**.  Learn from your mistakes - that's how learning works. 

However, I realize it can be helpful at times.  I ask that you don't completely copy/paste what it gives you and that you understand how it is helping.  Note that if I ask you to explain your code and you can't, then it becomes an academic misconduct violation.

If you become one of those coders in industry who can't function without an AI helper then you are pretty much useless.  Use it to clarify things, not to do your job.



---

# Remote Access

## SSH - Secure Shell

What is a shell?

What shell am I using?

```
echo $0
```

`$0` --> variable for the name of the shell

SSH is how you can access a remote shell

Try it!  *Or else!*

* Or else what?
    * Or else you won't be able to do your homework and pass the course!

---

<style scoped>>
  h1 {
    color: #fff;
  }
</style>

# The Bigger Picture

![Hackers bg](https://editorial.rottentomatoes.com/wp-content/uploads/2020/09/Hackers_Anniversary_Rep.jpg)

---

# The Bigger Picture (Linux edition)

## Who cares?

1. For one, think of how *cool* you'll look using the terminal in front of friends and family.
    * See previous slide

2. Access remote systems
    * Web servers, high-performance computing environments, cloud systems, etc.

3. Automate, automate, automate
    * Automate all the things (Windows included!)
       * Windows ... *how?!?!!*

---

# The Bigger Picture (C Edition)

C is *gross* - shouldn't we be using Rust?  Or Python or Java?!?!

- Does anybody know why C still exists?

<!--
* Better memory management - you know exactly what is being used
* Still used in embedded systems
* More importantly - still the leader in safety-critical programming (e.g., automotive, flight)
-->
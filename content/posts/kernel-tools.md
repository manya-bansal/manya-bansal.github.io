---
title: How to use common debugging hardware and traps to build tiny, effective kernel-level dynamic checkers
date : 2000-01-01
categories: 
mathjax : true
authors : ["Zachary Yedidia,", "Dawson Engler,", "Akshay Srivatsan,", "Manya Bansal."]
notes : "Under Submission"
---

**Abstract.** This paper shows how to use common debugging hardware support for single-step execution to make writing powerful dynamic tools easy --- often a few hundred lines of code. Unlike most current tools, these work well on kernel code. This novel ease makes it correspondingly easy to quickly build novel tools. We present a number of unique tools based on this approach to precisely and immediately find kernel bugs extremely difficult to track down without them.

We demonstrate our approach on both ARM and RISC-V hardware. Our hope is that after reading this paper a competent system implementor could fairly quickly write a few hundred lines of code and find errors in their system or, even better, show their absence. This confidence comes in part because over the past couple of years we have successfully shown roughly a hundred novice system builders how to do so.

*Email me (manya227@stanford.edu) for the pre-print.*

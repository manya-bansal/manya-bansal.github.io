---
title: "Mosaic: An Interoperable Compiler for Tensor Algebra"
categories: 
date : 2000-01-02
mathjax : true
authors : ["Manya Bansal,", "Olivia Hsu,", "Kunle Olukotun,", "Fredrik Kjolstad."]
notes : "Under Submission"
---

We introduce Mosaic, a sparse tensor algebra compiler that can bind tensor (sub-)expressions to external
functions of other tensor algebra libraries or compilers. Users can extend Mosaic by adding new functions and
can bind a sub-computation to a function using a scheduling API. Mosaic substitutes the bound
(sub-)expressions with the specified function call and automatically fills in the rest of the unbound code using
a default code generator. Mosaic also has a search system that can automatically map an expression to a set
of registered external functions. Both the explicit binding and automatic search are verified by Mosaic. We
demonstrate the benefits of our approach by showing that calling hand-written CPU and specialized hardware
functions can provide speedup of up to 206$\times$ and 173$\times$, respectively, over a homogeneous compiler. Mosaic’s
external function interface is simple and general. Currently, 38 external functions have been added to Mosaic,
with each addition averaging 20 lines of C++ code.

*Email me (manya227@stanford.edu) for the pre-print.*

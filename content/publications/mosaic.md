---
title: "Mosaic: An Interoperable Compiler for Tensor Algebra"
categories: 
date: 2023-06-01
mathjax: true
authors: ["Manya Bansal", "Olivia Hsu", "Kunle Olukotun", "Fredrik Kjolstad"]
notes: "ACM SIGPLAN Conference on Programming Language Design and Implementation (PLDI), June 2023"
award: "Distinguished Paper Award"
pdf_link: "https://dl.acm.org/doi/10.1145/3591236"
draft: false
---

[View PDF](../../papers/pldi23main-p107-final.pdf)

**Abstract.** We introduce Mosaic, a sparse tensor algebra compiler that can bind tensor expressions to external functions of other tensor algebra libraries and compilers. Users can extend Mosaic by adding new functions and bind a sub-expression to a function using a scheduling API. Mosaic substitutes the bound sub-expressions with calls to the external functions and automatically generates the remaining code using a default code generator. As the generated code is fused by default, users can productively leverage both fusion and calls to specialized functions within the same compiler. We demonstrate the benefits of our dual approach by showing that calling hand-written CPU and specialized hardware functions can provide speedups of up to $206\times$ against fused code in some cases, while generating fused code can provide speedups of up to $3.57\times$ against code that calls external functions in other cases. Mosaic also offers a search system that can automatically map an expression to a set of registered external functions. Both the explicit binding and automatic search are verified by Mosaic. Additionally, the interface for adding new external functions is simple and general. Currently, 38 external functions have been added to Mosaic, with each addition averaging 20 lines of code.

**(Distinguished Paper Award, PLDI'23)**
# webdata

Discussion of [numeric computing/data science](#introduction) on the web (JavaScript)

### Discussion Topics

- [64-bit integers](https://github.com/codeforscience/webdata/issues/1)
- [Memory efficiency: Typed Objects/Value Types](https://github.com/codeforscience/webdata/issues/3)
- [Concurrent data processing](https://github.com/codeforscience/webdata/issues/4)
- [File and network I/O](https://github.com/codeforscience/webdata/issues/5)
- [Native code (WebAssembly/Node native addons (for porting/running C++ to JS))](https://github.com/codeforscience/webdata/issues/6)
- [GPU compute](https://github.com/codeforscience/webdata/issues/8)
- [N-dimensional arrays](https://github.com/codeforscience/webdata/issues/7)

Have another one? Open an issue to discuss!

### Introduction

In the field of data science there is a sub-category called numeric computing. Data science itself encompasses everything from finding data, cleaning data, analyzing data, statistically modelling data, etc.

Numeric computing refers specifically to any aspect of those steps which requires loading and working with numeric data. Often times this data can be very large, very precise, or highly dimensional.

The three most popular languages for numeric computing today are C/C++, Python and R. I recommend watching the [Python data bikeshed](https://www.youtube.com/watch?v=RTiAMB2tQjo) for a great overview of the kinds of tools available to Python data developers. Check out this [CRAN list](https://cran.r-project.org/web/views/NumericalMathematics.html) for a sampling of the kinds of packages people are writing in R.

In Python people have written tools like Numpy and Pandas for dealing with multidimensional data. R has a built in datatype called the DataFrame (among others) that help with this. Also in both Python and R usually the critical functionality is implemented in a lower level language, and a nice API is exposed to the high level language.

For many of these applications memory efficiency is very important. Being able to fit a dataset into RAM generally makes the programmers life a lot easier. For datasets that are too large to fit on one machine there are so-called 'out of core computing' approaches for using multiple computers to analyze a dataset.

JavaScript traditionally has not focused on letting the programmer control memory usage. However in recent years JavaScript has seen the introduction of things like Node.js Buffers and JavaScript Typed Arrays which allow for greater control over memory allocation than was possible previously.

There are a lot of missing things that JavaScript (and the rest of HTML5) don't yet have. The goal of this repository is to get discussion going about what things are most important, and how we can help get them standardized and implemented.

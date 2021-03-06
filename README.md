# The Data Science Toolkit
An (opinionated) set of tools and resources for the new data scientist. 

[![GitHub Follow](https://img.shields.io/github/followers/pete-lawson)](https://github.com/pete-lawson)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
## Table of Contents

1. [Motivation](#intro)
2. [Background Mathematics](#math)
4. [Programming](#programming)
5. [Visualization](#visualization)
6. [Tools](#tools)
7. [Reproducibility](#repro)


<a name="intro"/>

## Introduction
Data science encompasses multiple domains and requires expertise across those
domains. This enhancement of Drew Conway's Data Science Venn diagram by Stephan
Kolassa makes this point clear, visually depicting the need for expertise at the
intersection of communication, statistics, programming, and business. This guide
attempts to curate tools and resources across these domains to help guide new
data scientists.

<img src="https://github.com/pete-lawson/data-science-toolkit/blob/master/figures/data_scientist_venn_diagram.png" alt="Data Science Venn Diagram" width="500">

Source: [Stephan Kolassa - Stack Overflow](https://datascience.stackexchange.com/questions/2403/data-science-without-knowledge-of-a-specific-topic-is-it-worth-pursuing-as-a-ca)

### Why I Started This Guide
My brother is in the process of beginning a graduate program in data science,
and over the course of discussing what he needs to know before beginning, I
realized compiling it all into a living document makes more sense. This guide is
the result of that discussion, incorporating all of the tools and resources I
have found helpful over the course of a PhD in a data science related field. The
guide favors open tools, and the content supports rigor and reproducibility. This guide assumes minimal background knowledge in data science.

### How to Use This Guide
This guide is themed along major topics, such as background mathematics, programming, visualization, data science tools, and reproducible research. Each topic breaks down into subtopics, and each subtopic is ordered in ascending order of rigor. In this way, by moving deeper through the resources in a subtopic, it is possible to gain an increasingly deeper understanding of the subtopic. Entries with an asterisk (**&ast;**) are not openly accessible (generally a textbook without an open PDF) but have been included due to their perceived value. Hopefully in these cases you can find them through an academic library or through a friend. 

<a name="math"/>

## Mathematics

### Linear Algebra
* [Essence of Linear Algebra - 3Blue1Brown](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab): An indispensable short video series (the entire series is no more than two hours) that provides a deep intuition for the why of linear algebra using a geometric approach. Watch this video series to gain a better understanding of how linear algebra works using well animated concise videos. This video series is a necessary precursor to any subsequent resources on linear algebra.
* [Linear Algebra - Khan Academy](https://www.khanacademy.org/math/linear-algebra): Khan academy's linear algebra lessons are especially clear, and provide a nice intermediate introduction to linear algebra.
* [Linear Algebra - MIT Open Courseware](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/): Gilbert Strang's MIT course provides one of the most thorough, insightful, and charming introductions to linear algebra. This should be a necessary stop on your journey through data science if you have the time.
* [Linear Algebra - Jim Hefferson](http://joshua.smcvt.edu/linearalgebra/): An free linear algebra textbook that provides a uniquely clear introduction to linear algebra. 


### Statistics and Probability
#### Bayesian Inference
* [Probabilistic Programming and Bayesian Methods for Hackers](https://camdavidsonpilon.github.io/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/)
* [Think Bayes - Bayesian Statistics Made Simple](https://greenteapress.com/wp/think-bayes/) 
* [Statistical Rethinking](https://xcelab.net/rm/statistical-rethinking/)**&ast;**: The Bayesian stats book you wish you had during graduate school.
* [Bayesian Data Analysis](http://www.stat.columbia.edu/~gelman/book/): A rigorous introduction to applied Bayesian inference.
#### Machine Learning
* [An Introduction to Statistical Learning](http://faculty.marshall.usc.edu/gareth-james/ISL/)
* [The Elements of Statistical Learning](https://web.stanford.edu/~hastie/ElemStatLearn/): Intro to Statistical Learning (ISL)'s older sibling. Reviews the same concepts as ISL, but with significantly more rigor and depth. This is not easy reading, but is an excellent reference.
<a name="tools"/>


## Tools

### Versioning Control (Git/Github)

For its ubiquity I am focusing on Git and its counterpart for hosting Git repositories online, Github.  

* [Github for Poets](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV) is a quick, clear, and enthusiastic introduction to Git and Github. It uses a poem as a motivating example rather than code, so you won't get bogged down in technical particularities. Instead it delivers the basics of Git in a fun way. Great for someone who has never used versioning control before and needs a primer.


### Editors
Choosing the right editor and IDE (integrated development environment) are the first step into becoming a data science. Your editor is a deeply personnel choice (the ongoing flame war between the Emacs and Vim editors are evidence of this). For this guide I take the controversial position of advocating exclusively for Emacs as both editor and IDE (I did say this is an opinionated guide).

#### Vim
Wait? Didn't you just say you advocate exclusively for Emacs? So why are we talking about Vim? Bear with me, I'm getting there. Vim is a terminal based text modal editor. Modal means you switch between a command mode (for entering commands) and a text mode, for inputting text. Vim's main power lies in its keyboard shortcuts and powerful search and replace, which together allow you to program at lightning speed, as Vim's keybindings allow you to keep your hands on the home row of the keyboard. Vim is also fairly ubiquitous, you will find it, or its precursor VI, on almost every Unix based system. So no matter the system you are on you will have a powerful editor available to you. Vim keybindings are present in a number of common applications and services as well, such as Gmail and GitHub. So go learn it! 

If you have Vim installed, open up a terminal and run `vimtutor`. Vim's own tutorial is excellent, and well worth spending the time to go through. There are some other interactive tutorials however:

* [Vim Interactive Tutorial](https://www.openvim.com/) An interactive online Vim tutorial.
* [Vim Adventures*](https://vim-adventures.com/) A Zelda-like adventure, except you learn Vim by controlling your character using Vim keybindings! Fun, but only the first level is free.
#### Emacs
* [GNU Emacs](https://www.gnu.org/software/emacs/)
* [Evil Mode: Or, How I learned to Stop Worrying and Love Emacs](https://www.youtube.com/watch?v=JWD1Fpdd4Pc) This a motivating perspective from a software engineer who switched from Vim to Emacs, and mirrors my own philosophy, which is Vim is a better editor, and Emacs is a better everything else, so why not combine them? Which brings me to my next recommendation:
* [Spacemacs](https://www.spacemacs.org/) Spacemacs is a community-driven Emacs distribution, pre-configured with a number of powerful packages and tools. With Evil mode it provides deep integration of Vim keybindings and modal editing into Emacs. Try starting with Spacemacs, but don't use it as a crutch. Think of it as a preview of all the Emacs packages you may want to use. Eventually you will want to configure Emacs yourself, and you can use what you love in Spacemacs to guide your own configuration.
<a name="repro"/>

## Reproducibility

* [Cookiecutter](https://github.com/cookiecutter/cookiecutter) is a command-line utility that creates new boilerplate projects from cookiecutters (project templates). A project template comprises a directory skeleton with boilerplate code, plaintext documentation, and supporting files populated by a user-created template. Cookiecutters are language and domain agnostic; they can contain templates for any plaintext files, including, but not limited to, markdown READMEs, code scripts in any language, Makefiles for building a project, and requirements files for managing project dependencies. Cookiecutters are best used at the beginning of a data science project to encourage consistent documentation and meaningful project structure.

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>

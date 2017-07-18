# Resampling Statistics

### Notes and code to go along with *Resampling: The New Statistics* (1974) by Julian L. Simon

> An introduction to Statistics, Python and R using words you know to explain things you don't

This book was originally written in 1974 and reprinted due to dankness is one of the best introductions to statistical thinking. *Statistical thinking* meaning how we can comprehend information in a numerical way. The type of statistics this book introduces is referred to as Non-parametric Statistics which is a scary sounding term we can unpack. Non-parametric means that we aren't making assumptions about the thing that created the numbers and statistics means to use the numbers available to tell us things that we are interested in.

These notebooks, which are written in both Python and R programming languages, use examples given in *Resampling* to explain concepts in probability and statistics by parsing them into modern programming languages. These are ready for you to explore and then use to do cool stuff with numbers in the real world and like impress people and stuff. If you don't have any previous programming experience GTFO! JK, the idea is we are going to introduce fancy programming stuff along the way. As a statistician unlike the mythical Data Scientist, people won't expect you to know every minute detail about the programming language you work in. This book will try to give you an understanding of the basic tools and how to use them in human speak. This book will absolutely not debate best practices in jargony words because that is what ytl;dr posts on Stack Overflow are for. Here we will introduce
the thing, its name and why tf we'd even bother to mentioning it.

# Setup

### To run these notebooks on your own, you're going to need to do a couple computer type things first:

1. Get R and Python set up on your computer:

  This can be a huge pain if you have never done it before and will leave you wondering things like "what is a system path" and "heck this computer do wrong".
  Today to install Python or R most everyone would tell you to use something called Anaconda to which you say, "heck is Anaconda?"

  [Anaconda](https://www.continuum.io/downloads) is a package manager and general life saver when it comes to Python. Python is really good at being easy to understand every where except for when it comes to using these things called packages, which can absolutely suc. Packages are ways of sharing code for repetitive stuff so you don't have to write it ur self. `conda` is a command line part of Anaconda that makes managing Python (and R) wayy easy and it just works. All of the Python packages we will be using will be installed already when you install Anaconda and you only have to type one line to add all of the R packages.

  To install click on the anaconda hyper link and follow the [instructions](https://conda.io/docs/install/full.html) for your operating system. You know, that thing that makes your computer go bleep bloop.

2. Make sure `conda` is added to your system path:

  This is super important because when you go to this thing called the command line or terminal(which u will soon love and hate), you will want be able to access `conda` from any directory. This will only be possible if anaconda is on your path.

  To add Anaconda to your path, you have to find where the anaconda files were installed on your computer.

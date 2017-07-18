# Resampling Statistics

### Notes and code to go along with *Resampling: The New Statistics* (1974) by Julian L. Simon

> An introduction to Statistics, Python and R using words you know to explain things you don't

This book was originally written in 1974 and reprinted due to dankness is one of the best introductions to statistical thinking. *Statistical thinking* meaning how we can comprehend information in a numerical way. The type of statistics this book introduces is referred to as Non-parametric Statistics which is a scary sounding term we can unpack. Non-parametric means that we aren't making assumptions about the thing that created the numbers and statistics means to use the numbers available to tell us things that we are interested in.

These notebooks, which are written in both Python and R programming languages, use examples given in *Resampling* to explain concepts in probability and statistics by parsing them into modern programming languages. These are ready for you to explore and then use to do cool stuff with numbers in the real world and like impress people and stuff. If you don't have any previous programming experience GTFO! JK, the idea is we are going to introduce fancy programming stuff along the way. As a statistician unlike the mythical Data Scientist, people won't expect you to know every minute detail about the programming language you work in. This book will try to give you an understanding of the basic tools and how to use them in human speak. This book will absolutely not debate best practices in jargony words because that is what ytl;dr posts on Stack Overflow are for. Here we will introduce
the thing, its name and why tf we'd even bother to mentioning it.

# Setup (for if you want to run this code):

If you want to simply view these notebooks: you can view them on NB Viewer via the links above.

### To run these notebooks on your own, you're going to need to do a couple computer type things first:

1. Get R and Python set up on your computer:

  This can be a huge pain if you have never done it before and will leave you wondering things like "what is a system path" and "heck this computer do wrong".
  Today to install Python or R most everyone would tell you to use something called Anaconda to which you say, "heck is Anaconda?"

  [Anaconda](https://www.continuum.io/downloads) is a package manager and general life saver when it comes to Python. Python is really good at being easy to understand every where except for when it comes to using these things called packages, which can absolutely suc. Packages are ways of sharing code for repetitive stuff so you don't have to write it ur self. `conda` is a command line part of Anaconda that makes managing Python (and R) wayy easy and it just works. All of the Python packages we will be using will be installed already when you install Anaconda and you only have to type one line to add all of the R packages.

  To install click on the anaconda hyper link and follow the [instructions](https://conda.io/docs/install/full.html) for your operating system. You know, that thing that makes your computer go bleep bloop.

2. Make sure `conda` is added to your system path:

  This is super important because when you go to this thing called the command line or terminal(which u will soon love and hate), you will want be able to access `conda` from any directory. This will only be possible if anaconda is on your path.

  You can check this by typing `conda` into your terminal, if you see output that says the command wasn't recognized, you need to follow the instructions below. If you get an info sheet explaining stuff about anaconda you're gucci.

  To add Anaconda to your path, you have to find where the anaconda files were installed on your computer. If you have a Mac or Linux OS run: `export PATH=$HOME/anaconda/bin:$PATH`

3. Adding R to Anaconda:

  So Anaconda is cool because it can not only manage Python packages but also R packages. You can install r packages into your anaconda distribution by running the command:
  ```bash
  $ conda install -c r r-essentials
  ```
  To break this command down the first two words are really standard. `conda install <package-name>` will be the way to typically install a python package. The addition of the `-c r` is how `conda` knows to look for R packages to install and the `r-essentials` is a bundle of the R packages that you would probably use to do cool R stuff.

  **_Note_:**  This isn't the way people usually install R but it makes it wayy more convenient for the sake of this tutorial, you can figure out how to install R and use RStudio on ur own if you want cause I believe in you!

4. Once u got all this installed, download the notebooks fam:

  If you feelin like a pro and want to use git (assuming it's installed), `cd` into the directory you want the folder in and run:

  ```bash
  $ git clone https://github.com/rgalbo/ResamplingStatistics.git
  ```

  After this, you can download any updates to this repo by simply running `git pull` and the most recent files will be downloaded.

  If you have absolutely no idea what I just said, simply download the zip file of the project from [github](https://github.com/rgalbo/ResamplingStatistics) and unzip it.

5. Running the notebooks:

    Now you should be able to `cd` into the repository you just cloned or unzipped so your prompt looks like `username:~/.../ResamplingStatistics/notebooks$` and run the command `jupyter notebooks` which will spin up a local jupyter notebook server and open your browser to something that looks like this:

    ![jupyter notebook](http://jupyter.readthedocs.io/en/latest/_images/tryjupyter_file.png)

6. Using the notebooks:

  Simply click on the notebook that you want to get into and jump right in using <kbd>CTRL</kbd>+<kbd>Z</kbd> (or <kbd>CMD</kbd>+<kbd>Z</kbd> on Mac) to execute the cells in order.

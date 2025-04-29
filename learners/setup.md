---
title: Setup
---

## Overview

This lesson is designed to be run on a personal computer.
All of the software and data used in this lesson are freely available online,
and instructions on how to obtain them are provided below.

## Get Python

In this lesson, we will be using Python 3 with some of its most popular scientific libraries.
We are going to be using [Google Colab](https://colab.google/), a hosted Jupyter Notebook service
that requires no setup to use and provides free access to computing resources,
including GPUs and TPUs.

To get started, you just need to log in with a Google account and either click ["New Notebook"](https://colab.new/),
or launch the relevant template notebook from the list below.

### Course notebooks

In addition to the detailed notes here, we also provide template notebooks for you to launch in Google Colab.

#### Day 1 notebooks:

- [Introduction](https://colab.research.google.com/github/ARCTraining/swd1a-notebooks/blob/main/01-intro.ipynb)
- [Lists](https://colab.research.google.com/github/ARCTraining/swd1a-notebooks/blob/main/04-lists.ipynb)
- [Loops](https://colab.research.google.com/github/ARCTraining/swd1a-notebooks/blob/main/05-loops.ipynb)
- [Numpy](https://colab.research.google.com/github/ARCTraining/swd1a-notebooks/blob/main/02-numpy.ipynb)

#### Day 1 exercise:

- [Day 1 exercise](https://colab.research.google.com/github/ARCTraining/swd1a-notebooks/blob/main/list_loops_exercise.ipynb)

#### Day 2 notebooks:

- [Visualising data](https://colab.research.google.com/github/ARCTraining/swd1a-notebooks/blob/main/03-matplotlib.ipynb)
- [Analysing multiple files](https://colab.research.google.com/github/ARCTraining/swd1a-notebooks/blob/main/06-files.ipynb)
- [Making choices](https://colab.research.google.com/github/ARCTraining/swd1a-notebooks/blob/main/07-choices.ipynb)

#### How to use these notebooks

Note that links in these notes may be broken, please
refer back to these course notes for glossary terms etc.

#### Stop! When you see the header "solution"

When you read a challenge asking you to do something, don't read beyond the next header that reads "Solution". Insert a new code cell below the question and attempt to solve it yourself before reading on.

#### Remember to apply PRIMM

When you see a piece of code, remember:

1. Before you do anything else, **predict** what the output is going to be.
2. Then **run** it, and compare the output to your prediction.
3. You can begin to **investigate**, especially if your guess is way off - what information can you find in the notes, or online?
4. Once you've tried to understand how the code works, try to **modify** it and make some changes.
5. Then, you're ready to start **making** your own code!

We will mainly be cycling through stages 1 and 2, with some of the later stages coming in as you build more knowledge.

## Obtain lesson materials

There a few different ways of loading in the data.

### 1. Download it directly in Colab

In Colab, you can access the terminal of the remote machine by using `!` in front of Linux
bash commands. This means you can use the Linux command `wget` to download files from the internet.
This snippet is included in the relevant template notebook files linked above.

**Note: the file storage space on the remote machine you are using in Google Colab is not persistent:
the files and folders you upload/save will not still be there when you next log in. Please download
your work if you want to save it.**

#### Download files

```python=
# Download 2 files and store in the swc-python folder
!wget -P swc-python https://swcarpentry.github.io/python-novice-inflammation/data/python-novice-inflammation-data.zip 
!wget -P swc-python https://swcarpentry.github.io/python-novice-inflammation/files/code/python-novice-inflammation-code.zip
```

#### Unzip files

```python=
# Extract .zip files inside the folder swc-python/
!unzip /content/swc-python/python-novice-inflammation-code.zip -d /content/swc-python/
!unzip /content/swc-python/python-novice-inflammation-data.zip -d /content/swc-python/
```

### 2. Manual download

You can download the files and code directly to your machine:

1. Download [python-novice-inflammation-data.zip][zipfile1]
  and [python-novice-inflammation-code.zip][zipfile2].
2. Create a folder called `swc-python` on your Desktop.
3. Move downloaded files to `swc-python`.
4. Unzip the files.

You should see two folders called `data` and `code` in the `swc-python` directory on your
Desktop.

You can then use the files dialogue in the right hand panel of Colab to upload these files.

## After this course: install Python

When you are working on research coding, you will want to use Python from your local
machine. Here are some instructions for you to follow *after* this course, to set
up Python on your machine.

Although one can install a plain-vanilla Python and all required libraries by hand,
we recommend installing [Miniforge](https://conda-forge.org/download/), an open-source
installer. You can see a [quick start guide](https://kirenz.github.io/codelabs/codelabs/miniforge-setup/#0)
for using `conda` to run Python scripts. You can see the [Python docs](https://www.python.org/about/gettingstarted/)
here for more information.

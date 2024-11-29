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

To get started, you just need to log in with a Google account and click ["New Notebook"](https://colab.new/).

## Obtain lesson materials

There a few different ways of loading in the data.

### 1. Download it directly in Colab

In Colab, you can access the terminal of the remote machine by using `!` in front of Linux
bash commands. This means you can use the Linux command `wget` to download files from the internet.

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

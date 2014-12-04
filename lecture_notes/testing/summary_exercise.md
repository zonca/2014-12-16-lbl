---
layout: lesson
root: ../..
title: A Summary Exercise
---

## The Problem

In 2D we have two points (p1 and p2) which define a line segment. Additionally, there exists experimental data which can be anywhere on the domain. Find the data point which is closest to the line segment.

<img src="points.png" alt="Find the nearest point to the line segment."/>


## Starting Point

Here is some sample data to get you started:

<div class="in">
<pre>import numpy as np

p1 = np.array([0.0, 0.0])
p2 = np.array([1.0, 1.0])
data = np.array([[0.3, 0.6], [0.25, 0.5], [1.0, 0.75]])
</pre>
</div>

If you want to generate some random points you can use `np.random.random`. Here we generate 50x 2D points.

<div class="in">
<pre>import numpy as np

data = np.random.random((50,2))
</pre>
</div>

## Warning

**Warning** this problem requires you to be comfortable with geometry.
But I am not expecting you to code a good answer.
I choose this problem because it should be easy to come up
with tests.
If geometry is not your forte don't worry about the code
too much you can make an obvously wrong code or one that only works sometimes.
The important part of this exercise is to come up with tests.

## Outline

1.  Create a git repository on your machine and commit the code you write.
2.  Write tests in test_*.py file.
3.  Write a code to find the nearest point (it doesn't have to work) in a *.py file.
4.  Run nose.
5.  Create a github repository, add it as a remote to your local repo, and push your local repo.
6.  Get your partners code on your machine. Either:
    1.  Pick a partner, clone  your partner's Github repo.
    2.  Pick a partner, fork  your partner's Github repo, and clone the foked repo onto your machine.
7.  Write tests to break their code.

## Optional Command Line Arguments

Write your code so that it can be run from the command line.
It should take 4 floating points as arguments (x0, y0, x1, y1) and a 5th argument which is a datafile with the datapoints.

### Generating a data file

You can generate a data file with np.random.random and np.savetext.

<div class="in">
<pre>import numpy as np

data = np.random.random((50,2))
np.savetxt(filename, data)
</pre>
</div>

### Reading a data file

You can read your data file with np.loadtxt.

<div class="in">
<pre>import numpy as np

data = np.loadtxt(filename)
</pre>
</div>





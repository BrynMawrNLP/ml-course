---
layout: default
title: "Math Review & Numpy"
type: Lab
number: 01
active_tab: lab
release_date: 2023-09-04

---

<!-- Check whether the assignment is ready to release -->
{% capture today %}{{'now' | date: '%s'}}{% endcapture %}
{% capture release_date %}{{page.release_date | date: '%s'}}{% endcapture %}
{% if release_date > today %} 
<div class="alert alert-danger">
Warning: this assignment is out of date.  It may still need to be updated for this year's class.  Check with your instructor before you start working on this assignment.
</div>
{% endif %}
<!-- End of check whether the assignment is up to date -->


<!-- Check whether the assignment is up to date -->
<!--{% capture this_year %}{{'now' | date: '%Y'}}{% endcapture %}
{% capture due_year %}{{page.due_date | date: '%Y'}}{% endcapture %}
{% if this_year != due_year %} 
<div class="alert alert-danger">
Warning: this assignment is out of date.  It may still need to be updated for this year's class.  Check with your instructor before you start working on this assignment.
</div>
{% endif %}-->
<!-- End of check whether the assignment is up to date -->



{% if page.materials %}
<div class="alert alert-info">
You can download the materials for this assignment here:
<ul>
{% for item in page.materials %}
<li><a href="{{item.url}}">{{ item.name }}</a></li>
{% endfor %}
</ul>

</div>
{% endif %}





{{page.type}} {{page.number}}: {{page.title}}
=============================================================

## Objectives:

The main goals for this lab are:

1. Start getting familiar with numpy.
2. Brush up on relevant math (Linear Algebra, Calculus, Probabiltiy).


Make sure to write down your answers below. In future labs, the TAs or Instructor
will check your answers. Whenever you see **TODO**, that means there is an action item for you to complete.


## 1. Python Introduction (Optional)

From the terminal, you can start a python interpreter by just typing `python` in the command-line. Once you create a python, you can run it from terminal by just running `python <filename>.py`. 

If you are new to python, go through at least the following sections of this [Python tutorial](https://docs.python.org/3/tutorial/):

- section 1
- section 3 
- section 4 (skip 4.6 & 4.8)
- section 5  
- section 6

## 2. Numpy Introduction

Some steps below are borrowed from [numpy quickstart tutorial](https://docs.scipy.org/doc/numpy/user/quickstart.html), which I encourage you to reference throughout the course.

During this course we will often use numpy to manage our datasets. Type the following commands in the python interpreter (filling in missing pieces) and make sure the output makes sense:

#### Array creation and modification

```python
python
>>> import numpy as np
>>>
>>> # create a 4x5 array of zeros
>>> m = np.zeros([4,5])
>>> m
array([[ 0.,  0.,  0.,  0.,  0.],
       [ 0.,  0.,  0.,  0.,  0.],
       [ 0.,  0.,  0.,  0.,  0.],
       [ 0.,  0.,  0.,  0.,  0.]])
>>>
>>> # create a 3x5 array of zeros using reshape
>>> a = np.arange(15).reshape(3, 5)
>>> a
array([[ 0,  1,  2,  3,  4],
      [ 5,  6,  7,  8,  9],
      [10, 11, 12, 13, 14]])
>>>
>>> # create an array from a list
>>> b = np.array([6, 7, 8])
>>> b
array([6, 7, 8])
```

**TODO and DISCUSS**

- Use the `.shape` attribute to find the shape of `m`, `a`, and `b` above
- Change several of the entries of `m` using assignment (similar to lists, i.e. `m[2][1]`)
- To what dimensions could you reshape `m`? Try out a few of these to see how the entries behave.
- What does reshape do when `-1` is used as part of the shape? For multi-dimensional arrays, how many dimensions can be specified with `-1`.

<br>
<br>
<br> 
*Switch who is navigator and driver*

#### Array slicing and concatenation

Try out the slicing operations below, predicting what will be printed each time. Make sure you have modified the `m` array enough that output is clear (you may need to recreate `m` if you switched who was sharing the screen).

```
>>> m[2]
>>> m[:,1]
>>> m[:3,:2]
```

**TODO and DISCUSS**

- Look up the `concatenate` function and apply it to your `m` array and `a` array to produce an 7x5 array.
Look up the `sort` function (from numpy) and apply it to both axes of your `m` array (as well as `axis=None`) and make sure the output makes sense.

*optional: save your interpreter commands to a file and email to each partner*

<br><br><br>

## 3. Math Pre-exam

Complete the following [math pre-exam]({{site.url}}{{site.baseurl}}labs/lab01/math_pretest.pdf). This will be graded on effort, not correctness - the purpose of this part of Lab 1 is so that I know how much math review to do later on. You have a few options for working on this part:

1. Print it out, write down your answers on the pages.
2. Write your answers on a separate sheet of paper, but clearly number the questions.
3. LaTeX your answers.
4. 
For the first two approaches, “scan” the pages using a phone (I recommend the app “CamScanner”) to create a single PDF. For all approaches, add the final PDF to your Lab 1 on Gradescope.

### Signing out
For the remaining labs, before leaving, make sure your TA/instructor have signed you out of the lab. If you finish the lab early, you are free to go.

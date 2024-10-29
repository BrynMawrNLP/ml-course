---
title: Final Project - Proposal
layout: default
active_tab: main_page 
---

# Overview

The goal of the final project is to gain experience with the entire machine learning pipeline. This will include identifying a dataset, algorithm(s), and scientific question. In your final presentation you should also include motivation, hypotheses, data collection/cleaning, algorithm development/application, evaluation of results, interpretation, and conclusion. Below I’ll describe the main components your project should include and provide a few dataset resources. You are welcome to choose a non-data-driven project (options below), but make sure your proposal is very thorough about what you will do in this case.

This document describes the project <i>proposal</i> and getting started on the project - there will be separate instructions for the oral presentation and writeup. The project is worth 15% of your overall grade.

### Timeline and Logistics

- November 14: project proposal due
- November 14 - December 13: working on projects
- December XX: oral project presentations during exam slot
- December XX: writeups and github repos must be finalized

For the oral presentations, each group will have roughly 10 minutes to speak.

You are <i>required</i> to work in pairs for the final project - group work is an important component of Computer Science (and other fields!) This in an opportunity to practice collaboration and creating something bigger than each person could individually. If you would like a random partner, please email me. 
Note: if you really prefer to work individually, requests will be considered on a case by case basis (please email me early about this).

# Proposal

The goal of the proposal is to help you start working on your final project and assembling the different resources you want to use (literature, software, data, etc). Broadly, your project should include:

1. A dataset
1. A machine learning algorithm(s) you will develop and/or apply to this dataset
1. A scientific question you are trying to answer
1. A train/validation learning curve
1. Additional ways to evaluate, interpret, and visualize the results
1. References

For the proposal, briefly outline each of these sections (details below) in a 1-page PDF document. Submit your proposal to me on gradescope.
I will provide brief feedback in the order I receive proposals. Include a title and both partner names.

### 1. Dataset

What dataset will you use for this project? Regardless of what you’re interested in, there is probably a dataset that is related. Please be as specific as possible - don’t assume your ideal data is available until you’ve actually downloaded and viewed it. Include a reference/link to your data in your proposal. Here are a few databases to get started. Note that I work mostly with biological data and do not have direct experience with most of these datasets. After you download the data, make sure that you can actually view it, that you understand the features and label (if applicable). What is `n`? What is `p`? Make sure the dataset includes enough examples that you could reasonably learn from it or analyze it (I would say `n<100` would be concerning).

- [Kaggle](https://www.kaggle.com/datasets): Wide variety of datasets (may need to create an account).

- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets.php): Also contains a wide variety of datasets (options on the left allow you to search by task, attribute type, etc which can be very useful).

- [Image Datasets](https://paperswithcode.com/datasets?mod=images): Large database of images (including MNIST and CIFAR-10).

- [Wikipedia Data List](https://en.wikipedia.org/wiki/List_of_datasets_for_machine-learning_research): Up-to-date list of datasets organized by category (may or may not be freely available):

	- Image data
	- Text data
	- Sound data
	- Signal data
	- Physical data
	- Biological data
	- Anomaly data
	- Question answering data
	- Multivariate data

### 2. Machine Learning method(s)
What software/methods will you use for the project? You can write your own methods, use your lab implementations from class, or use existing software, but there should be some programming component. You could compare two existing methods, or compare your own method to an existing method. Even if you’re planning to use existing software, there will likely be a significant programming component since you’ll have to get the data in the right format, learn how to run the program, and evaluate/visualize the results.

If you are using any existing software, include a reference.

### 3. Motivation and Scientific Question
Why is this an interesting or relevant topic? You could talk about your personal motivation for this topic, or why it would be interesting to investigate in general. What scientific question are you trying to answer? Briefly describe a hypothesis about the results you expect.

### 4. Training curve
This may not apply to all projects, but if your project involves training and/or hyperparameters, you should create a training/validation curve. This could have training iteration on the x-axis, or possibly model complexity. Think about if cross-validation approaches make sense here, and how to guard against over fitting.

### 5. Results: Evaluation, Interpretation, and Visualization
What type of results do you expect from your project? How will you evaluate and interpret the results? At least one visualization (figure) will be required for each project.

### 6. References
Include a list of at least two references (one might be the data). If you would like paper recommendations based on your topic, let me know. For the reference format, include:

	 - Author list (3 max, then et al)
	- Title (in quotes)
	- Journal (in italics)
	- Year (in parenthesis)

For references, you should use `bib` entries.


# Alternative Project Styles
1. Implementation based. If you would like to explore a large-scale software project, that is a great option. Ideas: you could implement a research paper that does not have code available online. Or you could implement an algorithm we have talked about in class but used existing software for (i.e. PCA). If you pursue this option, this software should be something you write from scratch yourself as part of this class, not something you have written before.

1. Theory based. I am also open to a more theoretical/mathematical project that does not involve data or substantial coding. If you have a concrete idea/plan for such a project, let me know. This option is fairly open-ended, but you should be creating something new or finding a new way to interpret complex/vague theory from the literature.

1. Reproduce a research paper. Another option is to reproduce the results and figures of an existing research paper. This is often not an easy task, but very illuminating into the data science pipeline. Please get in touch early with a specific paper if you’re interested in this option.

# Getting started after the proposal
I would recommend submitting your proposal as soon as possible so you can get feedback and get started. Your repository should include all the code you write for the project. Only include data if the datasets is very small (i.e. a fraction of the data or test example). The repository should also include your writeup (details about that will be in a separate assignment document) and eventually your slides for the presentation. Summary of what should be on git:

- All project code
- (optional) Small example datasets
- Writeup (details provided later on, but similar in spirit to Lab 6)
- README.md with command lines to reproduce your results and figures
- Presentation slides
- Do not include: existing software you are using, large datasets

### Project check-ins
There will be weekly project check-ins during class meetings.


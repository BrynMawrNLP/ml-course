---
title: Introduction to Machine Learning - Bryn Mawr College
layout: default
img: <!-- turk-engraving-detail -->
img_link: <!-- http://en.wikipedia.org/wiki/The_Turk -->
caption: <!--An engraving of the Mechanical Turk, the 18th century chess-playing automaton -->
active_tab: main_page 
---

Machine Learning as a field has grown considerably over the past few decades. In this course, we will explore both classical and modern approaches, with an emphasis on theoretical understanding. There will be a significant math component (statistics and probability in particular), as well as a substantial implementation component (as opposed to using high-level libraries). However, during the last part of the course we will use a few modern libraries such as Pytorch. By the end of this course, you should be able to form a hypothesis about a dataset of interest, use a variety of methods and approaches to test your hypothesis, and be able to interpret the results to form a meaningful conclusion. We will focus on real-world, publicly available datasets, not generating new data. 

<!-- Display an alert about upcoming homework assignments -->
{% capture now %}{{'now' | date: '%s'}}{% endcapture %}
{% for page in site.pages %}
{% if page.release_date and page.due_date %}
{% capture release_date %}{{page.release_date | date: '%s'}}{% endcapture %}
{% capture due_date %}{{page.due_date | date: '%s'}}{% endcapture %}
{% if release_date < now and due_date >= now %}
<div class="alert alert-info">
<a href="{{site.url}}{{site.baseurl}}{{page.url}}">{{ page.title }}</a> has been released.  
{% if page.deliverables %}
The assignment has multiple deliverables.
{% for deliverable in page.deliverables %}
The {{deliverable.description}} is due before {{ deliverable.due_date | date: "%I:%M%p" }} on {{ deliverable.due_date | date: "%A, %B %-d, %Y" }}.  
{% endfor %}
{% else %}
It is due before {{ page.due_date | date: "%I:%M%p" }} on {{ page.due_date | date: "%A, %B %-d, %Y" }}.
{% endif %}
</div>
{% endif %}
{% endif %}
{% endfor %}
<!-- End alert for upcoming homework assignments -->


<!--
<div class="alert alert-info" markdown="1">
Check out the [excellent final projects](http://crowdsourcing-class.org/final-projects-2016.html) from last year's class.
</div>
-->


Course number
: CMSC B151 

Instructor
: [Adam Poliak](http://azpoliak.github.io)

Teaching Assistants
: [Course Staff](staff.html) 

Website 
: [https://bmc-cs-151.github.io/](https://bmc-cs-151.github.io/)

Discussion Forum
: [Piazza](https://piazza.com/brynmawr/fall2024/c66e)

Time and place
: Fall 2024, TTh 10:10-11:30am, Location: Park 159
: Lab W: 2:40-4:00pm, Location: Park 231

Office Hours
: <a href="{{ site.url }}{{ site.baseurl }}/office-hours.html">Times</a>

Prerequisites
: The following courses are required with a grade of 2.0 or better (or permission of
the instructor):
1. CMSC B151 or CMSC HC 106/107
2. MATH B203 or MATH H215
3. CMSC 231

Course Readings
: Each lecture has an accompanying chapter/section of the following free online textbooks:
- <a href="http://ciml.info/">A Course in Machine Learning</a> by Hal Duame III ("Duame" in schedule below)
- <a href="http://faculty.marshall.usc.edu/gareth-james/ISL/">An Introduction to Statistical Learning</a> by Gareth James, Daniela Witten, Trevor Hastie, and Robert Tibshirani ("ISL" in schedule below)
: Some lectures will have accompanying optional reading related to the lecture's topic

Grading
* Homeworks: 32%
* Labs: 6%
* Midterms: 40%
* Final Project: 15% 
* Participation (includes quizzes): 7%

<br>
See the <a href="{{ site.url }}{{ site.baseurl }}/policies.html">Policies</a> for more details.

<!--- Acknowledgments-->

---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<!--
  Fill in each section below. Every line starting with * is a bullet point;
  indent a line by two spaces to make it a sub-bullet.

  To offer a PDF of the CV instead, upload it to the files/ folder and replace
  this whole page with a single link, like:
      [Download my CV](/files/cv.pdf)
-->

Education
======

Work experience
======

Skills
======

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>

Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Service and leadership
======

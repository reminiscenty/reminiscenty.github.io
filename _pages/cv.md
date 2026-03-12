---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

**Download:** [Resume (PDF)](/files/resume.pdf)

Education
======
* Ph.D. in Electrical and Computer Engineering, University of California, Santa Barbara, 2021 -- present (Advisor: Prof. Peng Li)
* B.E. in Electronic Engineering & B.S. in Mathematics, Tsinghua University, Beijing, 2016 -- 2020

Internship Experience
======
* Summer 2025: Software Engineering Intern, Google, Sunnyvale, CA
  * Research Topic: Large language models for cloud jobs' resource and runtime prediction
  * Mentor: Shengke Zhou

* Summer 2024: AI Research Intern, NXP Automotive Processing, Austin, TX
  * Research Topic: Conformal prediction for time series forecasting of PCB board aging
  * Mentor: Chen He

* Summer 2023: AI Research Intern, NXP Automotive Processing, Austin, TX
  * Research Topic: Reliable interval prediction for chip performance
  * Mentor: Chen He

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

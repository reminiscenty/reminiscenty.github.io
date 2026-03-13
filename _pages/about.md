---
permalink: /
# title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}


Hi, I'm Yuxuan Yin! I am a Ph.D. in Electrical and Computer Engineering at UC Santa Barbara, where I am advised by Prof. Peng Li. Prior to joining UCSB, I earned my Bachelor in Electronic Engineering and Mathematics from Tsinghua University.

My research focuses on Agentic AI and deep learning for real-world applications. I have hand-on experience of self-evolving through feedback, long-context modeling, post-training, and uncertainty quantifications. My research has been published in leading academic venues, including ICML, AAAI, DAC, and ICCAD.


---
📢 I am currently on the job market and actively seeking full-time opportunities! I am looking for roles where I can leverage my foundation in reliable machine learning and hands-on LLM experience. Please feel free to reach out to me at y_yin at ucsb dot edu.


## Internship Experience
* Summer 2025: Software Engineering Intern, Google, Sunnyvale, CA
  * Research Topic: Large language models for cloud jobs' resource and runtime prediction
  * Mentor: Shengke Zhou

* Summer 2024: AI Research Intern, NXP Automotive Processing, Austin, TX
  * Research Topic: Conformal prediction for time series forecasting of PCB board aging
  * Mentor: Chen He

* Summer 2023: AI Research Intern, NXP Automotive Processing, Austin, TX
  * Research Topic: Reliable interval prediction for chip performance
  * Mentor: Chen He


## Preprints

{% for post in site.publications reversed %}
  {% if post.category == "manuscripts" %}
<div style="display: flex; gap: 1em; margin-bottom: 1.5em; align-items: flex-start;">
  <img src="{% if post.header.teaser %}{{ post.header.teaser | prepend: '/images/' | prepend: base_path }}{% else %}{{ '/images/profile.png' | prepend: base_path }}{% endif %}" alt="" style="width: 240px; height: 240px; object-fit: cover; flex-shrink: 0; border-radius: 4px;">
  <div>
    <strong>{% if post.link %}<a href="{{ post.link }}">{{ post.title }}</a>{% else %}{{ post.title }}{% endif %}</strong><br>
    {{ post.citation }}{% if post.link %} <a href="{{ post.link }}">[paper]</a>{% endif %}
  </div>
</div>
  {% endif %}
{% endfor %}

## Publications

{% for post in site.publications reversed %}
  {% if post.category == "conferences" %}
<div style="display: flex; gap: 1em; margin-bottom: 1.5em; align-items: flex-start;">
  <img src="{% if post.header.teaser %}{{ post.header.teaser | prepend: '/images/' | prepend: base_path }}{% else %}{{ '/images/profile.png' | prepend: base_path }}{% endif %}" alt="" style="width: 240px; height: 240px; object-fit: cover; flex-shrink: 0; border-radius: 4px;">
  <div>
    <strong>{% if post.link %}<a href="{{ post.link }}">{{ post.title }}</a>{% else %}{{ post.title }}{% endif %}</strong><br>
    {{ post.citation }}{% if post.link %} <a href="{{ post.link }}">[paper]</a>{% endif %}
  </div>
</div>
  {% endif %}
{% endfor %}




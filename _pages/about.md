---
permalink: /
# title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}


Hi, I'm Yuxuan Yin, a Ph.D. candidate in Electrical and Computer Engineering at UC Santa Barbara, advised by [Prof. Peng Li](https://scholar.google.com/citations?user=QYQUS7gAAAAJ&hl=en&authuser=2). I received my B.E. in Electronic Engineering and B.S. in Mathematics from Tsinghua University.

My research spans agentic AI and reliable deep learning for real-world applications, with hands-on experience in LLM post-training, long-context modeling, and uncertainty quantification. I am the lead author of [ADO-LLM](https://dl.acm.org/doi/abs/10.1145/3676536.3676816), the first LLM-driven agent for automated analog circuit sizing. My work has appeared at ICML, AAAI, ICCAD, DAC, and ISCA.

---
📢 I am on the job market and actively seeking full-time opportunities. I am looking for roles where I can leverage my expertise in reliable ML and LLM systems. Feel free to reach out at y_yin [at] ucsb [dot] edu.


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
  <div style="font-size: 0.9em;">
    <strong>{{ post.title }}</strong><br>
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
  <div style="font-size: 0.9em;">
    <strong>{{ post.title }}</strong><br>
    {{ post.citation }}{% if post.link %} <a href="{{ post.link }}">[paper]</a>{% endif %}
  </div>
</div>
  {% endif %}
{% endfor %}




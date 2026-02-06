---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **Ph.D. in Engineering**, Institute of Science Tokyo (formerly Tokyo Institute of Technology), Apr. 2025 – Present 
  * Advisor: Prof. Daisuke Kurabayashi 
* **M.S. in Engineering**, Institute of Science Tokyo (formerly Tokyo Institute of Technology), Sept. 2023 – Mar. 2025 
  * **Completed in 1.5 years (6 months early completion)** 
* **B.S. in Engineering**, Tokyo Institute of Technology, Apr. 2020 – Sept. 2023 
  * **Completed in 3.5 years (6 months early completion)** 

Research Experience
======
* **JSPS Research Fellow (DC1)**, Apr. 2025 – Present 
  * Japan Society for the Promotion of Science (JSPS) 
* **Visiting Researcher**, Sept. 2025 – Present
  * BioRobotics Laboratory (BioRob), EPFL, Switzerland 
  * Supported by TOBITATE! Young Ambassador Program 

Technical Skills
======
* **Nonlinear Systems**: Expertise in phase oscillators and phase reduction theory 
* **Robotics**: Hardware design, PCB fabrication, and autonomous robot programming 
* **Programming**: Python, C++, MATLAB, ROS 
* **Languages**: English (TOEIC 905) 

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Awards
======
* **Outstanding Master's Thesis Presentation Award**, Institute of Science Tokyo, Mar. 2025
* **Best Research Encouragement Award (Emerging Research Category)**, SSS 2025, Jan. 2025
* **TOBITATE! Young Ambassador Program Scholarship**, MEXT, 2025 
* **JSPS Research Fellowship (DC1)**, 2025 – 2028 

Talks
======
<ul>
  {% for post in site.talks reversed %}
    <li>
      <strong>{{ post.title }}</strong><br />
      <span style="font-size: 0.85em; color: #5a5a5a;">
        {% if post.type %}{{ post.type }}, {% endif %}
        <i>{{ post.venue }}</i>, {{ post.location }}, {{ post.date | date: "%b %Y" }}.
      </span>
    </li>
  {% endfor %}
</ul>
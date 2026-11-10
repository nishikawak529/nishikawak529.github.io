---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<h2 data-lang="en">Education</h2>
<h2 data-lang="ja">学歴</h2>
<ul>
  <li data-lang="en"><strong>Doctoral Student in Engineering</strong>, Institute of Science Tokyo (formerly Tokyo Institute of Technology), Apr. 2025 – Present<br>Advisor: Prof. Daisuke Kurabayashi</li>
  <li data-lang="ja"><strong>博士課程（工学）</strong>、東京科学大学（旧 東京工業大学）、2025年4月 – 現在<br>指導教員：倉林大輔 教授</li>
  <li data-lang="en"><strong>M.S. in Engineering</strong>, Institute of Science Tokyo (formerly Tokyo Institute of Technology), Sept. 2023 – Mar. 2025<br><strong>Completed in 1.5 years (6 months early completion)</strong></li>
  <li data-lang="ja"><strong>修士（工学）</strong>、東京科学大学（旧 東京工業大学）、2023年9月 – 2025年3月<br><strong>1年半で修了（半年早期修了）</strong></li>
  <li data-lang="en"><strong>B.S. in Engineering</strong>, Tokyo Institute of Technology, Apr. 2020 – Sept. 2023<br><strong>Completed in 3.5 years (6 months early completion)</strong></li>
  <li data-lang="ja"><strong>学士（工学）</strong>、東京工業大学、2020年4月 – 2023年9月<br><strong>3年半で卒業（半年早期卒業）</strong></li>
</ul>

<h2 data-lang="en">Research Experience</h2>
<h2 data-lang="ja">研究歴</h2>
<ul>
  <li data-lang="en"><strong>JSPS Research Fellow (DC1)</strong>, Apr. 2025 – Present<br>Japan Society for the Promotion of Science (JSPS)</li>
  <li data-lang="ja"><strong>日本学術振興会 特別研究員（DC1）</strong>、2025年4月 – 現在</li>
  <li data-lang="en"><strong>Visiting Doctoral Student</strong>, Sept. 2025 – Sept. 30, 2026<br>Biorobotics Laboratory (BioRob), EPFL, Switzerland<br>Supported by the TOBITATE! Young Ambassador Program</li>
  <li data-lang="ja"><strong>Visiting Doctoral Student（博士課程訪問学生）</strong>、2025年9月 – 2026年9月30日<br>スイス連邦工科大学ローザンヌ校（EPFL）Biorobotics Laboratory（BioRob）<br>トビタテ！留学JAPANの支援による研究滞在</li>
</ul>

<h2 data-lang="en">Technical Skills</h2>
<h2 data-lang="ja">専門・スキル</h2>
<ul>
  <li data-lang="en"><strong>Nonlinear Systems:</strong> Expertise in phase oscillators and phase reduction theory</li>
  <li data-lang="ja"><strong>非線形システム：</strong>位相振動子・位相縮約理論</li>
  <li data-lang="en"><strong>Robotics:</strong> Hardware design, PCB fabrication, and autonomous robot programming</li>
  <li data-lang="ja"><strong>ロボティクス：</strong>ハードウェア設計、基板製作、自律ロボットのプログラミング</li>
  <li data-lang="en"><strong>Programming:</strong> Python, C++, MATLAB, ROS</li>
  <li data-lang="ja"><strong>プログラミング：</strong>Python、C++、MATLAB、ROS</li>
  <li data-lang="en"><strong>Languages:</strong> English (TOEIC 905)</li>
  <li data-lang="ja"><strong>語学：</strong>英語（TOEIC 905点）</li>
</ul>

<h2 data-lang="en">Publications</h2>
<h2 data-lang="ja">論文</h2>
{% include publication-list.html heading="h3" %}

<h2 data-lang="en">Awards</h2>
<h2 data-lang="ja">受賞・採択</h2>
<ul>
  <li data-lang="en"><strong>JSME Young Excellent Presentation Fellow Award</strong> (日本機械学会若手優秀講演フェロー賞), award ceremony at ROBOMECH 2026 on June 30, 2026</li>
  <li data-lang="ja"><strong>日本機械学会若手優秀講演フェロー賞</strong>、ROBOMECH 2026での授賞式：2026年6月30日</li>
  <li data-lang="en"><strong>Outstanding Master's Thesis Presentation Award</strong>, Institute of Science Tokyo, Mar. 2025</li>
  <li data-lang="ja"><strong>優秀論文発表賞</strong>、東京科学大学、2025年3月</li>
  <li data-lang="en"><strong>Best Research Encouragement Award (Emerging Research Category)</strong>, SSS 2025, Jan. 2025</li>
  <li data-lang="ja"><strong>最優秀研究奨励賞（萌芽研究部門）</strong>、第37回自律分散システム・シンポジウム、2025年1月</li>
  <li data-lang="en"><strong>TOBITATE! Young Ambassador Program Scholarship</strong>, MEXT, 2025</li>
  <li data-lang="ja"><strong>トビタテ！留学JAPAN 新日本代表プログラム 奨学金</strong>、文部科学省、2025年</li>
  <li data-lang="en"><strong>JSPS Research Fellowship (DC1)</strong>, 2025 – 2028</li>
  <li data-lang="ja"><strong>日本学術振興会 特別研究員（DC1）</strong>、2025年 – 2028年</li>
</ul>

<h2 data-lang="en">Talks</h2>
<h2 data-lang="ja">学会発表</h2>
<ul>
  {% assign talks = site.talks | sort: 'date' | reverse %}
  {% for post in talks %}
    <li>
      <strong>{{ post.title }}</strong><br>
      <span class="page__meta">
        <span data-lang="en">{% if post.type %}{{ post.type }}, {% endif %}<i>{{ post.venue }}</i>, {{ post.location }}, {{ post.date | date: "%b %Y" }}.</span>
        <span data-lang="ja">{% if post.type_ja %}{{ post.type_ja }}、{% elsif post.type == 'Poster presentation' %}ポスター発表、{% elsif post.type == 'Oral presentation' %}口頭発表、{% elsif post.type %}{{ post.type }}、{% endif %}<i>{{ post.venue }}</i>、{{ post.location }}、{{ post.date | date: "%Y年%m月" }}。</span>
      </span>
    </li>
  {% endfor %}
</ul>

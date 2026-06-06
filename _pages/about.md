---
layout: default
permalink: /
title: "Home"
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

<main class="page--wide" role="main">
  <section class="profile-hero">
    <img src="/images/profile.png" alt="Xiangchen Wang profile photo">
    <div>
      <h1>Xiangchen Wang</h1>
      <p>video understanding, Multi-model Agent and embodied navigation.</p>
    </div>
  </section>

  <p>I am currently completing my M.S. in Computer Science at Southern University of Science and Technology (SUSTech), and will begin my Ph.D. study at Zhejiang University in Fall 2026.</p>

  <h2 class="section-heading">News</h2>
  <ul class="compact-list">
  </ul>

  <h2 class="section-heading">Experience</h2>
  <ul class="compact-list">
    <li><strong>Ph.D.</strong>, Zhejiang University, from Fall 2026</li>
    <li><strong>M.S.</strong>, Southern University of Science and Technology, 2023-2026</li>
    <li><strong>B.S.</strong>, Southern University of Science and Technology, 2019-2023</li>
  </ul>



  <!-- <h2 class="section-heading">Research Interests</h2>
  <ul class="compact-list">
    <li>Vision-language learning</li>
    <li>Video understanding and efficient multimodal modeling</li>
    <li>Embodied AI and vision-language navigation</li>
    <li>Adaptive inference for real-world deployment</li>
  </ul> -->

  <h2 class="section-heading">Research</h2>
  <div class="works-list">
    {% assign works = site.data.works | sort: "date" | reverse %}
    {% for work in works %}
      {% include work-card.html work=work %}
    {% endfor %}
  </div>
</main>

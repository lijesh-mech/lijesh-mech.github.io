---
layout: page
title: About
permalink: /
nav: true
nav_order: 1
description: "Academic website of Dr. Lijesh Koottaparambil"
---
<style>
  /* Expand the page width */
  .post,
  .post-content,
  .container,
  main {
    max-width: 1500px !important;
    width: 96% !important;
  }

  .custom-home {
    display: grid;
    grid-template-columns: 255px minmax(0, 1fr) 300px;
    gap: 34px;
    align-items: start;
    width: 100%;
    margin: 28px auto 0;
  }

  /* Left purple profile panel */
  .home-sidebar {
    min-height: 720px;
    background-color: #461d7c;
    border: 1px solid #35145f;
    color: #ffffff;
    overflow: hidden;
  }

  .home-sidebar img {
    display: block;
    width: 100% !important;
    height: 285px !important;
    margin: 0;
    object-fit: cover;
    object-position: top center;
  }

  .home-sidebar p {
    margin: 0;
    padding: 16px 20px 0;
    color: #ffffff;
    font-size: 15px;
    line-height: 1.35;
  }

  .home-sidebar p strong {
    display: inline-block;
    margin-right: 4px;
    color: #fdd023;
    font-size: 24px;
  }

  /* Main center content */
  .home-main {
    min-width: 0;
    padding-top: 2px;
  }

  .home-main > h1 {
    margin: 0 0 6px;
    padding-bottom: 10px;
    border-bottom: 2px solid #461d7c;
    font-size: 40px;
    font-weight: 500;
    line-height: 1.2;
  }

  .home-main > h1 + p {
    margin: 0 0 30px;
    font-size: 15px;
    line-height: 1.5;
  }

  .home-main hr {
    display: none;
  }

  .home-main p {
    font-size: 16px;
    line-height: 1.65;
    margin-bottom: 18px;
  }

  .home-main h3 {
    margin-top: 28px;
    margin-bottom: 10px;
    font-size: 23px;
  }

  /* Profile buttons */
  .home-main h3:last-of-type + p {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
  }

  .home-main h3:last-of-type + p a {
    display: inline-block;
    padding: 10px 14px;
    border-radius: 4px;
    background-color: #461d7c;
    color: #ffffff !important;
    text-decoration: none;
  }

  .home-main h3:last-of-type + p a:hover {
    background-color: #5f2a96;
    color: #fdd023 !important;
  }

  /* Right news panel */
  .home-news {
    padding: 22px;
    background-color: #f4f4f4;
    border-top: 6px solid #461d7c;
  }

  .home-news h2 {
    margin: 0 0 20px;
    font-size: 26px;
  }

  .home-news p {
    margin-bottom: 18px;
    padding-bottom: 16px;
    border-bottom: 1px solid #d5d5d5;
    font-size: 14px;
    line-height: 1.5;
  }

  .home-news p strong {
    color: #461d7c;
  }

  /* Hide only the visible page title area above the custom layout */
  .post-header > h1,
  .post-header > .post-description {
    display: none !important;
  }

  /* Tablet */
  @media screen and (max-width: 1150px) {
    .custom-home {
      grid-template-columns: 230px minmax(0, 1fr);
    }

    .home-news {
      grid-column: 1 / -1;
    }

    .home-sidebar {
      min-height: 650px;
    }
  }

  /* Mobile */
  @media screen and (max-width: 760px) {
    .post,
    .post-content,
    .container,
    main {
      width: 94% !important;
    }

    .custom-home {
      display: block;
    }

    .home-sidebar {
      min-height: auto;
      margin-bottom: 28px;
    }

    .home-sidebar img {
      height: auto !important;
      max-height: 430px;
    }

    .home-main {
      margin-bottom: 30px;
    }

    .home-main > h1 {
      font-size: 31px;
    }

    .home-news {
      margin-top: 25px;
    }
  }
</style>
<div class="custom-home">

  <div class="home-sidebar">

    <img
      src="{{ '/assets/img/lijesh_profile.jpg' | relative_url }}"
      alt="Dr. Lijesh Koottaparambil"
      style="width: 240px; height: auto;"
    >

    <p><strong>110+</strong> Publications</p>
    <p><strong>8</strong> Patents</p>
    <p><strong>15+</strong> Years of Research</p>

  </div>

  <div class="home-main">

    <h1>Dr. Lijesh Koottaparambil</h1>

    <p>
      Research Associate | Center for Rotating Machinery (CeRoM),
      Louisiana State University
    </p>

    <hr>

    <p>
      I am <strong>Dr. Lijesh Koottaparambil</strong>, a Research Associate
      at the <strong>Center for Rotating Machinery (CeRoM), Louisiana State
      University (LSU), USA</strong>.
    </p>

    <p>
      My research focuses on thermodynamics-based degradation assessment,
      tribology, hydrogen embrittlement, corrosion, molecular dynamics,
      food-process monitoring, battery health diagnostics, and
      AI-enabled intelligent manufacturing.
    </p>

    <p>
      My work aims to develop physics-informed methods and advanced sensing
      technologies for predicting degradation, remaining useful life, and
      process quality across engineering and manufacturing systems.
    </p>

    <h3>Research Interests</h3>

    <p>
      Degradation Entropy Generation |
      Tribology |
      Hydrogen Embrittlement |
      Molecular Dynamics |
      Food Manufacturing |
      Battery Diagnostics
    </p>

    <h3>Professional Profiles</h3>

    <p>
      <a href="mailto:lijesh@lsu.edu">Email</a> |
      <a href="https://www.linkedin.com/in/lijesh-koottaparambil-12270b95/" target="_blank" rel="noopener noreferrer">LinkedIn</a> |
      <a href="https://scholar.google.com/citations?user=h7tDdkwAAAAJ" target="_blank" rel="noopener noreferrer">Google Scholar</a> |
      <a href="https://www.researchgate.net/profile/Lijesh-P-2" target="_blank" rel="noopener noreferrer">ResearchGate</a>
    </p>

  </div>

  <div class="home-news">

    <h2>News &amp; Updates</h2>

    <p>
      <strong>2026</strong><br>
      Appointed Associate Editor of the ASME Journal of Tribology.
    </p>

    <p>
      <strong>2025</strong><br>
      New U.S. patent granted for real-time food-process monitoring.
    </p>

    <p>
      <strong>2025</strong><br>
      Advanced entropy-based approaches for engineering degradation assessment.
    </p>

    <p>
      <a href="{{ '/awards/' | relative_url }}">
        View Awards &amp; Honors
      </a>
    </p>

  </div>

</div>

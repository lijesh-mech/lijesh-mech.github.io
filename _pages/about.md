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
    grid-template-columns: 285px minmax(0, 1fr) 310px;
    gap: 36px;
    align-items: start;
    width: 100%;
    margin: 28px auto 0;
  }

  /* Professional left profile panel */
  .home-sidebar {
    min-height: 720px;
    overflow: hidden;
    background: #461d7c;
    border: 1px solid rgba(70, 29, 124, 0.35);
    border-radius: 8px;
    color: #ffffff;
  }

  .profile-image-wrapper {
    padding: 10px 10px 0;
    background: #461d7c;
  }

  .sidebar-profile-image {
    display: block;
    width: 100% !important;
    height: 295px !important;
    margin: 0;
    border-radius: 4px 4px 0 0;
    object-fit: cover;
    object-position: top center;
  }

  .sidebar-content {
    padding: 24px 20px 28px;
  }

  .sidebar-contact {
    display: flex;
    flex-direction: column;
    gap: 7px;
  }

  .contact-row {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 11px 8px;
    border-radius: 5px;
    color: #ffffff !important;
    text-decoration: none !important;
    transition:
      background-color 0.2s ease,
      transform 0.2s ease;
  }

  .contact-row:hover {
    background: rgba(255, 255, 255, 0.11);
    transform: translateX(2px);
  }

  .contact-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    flex: 0 0 34px;
    width: 34px;
    height: 34px;
    border: 1px solid rgba(253, 208, 35, 0.75);
    border-radius: 50%;
    color: #fdd023;
    font-size: 15px;
  }

  .contact-text {
    display: flex;
    min-width: 0;
    flex-direction: column;
  }

  .contact-text small {
    margin-bottom: 2px;
    color: rgba(255, 255, 255, 0.72);
    font-size: 10px;
    font-weight: 600;
    letter-spacing: 0.06em;
    line-height: 1.2;
    text-transform: uppercase;
  }

  .contact-text strong {
    color: #ffffff;
    font-size: 13px;
    font-weight: 500;
    line-height: 1.4;
    overflow-wrap: anywhere;
  }

  .sidebar-divider {
    height: 1px;
    margin: 22px 0 18px;
    background: rgba(255, 255, 255, 0.22);
  }

  .sidebar-profiles {
    display: flex;
    flex-direction: column;
    gap: 8px;
  }

  .sidebar-profiles a {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 11px 12px;
    border: 1px solid rgba(253, 208, 35, 0.45);
    border-radius: 5px;
    color: #ffffff !important;
    font-size: 13px;
    font-weight: 500;
    text-decoration: none !important;
    transition:
      background-color 0.2s ease,
      border-color 0.2s ease,
      color 0.2s ease;
  }

  .sidebar-profiles a:hover {
    background: #fdd023;
    border-color: #fdd023;
    color: #35145f !important;
  }

  .profile-arrow {
    color: #fdd023;
    font-size: 15px;
    transition: transform 0.2s ease;
  }

  .sidebar-profiles a:hover .profile-arrow {
    color: #35145f;
    transform: translate(2px, -2px);
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

  .home-position {
    margin: 0 0 30px;
    color: var(--global-text-color-light);
    font-size: 15px;
    line-height: 1.5;
  }

  .home-main p {
    margin-bottom: 19px;
    font-size: 16px;
    line-height: 1.67;
  }

  .home-main h3 {
    margin-top: 30px;
    margin-bottom: 12px;
    font-size: 23px;
    font-weight: 500;
  }

  /* Research-interest tags */
  .research-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 9px;
    margin-top: 12px;
  }

  .research-tags span {
    display: inline-block;
    padding: 8px 12px;
    border: 1px solid rgba(70, 29, 124, 0.55);
    border-radius: 999px;
    background: rgba(70, 29, 124, 0.04);
    font-size: 13px;
    line-height: 1.2;
  }

  /* Right news panel */
  .home-news {
    padding: 22px;
    background-color: #f4f4f4;
    border-top: 6px solid #461d7c;
    border-radius: 0 0 6px 6px;
  }

  .home-news h2 {
    margin: 0 0 20px;
    font-size: 26px;
    font-weight: 500;
  }

  .news-item {
    margin-bottom: 18px;
    padding-bottom: 16px;
    border-bottom: 1px solid #d5d5d5;
  }

  .news-year {
    display: inline-block;
    margin-bottom: 6px;
    color: #461d7c;
    font-size: 13px;
    font-weight: 700;
  }

  .news-item p {
    margin: 0;
    font-size: 14px;
    line-height: 1.5;
  }

  .news-link {
    display: inline-block;
    margin-top: 4px;
    font-weight: 600;
    text-decoration: none;
  }

  /* Hide only the default heading area above the custom content */
  .post-header > h1,
  .post-header > .post-description {
    display: none !important;
  }

  /* Tablet */
  @media screen and (max-width: 1150px) {
    .custom-home {
      grid-template-columns: 260px minmax(0, 1fr);
    }

    .home-news {
      grid-column: 1 / -1;
    }

    .home-sidebar {
      min-height: 660px;
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

    .sidebar-profile-image {
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

  <aside class="home-sidebar">

    <div class="profile-image-wrapper">
      <img
        src="{{ '/assets/img/lijesh_profile.jpg' | relative_url }}"
        alt="Dr. Lijesh Koottaparambil"
        class="sidebar-profile-image"
      >
    </div>

    <div class="sidebar-content">

      <div class="sidebar-contact">

        <a class="contact-row" href="mailto:lijesh@lsu.edu">
          <span class="contact-icon">✉</span>
          <span class="contact-text">
            <small>University Email</small>
            <strong>lijesh@lsu.edu</strong>
          </span>
        </a>

        <a class="contact-row" href="mailto:lijesh_mech@yahoo.co.in">
          <span class="contact-icon">✉</span>
          <span class="contact-text">
            <small>Alternative Email</small>
            <strong>lijesh_mech@yahoo.co.in</strong>
          </span>
        </a>

        <a class="contact-row" href="tel:+16465499651">
          <span class="contact-icon">☎</span>
          <span class="contact-text">
            <small>Phone</small>
            <strong>(646) 549-9651</strong>
          </span>
        </a>

      </div>

      <div class="sidebar-divider"></div>

      <nav class="sidebar-profiles" aria-label="Professional profiles">

        <a
          href="https://scholar.google.com/citations?user=h7tDdkwAAAAJ"
          target="_blank"
          rel="noopener noreferrer"
        >
          <span>Google Scholar</span>
          <span class="profile-arrow">↗</span>
        </a>

        <a
          href="https://www.linkedin.com/in/lijesh-koottaparambil-12270b95/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <span>LinkedIn</span>
          <span class="profile-arrow">↗</span>
        </a>

        <a
          href="https://www.researchgate.net/profile/Lijesh-P-2"
          target="_blank"
          rel="noopener noreferrer"
        >
          <span>ResearchGate</span>
          <span class="profile-arrow">↗</span>
        </a>

      </nav>

    </div>

  </aside>

  <main class="home-main">

    <h1>Dr. Lijesh Koottaparambil</h1>

    <p class="home-position">
      Research Associate | Center for Rotating Machinery (CeRoM),
      Louisiana State University
    </p>

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

    <div class="research-tags">
      <span>Degradation Entropy Generation</span>
      <span>Tribology</span>
      <span>Hydrogen Embrittlement</span>
      <span>Molecular Dynamics</span>
      <span>Food Manufacturing</span>
      <span>Battery Diagnostics</span>
    </div>

  </main>

  <aside class="home-news">

    <h2>News &amp; Updates</h2>

    <div class="news-item">
      <span class="news-year">2026</span>
      <p>
        Appointed Associate Editor of the ASME Journal of Tribology.
      </p>
    </div>

    <div class="news-item">
      <span class="news-year">2025</span>
      <p>
        New U.S. patent granted for real-time food-process monitoring.
      </p>
    </div>

    <div class="news-item">
      <span class="news-year">2025</span>
      <p>
        Advanced entropy-based approaches for engineering degradation assessment.
      </p>
    </div>

    <a class="news-link" href="{{ '/awards/' | relative_url }}">
      View Awards &amp; Honors →
    </a>

  </aside>

</div>

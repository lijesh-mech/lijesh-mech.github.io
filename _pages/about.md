---
layout: page
title: About
permalink: /
nav: true
nav_order: 1
description: "Academic website of Dr. Lijesh Koottaparambil"
---

<style>
  :root {
    --profile-purple: #461d7c;
    --profile-purple-dark: #32105f;
    --profile-purple-light: #f6f2fb;
    --profile-text: #242433;
    --profile-muted: #686879;
    --profile-border: #e1e1e8;
    --profile-background: #ffffff;
    --profile-panel: #fafafd;
  }

  /* Expand the page width */
  .post,
  .post-content,
  .container {
    width: 96% !important;
    max-width: 1500px !important;
  }

  /* Hide the default page title */
  .post-header > h1,
  .post-header > .post-description {
    display: none !important;
  }

  /* Hide the standard al-folio footer */
  footer.fixed-bottom,
  footer.sticky-bottom {
    display: none !important;
  }

  .academic-home {
    width: 100%;
    margin: 34px auto 0;
    color: var(--profile-text);
  }

  .academic-grid {
    display: grid;
    grid-template-columns: 285px minmax(0, 1fr) 325px;
    gap: 42px;
    align-items: start;
  }

  /* =========================================================
     LEFT PROFILE AND CONTACT CARD
     ========================================================= */

  .profile-card {
    overflow: hidden;
    background: var(--profile-background);
    border: 1px solid var(--profile-border);
    border-top: 5px solid var(--profile-purple);
    border-radius: 10px;
    box-shadow: 0 6px 24px rgba(28, 20, 50, 0.07);
  }

  .profile-photo-wrapper {
    padding: 14px 14px 0;
  }

  .profile-photo {
    display: block;
    width: 100% !important;
    height: auto !important;
    margin: 0;
    border-radius: 7px;
    object-fit: cover;
    object-position: top center;
  }

  .profile-contact-panel {
    padding: 18px 16px 17px;
  }

  .profile-contact-list {
    display: flex;
    flex-direction: column;
    gap: 2px;
  }

  .profile-contact-item {
    display: grid;
    grid-template-columns: 28px minmax(0, 1fr);
    gap: 10px;
    align-items: center;
    min-height: 54px;
    margin: 0;
    padding: 8px 5px;
    border-radius: 6px;
    color: var(--profile-text) !important;
    text-decoration: none !important;
    transition:
      background-color 0.2s ease,
      transform 0.2s ease;
  }

  .profile-contact-item:hover {
    background: var(--profile-purple-light);
    transform: translateX(2px);
  }

  .profile-contact-icon,
  .profile-social-icon {
    display: inline-flex !important;
    align-items: center;
    justify-content: center;
    width: 24px !important;
    height: 24px !important;
    min-width: 24px !important;
    min-height: 24px !important;
    margin: 0 !important;
    padding: 0 !important;
    color: var(--profile-purple);
    font-size: 12px;
    line-height: 1;
  }

  .profile-contact-icon svg,
  .profile-social-icon svg {
    display: block !important;
    width: 20px !important;
    height: 20px !important;
    max-width: 20px !important;
    max-height: 20px !important;
    margin: 0 !important;
    fill: none !important;
    stroke: currentColor !important;
    stroke-width: 1.8 !important;
    stroke-linecap: round;
    stroke-linejoin: round;
  }

  .profile-contact-copy {
    display: flex;
    min-width: 0;
    flex-direction: column;
  }

  .profile-contact-copy strong {
    margin: 0;
    color: var(--profile-text);
    font-size: 12px;
    font-weight: 700;
    line-height: 1.3;
  }

  .profile-contact-copy span {
    margin-top: 2px;
    color: var(--profile-muted);
    font-size: 11px;
    line-height: 1.4;
    overflow-wrap: anywhere;
  }

  .profile-divider {
    height: 1px;
    margin: 13px 0 7px;
    background: var(--profile-border);
  }

  .profile-social-links {
    display: flex;
    flex-direction: column;
    margin: 0;
    padding: 0;
  }

  .profile-social-links a {
    display: grid;
    grid-template-columns: 28px minmax(0, 1fr) 16px;
    gap: 10px;
    align-items: center;
    min-height: 47px;
    margin: 0;
    padding: 8px 5px;
    border-bottom: 1px solid var(--profile-border);
    color: var(--profile-purple) !important;
    font-size: 12px;
    font-weight: 700;
    line-height: 1.3;
    text-decoration: none !important;
    transition:
      background-color 0.2s ease,
      padding-left 0.2s ease;
  }

  .profile-social-links a:last-child {
    border-bottom: 0;
  }

  .profile-social-links a:hover {
    padding-left: 9px;
    background: var(--profile-purple-light);
  }

  .profile-social-text-icon {
    border: 1px solid var(--profile-purple);
    border-radius: 3px;
    font-size: 12px !important;
    font-weight: 800;
  }

  .profile-social-text-icon sup {
    position: relative;
    top: -0.25em;
    font-size: 7px;
  }

  .profile-social-arrow {
    color: var(--profile-purple);
    font-size: 15px;
    line-height: 1;
    text-align: right;
  }

  /* =========================================================
     CENTER PROFILE CONTENT
     ========================================================= */

  .biography-panel {
    min-width: 0;
    padding-top: 4px;
  }

  .main-name {
    position: relative;
    margin: 0 0 25px;
    padding-bottom: 17px;
    color: var(--profile-text);
    font-size: clamp(32px, 3vw, 45px);
    font-weight: 700;
    letter-spacing: -0.025em;
    line-height: 1.08;
  }

  .main-name::after {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 62px;
    height: 4px;
    background: var(--profile-purple);
    border-radius: 999px;
    content: "";
  }

  .position-block {
    margin-bottom: 20px;
  }

  .position-title {
    margin: 0 0 5px;
    color: var(--profile-purple);
    font-size: 18px;
    font-weight: 750;
  }

  .position-affiliation {
    margin: 0;
    color: var(--profile-muted);
    font-size: 14px;
    line-height: 1.6;
  }

  /* Associate Editor and fellowship */

  .professional-highlights {
    display: grid;
    grid-template-columns: repeat(2, minmax(210px, 1fr));
    gap: 12px;
    margin: 25px 0 32px;
  }

  .highlight-card {
    display: flex;
    gap: 12px;
    align-items: center;
    min-height: 72px;
    padding: 13px 15px;
    background: var(--profile-panel);
    border: 1px solid var(--profile-border);
    border-radius: 8px;
    transition:
      background-color 0.2s ease,
      border-color 0.2s ease,
      transform 0.2s ease;
  }

  .highlight-card:hover {
    background: var(--profile-purple-light);
    border-color: rgba(70, 29, 124, 0.35);
    transform: translateY(-2px);
  }

  .highlight-icon {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    flex: 0 0 34px;
    width: 34px;
    height: 34px;
    color: var(--profile-purple);
  }

  .highlight-icon svg {
    display: block;
    width: 26px;
    height: 26px;
    fill: none;
    stroke: currentColor;
    stroke-width: 1.8;
    stroke-linecap: round;
    stroke-linejoin: round;
  }

  .highlight-content {
    display: flex;
    min-width: 0;
    flex-direction: column;
  }

  .highlight-content strong {
    color: var(--profile-text);
    font-size: 13px;
    font-weight: 750;
    line-height: 1.35;
  }

  .highlight-content span {
    margin-top: 3px;
    color: var(--profile-muted);
    font-size: 12px;
    line-height: 1.4;
  }

  /* Main sections */

  .content-section {
    margin-top: 30px;
    padding-top: 28px;
    border-top: 1px solid var(--profile-border);
  }

  .section-heading {
    display: flex;
    gap: 11px;
    align-items: center;
    margin: 0 0 19px;
    color: var(--profile-purple);
    font-size: 23px;
    font-weight: 700;
  }

  .section-icon {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    flex: 0 0 27px;
    width: 27px;
    height: 27px;
    color: var(--profile-purple);
  }

  .section-icon svg {
    display: block;
    width: 23px;
    height: 23px;
    fill: none;
    stroke: currentColor;
    stroke-width: 1.8;
    stroke-linecap: round;
    stroke-linejoin: round;
  }

  /* Biographical Sketch */

  .biography-copy p {
    margin: 0 0 18px;
    color: var(--profile-text);
    font-size: 15px;
    line-height: 1.75;
  }

  .biography-copy strong {
    color: var(--profile-purple-dark);
  }

  /* Research Interests */

  .research-chips {
    display: grid;
    grid-template-columns: repeat(3, minmax(165px, 1fr));
    gap: 11px;
  }

  .research-chip {
    display: flex;
    gap: 9px;
    align-items: center;
    min-height: 48px;
    padding: 10px 13px;
    background: var(--profile-panel);
    border: 1px solid var(--profile-border);
    border-radius: 8px;
    color: var(--profile-text);
    font-size: 13px;
    font-weight: 650;
    line-height: 1.3;
    transition:
      background-color 0.2s ease,
      border-color 0.2s ease,
      transform 0.2s ease;
  }

  .research-chip:hover {
    background: var(--profile-purple-light);
    border-color: rgba(70, 29, 124, 0.38);
    transform: translateY(-2px);
  }

  .research-chip-icon {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    flex: 0 0 21px;
    width: 21px;
    height: 21px;
    color: var(--profile-purple);
  }

  .research-chip-icon svg {
    display: block;
    width: 18px;
    height: 18px;
    fill: none;
    stroke: currentColor;
    stroke-width: 1.8;
    stroke-linecap: round;
    stroke-linejoin: round;
  }

  /* Selected Publications */

  .selected-publications {
    display: flex;
    flex-direction: column;
  }

  .publication-item {
    display: grid;
    grid-template-columns: 42px minmax(0, 1fr);
    gap: 14px;
    padding: 17px 0;
    border-bottom: 1px solid var(--profile-border);
  }

  .publication-item:first-child {
    padding-top: 4px;
  }

  .publication-number {
    padding-top: 2px;
    color: var(--profile-purple);
    font-size: 13px;
    font-weight: 750;
  }

  .publication-content h3 {
    margin: 0 0 6px;
    color: var(--profile-text);
    font-size: 15px;
    font-weight: 700;
    line-height: 1.45;
  }

  .publication-content h3 a {
    color: var(--profile-text) !important;
    text-decoration: none !important;
  }

  .publication-content h3 a:hover {
    color: var(--profile-purple) !important;
    text-decoration: underline !important;
    text-underline-offset: 3px;
  }

  .publication-authors {
    margin: 0 0 4px;
    color: var(--profile-muted);
    font-size: 13px;
    line-height: 1.5;
  }

  .publication-journal {
    margin: 0;
    color: var(--profile-purple);
    font-size: 12px;
    font-style: italic;
    line-height: 1.5;
  }

  .publication-link {
    display: inline-flex;
    gap: 7px;
    align-items: center;
    margin-top: 18px;
    color: var(--profile-purple) !important;
    font-size: 13px;
    font-weight: 700;
    text-decoration: none !important;
  }

  .publication-link:hover {
    color: var(--profile-purple-dark) !important;
  }

  /* =========================================================
     RIGHT NEWS PANEL
     ========================================================= */

  .news-card {
    overflow: hidden;
    padding: 25px 26px;
    background: var(--profile-background);
    border: 1px solid var(--profile-border);
    border-radius: 10px;
    box-shadow: 0 6px 24px rgba(28, 20, 50, 0.06);
  }

  .news-heading {
    display: flex;
    gap: 11px;
    align-items: center;
    margin: 0 0 24px;
    color: var(--profile-purple);
    font-size: 23px;
    font-weight: 700;
  }

  .news-entry {
    padding-bottom: 21px;
    margin-bottom: 21px;
    border-bottom: 1px solid var(--profile-border);
  }

  .news-meta {
    display: flex;
    gap: 8px;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 10px;
  }

  .news-year {
    color: var(--profile-purple);
    font-size: 14px;
    font-weight: 750;
  }

  .news-badge {
    display: inline-flex;
    align-items: center;
    padding: 5px 9px;
    background: var(--profile-purple-light);
    border-radius: 999px;
    color: var(--profile-purple);
    font-size: 10px;
    font-weight: 700;
    white-space: nowrap;
  }

  .news-entry p {
    margin: 0;
    color: var(--profile-text);
    font-size: 14px;
    line-height: 1.65;
  }

  .news-more {
    display: inline-flex;
    gap: 7px;
    align-items: center;
    color: var(--profile-purple) !important;
    font-size: 13px;
    font-weight: 700;
    text-decoration: none !important;
  }

  /* =========================================================
     CUSTOM FOOTER
     ========================================================= */

  .academic-footer {
    display: grid;
    grid-template-columns: 1.4fr 1fr 1fr;
    gap: 30px;
    align-items: center;
    margin-top: 58px;
    padding: 24px 3%;
    background: var(--profile-panel);
    border-top: 1px solid var(--profile-border);
  }

  .footer-lsu {
    display: flex;
    gap: 17px;
    align-items: center;
  }

  .lsu-wordmark {
    color: var(--profile-purple);
    font-size: 33px;
    font-weight: 850;
    letter-spacing: -0.07em;
    line-height: 1;
  }

  .footer-affiliation,
  .footer-copyright {
    color: var(--profile-muted);
    font-size: 12px;
    line-height: 1.55;
  }

  .footer-copyright {
    text-align: center;
  }

  .footer-links {
    display: flex;
    gap: 11px;
    align-items: center;
    justify-content: flex-end;
  }

  .footer-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 39px;
    height: 39px;
    background: var(--profile-background);
    border: 1px solid var(--profile-border);
    border-radius: 50%;
    color: var(--profile-purple) !important;
    font-size: 14px;
    font-weight: 800;
    text-decoration: none !important;
    transition:
      background-color 0.2s ease,
      transform 0.2s ease;
  }

  .footer-link:hover {
    background: var(--profile-purple-light);
    transform: translateY(-2px);
  }

  .footer-link svg {
    display: block;
    width: 19px;
    height: 19px;
    fill: none;
    stroke: currentColor;
    stroke-width: 1.8;
    stroke-linecap: round;
    stroke-linejoin: round;
  }

  .footer-rg sup {
    position: relative;
    top: -0.3em;
    font-size: 7px;
  }

  /* =========================================================
     RESPONSIVE DESIGN
     ========================================================= */

  @media screen and (max-width: 1200px) {
    .academic-grid {
      grid-template-columns: 260px minmax(0, 1fr);
      gap: 32px;
    }

    .news-card {
      grid-column: 1 / -1;
    }

    .research-chips {
      grid-template-columns: repeat(2, minmax(170px, 1fr));
    }
  }

  @media screen and (max-width: 780px) {
    .post,
    .post-content,
    .container {
      width: 94% !important;
    }

    .academic-home {
      margin-top: 20px;
    }

    .academic-grid {
      display: block;
    }

    .profile-card,
    .biography-panel,
    .news-card {
      margin-bottom: 30px;
    }

    .main-name {
      margin-top: 8px;
      font-size: 34px;
    }

    .professional-highlights,
    .research-chips {
      grid-template-columns: 1fr;
    }

    .academic-footer {
      grid-template-columns: 1fr;
      text-align: center;
    }

    .footer-lsu,
    .footer-links {
      justify-content: center;
    }
  }
</style>

<div class="academic-home">

  <div class="academic-grid">

    <!-- LEFT PROFILE AND CONTACT CARD -->
    <aside class="profile-card">

      <div class="profile-photo-wrapper">
        <img
          src="{{ '/assets/img/lijesh_profile.jpg' | relative_url }}"
          alt="Dr. Lijesh Koottaparambil"
          class="profile-photo"
        >
      </div>

      <div class="profile-contact-panel">

        <div class="profile-contact-list">

          <a class="profile-contact-item" href="mailto:lijesh@lsu.edu">

            <span class="profile-contact-icon" aria-hidden="true">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <rect x="3" y="5" width="18" height="14" rx="2"></rect>
                <path d="m4 7 8 6 8-6"></path>
              </svg>
            </span>

            <span class="profile-contact-copy">
              <strong>Email</strong>
              <span>lijesh@lsu.edu</span>
            </span>

          </a>

          <a
            class="profile-contact-item"
            href="mailto:lijesh_mech@yahoo.co.in"
          >

            <span class="profile-contact-icon" aria-hidden="true">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <rect x="3" y="5" width="18" height="14" rx="2"></rect>
                <path d="m4 7 8 6 8-6"></path>
              </svg>
            </span>

            <span class="profile-contact-copy">
              <strong>Secondary Email</strong>
              <span>lijesh_mech@yahoo.co.in</span>
            </span>

          </a>

          <a class="profile-contact-item" href="tel:+16465499651">

            <span class="profile-contact-icon" aria-hidden="true">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <path d="M7 3h3l2 5-2 2a16 16 0 0 0 4 4l2-2 5 2v3a3 3 0 0 1-3 3C10 20 4 14 4 6a3 3 0 0 1 3-3z"></path>
              </svg>
            </span>

            <span class="profile-contact-copy">
              <strong>Phone</strong>
              <span>(646) 549-9651</span>
            </span>

          </a>

        </div>

        <div class="profile-divider"></div>

        <nav
          class="profile-social-links"
          aria-label="Professional profiles"
        >

          <a
            href="https://scholar.google.com/citations?user=h7tDdkwAAAAJ"
            target="_blank"
            rel="noopener noreferrer"
          >

            <span class="profile-social-icon" aria-hidden="true">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <path d="m3 9 9-5 9 5-9 5-9-5z"></path>
                <path d="M7 12v5c3 2 7 2 10 0v-5"></path>
              </svg>
            </span>

            <span>Google Scholar</span>
            <span class="profile-social-arrow">→</span>

          </a>

          <a
            href="https://www.linkedin.com/in/lijesh-koottaparambil-12270b95/"
            target="_blank"
            rel="noopener noreferrer"
          >

            <span class="profile-social-icon profile-social-text-icon">
              in
            </span>

            <span>LinkedIn</span>
            <span class="profile-social-arrow">→</span>

          </a>

          <a
            href="https://www.researchgate.net/profile/Lijesh-P-2"
            target="_blank"
            rel="noopener noreferrer"
          >

            <span class="profile-social-icon profile-social-text-icon">
              R<sup>G</sup>
            </span>

            <span>ResearchGate</span>
            <span class="profile-social-arrow">→</span>

          </a>

        </nav>

      </div>

    </aside>

    <!-- CENTER CONTENT -->
    <section class="biography-panel">

      <!-- NAME -->
      <h1 class="main-name">Dr. Lijesh Koottaparambil</h1>

      <!-- RESEARCH ASSOCIATE DETAILS -->
      <div class="position-block">

        <p class="position-title">Research Associate</p>

        <p class="position-affiliation">
          Center for Rotating Machinery (CeRoM)<br>
          Department of Mechanical &amp; Industrial Engineering<br>
          Louisiana State University, Baton Rouge, Louisiana, USA
        </p>

      </div>

      <!-- ASSOCIATE EDITOR AND FELLOWSHIP -->
      <div class="professional-highlights">

        <div class="highlight-card">

          <span class="highlight-icon" aria-hidden="true">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
            >
              <path d="M4 5a3 3 0 0 1 3-2h5v17H7a3 3 0 0 0-3 2z"></path>
              <path d="M20 5a3 3 0 0 0-3-2h-5v17h5a3 3 0 0 1 3 2z"></path>
            </svg>
          </span>

          <span class="highlight-content">
            <strong>Associate Editor</strong>
            <span>ASME Journal of Tribology</span>
          </span>

        </div>

        <div class="highlight-card">

          <span class="highlight-icon" aria-hidden="true">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
            >
              <path d="m3 9 9-5 9 5-9 5-9-5z"></path>
              <path d="M7 12v5c3 2 7 2 10 0v-5"></path>
            </svg>
          </span>

          <span class="highlight-content">
            <strong>Indo-US Postdoctoral Fellow</strong>
            <span>2018–2020</span>
          </span>

        </div>

      </div>

      <!-- BIOGRAPHICAL SKETCH -->
      <section class="content-section">

        <h2 class="section-heading">

          <span class="section-icon" aria-hidden="true">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
            >
              <path d="M4 5a3 3 0 0 1 3-2h5v17H7a3 3 0 0 0-3 2z"></path>
              <path d="M20 5a3 3 0 0 0-3-2h-5v17h5a3 3 0 0 1 3 2z"></path>
            </svg>
          </span>

          Biographical Sketch

        </h2>

        <div class="biography-copy">

          <p>
            Dr. Lijesh Koottaparambil is a Research Associate at the Center
            for Rotating Machinery (CeRoM), Louisiana State University. His
            research focuses on thermodynamics-based degradation assessment,
            tribology, hydrogen embrittlement, corrosion, molecular dynamics,
            food-process monitoring, battery diagnostics, and intelligent
            manufacturing.
          </p>

          <p>
            His work develops physics-informed methods and advanced sensing
            technologies for evaluating material and system degradation,
            predicting remaining useful life, and monitoring manufacturing
            process quality. He has authored more than 110 peer-reviewed
            publications, contributed to multiple U.S. and international
            patents, and supports the scientific community through editorial
            leadership, peer review, and interdisciplinary research
            collaboration.
          </p>

        </div>

      </section>

      <!-- RESEARCH INTERESTS -->
      <section class="content-section">

        <h2 class="section-heading">

          <span class="section-icon" aria-hidden="true">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
            >
              <path d="M9 3h6"></path>
              <path d="M10 3v6l-5 9a2 2 0 0 0 2 3h10a2 2 0 0 0 2-3l-5-9V3"></path>
              <path d="M8 15h8"></path>
            </svg>
          </span>

          Research Interests

        </h2>

        <div class="research-chips">

          <div class="research-chip">

            <span class="research-chip-icon" aria-hidden="true">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <path d="M9 3h6"></path>
                <path d="M10 3v6l-5 9a2 2 0 0 0 2 3h10a2 2 0 0 0 2-3l-5-9V3"></path>
                <path d="M8 15h8"></path>
              </svg>
            </span>

            <span>Degradation Entropy Generation</span>

          </div>

          <div class="research-chip">

            <span class="research-chip-icon" aria-hidden="true">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <path d="M10 13a5 5 0 0 0 7 0l2-2a5 5 0 0 0-7-7l-1 1"></path>
                <path d="M14 11a5 5 0 0 0-7 0l-2 2a5 5 0 0 0 7 7l1-1"></path>
              </svg>
            </span>

            <span>Tribology</span>

          </div>

          <div class="research-chip">

            <span class="research-chip-icon" aria-hidden="true">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <path d="M7 4v16"></path>
                <path d="M17 4v16"></path>
                <path d="M7 12h10"></path>
              </svg>
            </span>

            <span>Hydrogen Embrittlement</span>

          </div>

          <div class="research-chip">

            <span class="research-chip-icon" aria-hidden="true">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <circle cx="12" cy="12" r="2"></circle>
                <ellipse cx="12" cy="12" rx="10" ry="4"></ellipse>
                <ellipse
                  cx="12"
                  cy="12"
                  rx="4"
                  ry="10"
                  transform="rotate(45 12 12)"
                ></ellipse>
                <ellipse
                  cx="12"
                  cy="12"
                  rx="4"
                  ry="10"
                  transform="rotate(-45 12 12)"
                ></ellipse>
              </svg>
            </span>

            <span>Molecular Dynamics</span>

          </div>

          <div class="research-chip">

            <span class="research-chip-icon" aria-hidden="true">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <rect x="4" y="4" width="6" height="6" rx="1"></rect>
                <rect x="14" y="4" width="6" height="6" rx="1"></rect>
                <rect x="4" y="14" width="6" height="6" rx="1"></rect>
                <rect x="14" y="14" width="6" height="6" rx="1"></rect>
                <path d="M10 7h4M7 10v4M17 10v4M10 17h4"></path>
              </svg>
            </span>

            <span>Food Manufacturing</span>

          </div>

          <div class="research-chip">

            <span class="research-chip-icon" aria-hidden="true">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <rect x="5" y="5" width="13" height="14" rx="2"></rect>
                <path d="M18 9h2v6h-2"></path>
                <path d="m12 8-3 5h3l-1 4 4-6h-3z"></path>
              </svg>
            </span>

            <span>Battery Diagnostics</span>

          </div>

        </div>

      </section>

      <!-- SELECTED PUBLICATIONS -->
      <section class="content-section">

        <h2 class="section-heading">

          <span class="section-icon" aria-hidden="true">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
            >
              <path d="M4 5a3 3 0 0 1 3-2h5v17H7a3 3 0 0 0-3 2z"></path>
              <path d="M20 5a3 3 0 0 0-3-2h-5v17h5a3 3 0 0 1 3 2z"></path>
            </svg>
          </span>

          Selected Publications

        </h2>

        <div class="selected-publications">

          <article class="publication-item">

            <div class="publication-number">01</div>

            <div class="publication-content">

              <h3>
                <a
                  href="https://doi.org/10.1016/j.newton.2025.100035"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  Entropy-Based Unified Theory of Failure Threshold of
                  Degrading Systems
                </a>
              </h3>

              <p class="publication-authors">
                Koottaparambil, L., and M. M. Khonsari
              </p>

              <p class="publication-journal">
                Newton 1, no. 3 (2025): 100035
              </p>

            </div>

          </article>

          <article class="publication-item">

            <div class="publication-number">02</div>

            <div class="publication-content">

              <h3>
                <a
                  href="https://doi.org/10.1016/j.cej.2024.151306"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  Application of Thermodynamics to Industrial Grease Production
                </a>
              </h3>

              <p class="publication-authors">
                Lijesh, K. P., R. A. Miller, A. Sanford, J. Carroll, and
                M. M. Khonsari
              </p>

              <p class="publication-journal">
                Chemical Engineering Journal 489 (2024): 151306
              </p>

            </div>

          </article>

          <article class="publication-item">

            <div class="publication-number">03</div>

            <div class="publication-content">

              <h3>
                <a
                  href="https://doi.org/10.1016/j.corsci.2024.112063"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  Experimentally Verified Thermodynamic Framework for Corrosion
                </a>
              </h3>

              <p class="publication-authors">
                Lijesh, K. P., A. Mahmoudi, and M. M. Khonsari
              </p>

              <p class="publication-journal">
                Corrosion Science 233 (2024): 112063
              </p>

            </div>

          </article>

          <article class="publication-item">

            <div class="publication-number">04</div>

            <div class="publication-content">

              <h3>
                <a
                  href="https://doi.org/10.1016/j.est.2024.110565"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  A Thermodynamic Approach for Characterizing the Degradation
                  of Li-Ion Batteries
                </a>
              </h3>

              <p class="publication-authors">
                Lijesh, K. P., and M. M. Khonsari
              </p>

              <p class="publication-journal">
                Journal of Energy Storage 82 (2024): 110565
              </p>

            </div>

          </article>

          <article class="publication-item">

            <div class="publication-number">05</div>

            <div class="publication-content">

              <h3>
                <a
                  href="https://doi.org/10.1016/j.wear.2026.206694"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  Wear Maps Derived from Thermodynamic Principles
                </a>
              </h3>

              <p class="publication-authors">
                Lijesh, K. P., and M. M. Khonsari
              </p>

              <p class="publication-journal">
                Wear 595 (2026): 206694
              </p>

            </div>

          </article>

          <article class="publication-item">

            <div class="publication-number">06</div>

            <div class="publication-content">

              <h3>
                <a
                  href="https://doi.org/10.1016/j.ijhydene.2026.156097"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  Entropy-Based Quantification of Hydrogen Embrittlement
                </a>
              </h3>

              <p class="publication-authors">
                Lijesh, K. P., M. Khorasani, M. Rouhi Moghanlou, and
                M. M. Khonsari
              </p>

              <p class="publication-journal">
                International Journal of Hydrogen Energy 251 (2026): 156097
              </p>

            </div>

          </article>

        </div>

        <a
          class="publication-link"
          href="{{ '/publications/' | relative_url }}"
        >
          View all publications
          <span aria-hidden="true">→</span>
        </a>

      </section>

    </section>

    <!-- NEWS AND UPDATES -->
    <aside class="news-card">

      <h2 class="news-heading">

        <span class="section-icon" aria-hidden="true">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
          >
            <rect x="3" y="5" width="18" height="16" rx="2"></rect>
            <path d="M7 3v4M17 3v4M3 10h18"></path>
          </svg>
        </span>

        News &amp; Updates

      </h2>

      <article class="news-entry">

        <div class="news-meta">
          <span class="news-year">2026</span>
          <span class="news-badge">Editorial Role</span>
        </div>

        <p>
          Appointed Associate Editor of the ASME Journal of Tribology.
        </p>

      </article>

      <article class="news-entry">

        <div class="news-meta">
          <span class="news-year">2025</span>
          <span class="news-badge">Patent</span>
        </div>

        <p>
          New U.S. patent granted for real-time food-process monitoring.
        </p>

      </article>

      <article class="news-entry">

        <div class="news-meta">
          <span class="news-year">2025</span>
          <span class="news-badge">Research</span>
        </div>

        <p>
          Advanced entropy-based approaches for engineering degradation
          assessment.
        </p>

      </article>

      <a class="news-more" href="{{ '/awards/' | relative_url }}">
        View all updates
        <span aria-hidden="true">→</span>
      </a>

    </aside>

  </div>

  <!-- CUSTOM FOOTER -->
  <footer class="academic-footer">

    <div class="footer-lsu">

      <div class="lsu-wordmark">LSU</div>

      <div class="footer-affiliation">
        <strong>Center for Rotating Machinery (CeRoM)</strong><br>
        Louisiana State University, Baton Rouge, Louisiana, USA
      </div>

    </div>

    <div class="footer-copyright">
      © 2026 Dr. Lijesh Koottaparambil.<br>
      All rights reserved.
    </div>

    <div class="footer-links">

      <a
        class="footer-link"
        href="https://scholar.google.com/citations?user=h7tDdkwAAAAJ"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Google Scholar"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
          aria-hidden="true"
        >
          <path d="m3 9 9-5 9 5-9 5-9-5z"></path>
          <path d="M7 12v5c3 2 7 2 10 0v-5"></path>
        </svg>
      </a>

      <a
        class="footer-link"
        href="https://www.linkedin.com/in/lijesh-koottaparambil-12270b95/"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="LinkedIn"
      >
        in
      </a>

      <a
        class="footer-link footer-rg"
        href="https://www.researchgate.net/profile/Lijesh-P-2"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="ResearchGate"
      >
        R<sup>G</sup>
      </a>

    </div>

  </footer>

</div>

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
    --profile-purple-light: #f5f1fa;
    --profile-text: #242433;
    --profile-muted: #686879;
    --profile-border: #e1e1e8;
    --profile-background: #ffffff;
    --profile-panel: #fafafd;
  }

  /* Expand the page width */
  .post,
  .post-content,
  .container,
  main {
    width: 96% !important;
    max-width: 1500px !important;
  }

  /* Hide the default page heading */
  .post-header > h1,
  .post-header > .post-description {
    display: none !important;
  }

  /* Hide the default footer */
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
     LEFT PROFILE PHOTO
     ========================================================= */

  .profile-photo-card {
    overflow: hidden;
    padding: 14px;
    background: var(--profile-background);
    border: 1px solid var(--profile-border);
    border-top: 5px solid var(--profile-purple);
    border-radius: 10px;
    box-shadow: 0 6px 24px rgba(28, 20, 50, 0.07);
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

  /* Position and affiliation */

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

  /* Professional appointments */

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
  }

  .highlight-card:hover {
    background: var(--profile-purple-light);
    border-color: rgba(70, 29, 124, 0.35);
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
    width: 23px;
    height: 23px;
    fill: none;
    stroke: currentColor;
    stroke-width: 1.8;
    stroke-linecap: round;
    stroke-linejoin: round;
  }

  /* Biographical sketch */

  .biography-copy p {
    margin: 0 0 18px;
    color: var(--profile-text);
    font-size: 15px;
    line-height: 1.75;
  }

  .biography-copy strong {
    color: var(--profile-purple-dark);
  }

  /* Research interests */

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

  .research-chip .section-icon {
    flex: 0 0 21px;
    width: 21px;
    height: 21px;
  }

  .research-chip .section-icon svg {
    width: 18px;
    height: 18px;
  }

  /* Selected publications */

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
    text-decoration: none !important;
  }

  .footer-link:hover {
    background: var(--profile-purple-light);
    transform: translateY(-2px);
  }

  .footer-link svg {
    width: 19px;
    height: 19px;
    fill: none;
    stroke: currentColor;
    stroke-width: 1.8;
    stroke-linecap: round;
    stroke-linejoin: round;
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
    .container,
    main {
      width: 94% !important;
    }

    .academic-home {
      margin-top: 20px;
    }

    .academic-grid {
      display: block;
    }

    .profile-photo-card,
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

<!-- Reusable SVG icons -->
<svg
  xmlns="http://www.w3.org/2000/svg"
  style="position:absolute;width:0;height:0;overflow:hidden"
  aria-hidden="true"
>
  <symbol id="icon-book" viewBox="0 0 24 24">
    <path d="M4 5a3 3 0 0 1 3-2h5v17H7a3 3 0 0 0-3 2z"></path>
    <path d="M20 5a3 3 0 0 0-3-2h-5v17h5a3 3 0 0 1 3 2z"></path>
  </symbol>

  <symbol id="icon-scholar" viewBox="0 0 24 24">
    <path d="m3 9 9-5 9 5-9 5-9-5z"></path>
    <path d="M7 12v5c3 2 7 2 10 0v-5"></path>
  </symbol>

  <symbol id="icon-flask" viewBox="0 0 24 24">
    <path d="M9 3h6"></path>
    <path d="M10 3v6l-5 9a2 2 0 0 0 2 3h10a2 2 0 0 0 2-3l-5-9V3"></path>
    <path d="M8 15h8"></path>
  </symbol>

  <symbol id="icon-chain" viewBox="0 0 24 24">
    <path d="M10 13a5 5 0 0 0 7 0l2-2a5 5 0 0 0-7-7l-1 1"></path>
    <path d="M14 11a5 5 0 0 0-7 0l-2 2a5 5 0 0 0 7 7l1-1"></path>
  </symbol>

  <symbol id="icon-hydrogen" viewBox="0 0 24 24">
    <path d="M7 4v16"></path>
    <path d="M17 4v16"></path>
    <path d="M7 12h10"></path>
  </symbol>

  <symbol id="icon-atom" viewBox="0 0 24 24">
    <circle cx="12" cy="12" r="2"></circle>
    <ellipse cx="12" cy="12" rx="10" ry="4"></ellipse>
    <ellipse cx="12" cy="12" rx="4" ry="10" transform="rotate(45 12 12)"></ellipse>
    <ellipse cx="12" cy="12" rx="4" ry="10" transform="rotate(-45 12 12)"></ellipse>
  </symbol>

  <symbol id="icon-process" viewBox="0 0 24 24">
    <rect x="4" y="4" width="6" height="6" rx="1"></rect>
    <rect x="14" y="4" width="6" height="6" rx="1"></rect>
    <rect x="4" y="14" width="6" height="6" rx="1"></rect>
    <rect x="14" y="14" width="6" height="6" rx="1"></rect>
    <path d="M10 7h4M7 10v4M17 10v4M10 17h4"></path>
  </symbol>

  <symbol id="icon-battery" viewBox="0 0 24 24">
    <rect x="5" y="5" width="13" height="14" rx="2"></rect>
    <path d="M18 9h2v6h-2"></path>
    <path d="m12 8-3 5h3l-1 4 4-6h-3z"></path>
  </symbol>

  <symbol id="icon-calendar" viewBox="0 0 24 24">
    <rect x="3" y="5" width="18" height="16" rx="2"></rect>
    <path d="M7 3v4M17 3v4M3 10h18"></path>
  </symbol>

  <symbol id="icon-linkedin" viewBox="0 0 24 24">
    <rect x="4" y="9" width="3" height="10"></rect>
    <circle cx="5.5" cy="5.5" r="1.5"></circle>
    <path d="M11 19V9h3v2c1-2 6-3 6 3v5h-3v-5c0-2-3-2-3 0v5z"></path>
  </symbol>

  <symbol id="icon-researchgate" viewBox="0 0 24 24">
    <circle cx="12" cy="12" r="9"></circle>
    <path d="M8 17V7h4a3 3 0 0 1 0 6H8"></path>
    <path d="m12 13 4 4"></path>
  </symbol>
</svg>

<div class="academic-home">

  <div class="academic-grid">

    <!-- LEFT PHOTO -->
    <aside class="profile-photo-card">
      <img
        src="{{ '/assets/img/lijesh_profile.jpg' | relative_url }}"
        alt="Dr. Lijesh Koottaparambil"
        class="profile-photo"
      >
    </aside>

    <!-- CENTER CONTENT -->
    <main class="biography-panel">

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
          <span class="highlight-icon">
            <svg aria-hidden="true">
              <use href="#icon-book"></use>
            </svg>
          </span>

          <span class="highlight-content">
            <strong>Associate Editor</strong>
            <span>ASME Journal of Tribology</span>
          </span>
        </div>

        <div class="highlight-card">
          <span class="highlight-icon">
            <svg aria-hidden="true">
              <use href="#icon-scholar"></use>
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
          <span class="section-icon">
            <svg aria-hidden="true">
              <use href="#icon-book"></use>
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
          <span class="section-icon">
            <svg aria-hidden="true">
              <use href="#icon-flask"></use>
            </svg>
          </span>
          Research Interests
        </h2>

        <div class="research-chips">

          <div class="research-chip">
            <span class="section-icon">
              <svg aria-hidden="true">
                <use href="#icon-flask"></use>
              </svg>
            </span>
            <span>Degradation Entropy Generation</span>
          </div>

          <div class="research-chip">
            <span class="section-icon">
              <svg aria-hidden="true">
                <use href="#icon-chain"></use>
              </svg>
            </span>
            <span>Tribology</span>
          </div>

          <div class="research-chip">
            <span class="section-icon">
              <svg aria-hidden="true">
                <use href="#icon-hydrogen"></use>
              </svg>
            </span>
            <span>Hydrogen Embrittlement</span>
          </div>

          <div class="research-chip">
            <span class="section-icon">
              <svg aria-hidden="true">
                <use href="#icon-atom"></use>
              </svg>
            </span>
            <span>Molecular Dynamics</span>
          </div>

          <div class="research-chip">
            <span class="section-icon">
              <svg aria-hidden="true">
                <use href="#icon-process"></use>
              </svg>
            </span>
            <span>Food Manufacturing</span>
          </div>

          <div class="research-chip">
            <span class="section-icon">
              <svg aria-hidden="true">
                <use href="#icon-battery"></use>
              </svg>
            </span>
            <span>Battery Diagnostics</span>
          </div>

        </div>

      </section>

      <!-- SELECTED PUBLICATIONS -->
      <section class="content-section">

        <h2 class="section-heading">
          <span class="section-icon">
            <svg aria-hidden="true">
              <use href="#icon-book"></use>
            </svg>
          </span>
          Selected Publications
        </h2>

        <div class="selected-publications">

          <article class="publication-item">
            <div class="publication-number">01</div>

            <div class="publication-content">
              <h3>Insert selected publication title here</h3>

              <p class="publication-authors">
                Lijesh Koottaparambil and co-authors
              </p>

              <p class="publication-journal">
                Journal name, volume, pages, year
              </p>
            </div>
          </article>

          <article class="publication-item">
            <div class="publication-number">02</div>

            <div class="publication-content">
              <h3>Insert selected publication title here</h3>

              <p class="publication-authors">
                Lijesh Koottaparambil and co-authors
              </p>

              <p class="publication-journal">
                Journal name, volume, pages, year
              </p>
            </div>
          </article>

          <article class="publication-item">
            <div class="publication-number">03</div>

            <div class="publication-content">
              <h3>Insert selected publication title here</h3>

              <p class="publication-authors">
                Lijesh Koottaparambil and co-authors
              </p>

              <p class="publication-journal">
                Journal name, volume, pages, year
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

    </main>

    <!-- NEWS AND UPDATES -->
    <aside class="news-card">

      <h2 class="news-heading">
        <span class="section-icon">
          <svg aria-hidden="true">
            <use href="#icon-calendar"></use>
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
        <svg aria-hidden="true">
          <use href="#icon-scholar"></use>
        </svg>
      </a>

      <a
        class="footer-link"
        href="https://www.linkedin.com/in/lijesh-koottaparambil-12270b95/"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="LinkedIn"
      >
        <svg aria-hidden="true">
          <use href="#icon-linkedin"></use>
        </svg>
      </a>

      <a
        class="footer-link"
        href="https://www.researchgate.net/profile/Lijesh-P-2"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="ResearchGate"
      >
        <svg aria-hidden="true">
          <use href="#icon-researchgate"></use>
        </svg>
      </a>

    </div>

  </footer>

</div>

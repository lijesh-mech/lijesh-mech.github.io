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
    --lijesh-purple: #461d7c;
    --lijesh-purple-dark: #31105e;
    --lijesh-purple-soft: #f5f1fa;
    --lijesh-gold: #fdd023;
    --lijesh-text: #232333;
    --lijesh-muted: #666779;
    --lijesh-border: #e2e2e8;
    --lijesh-card: #ffffff;
    --lijesh-panel: #fafafd;
  }

  /* Expand the theme content area */
  .post,
  .post-content,
  .container,
  main {
    width: 96% !important;
    max-width: 1500px !important;
  }

  /* Hide only the default page title and description */
  .post-header > h1,
  .post-header > .post-description {
    display: none !important;
  }

  /* Hide the standard theme footer because a custom footer is included below */
  footer.fixed-bottom,
  footer.sticky-bottom {
    display: none !important;
  }

  .academic-home {
    width: 100%;
    margin: 34px auto 0;
    color: var(--lijesh-text);
  }

  .academic-grid {
    display: grid;
    grid-template-columns: 310px minmax(0, 1fr) 330px;
    gap: 46px;
    align-items: start;
  }

  /* =========================================================
     LEFT PROFILE CARD
     ========================================================= */

  .profile-card {
    overflow: hidden;
    background: var(--lijesh-card);
    border: 1px solid var(--lijesh-border);
    border-top: 5px solid var(--lijesh-purple);
    border-radius: 10px;
    box-shadow: 0 6px 24px rgba(28, 20, 50, 0.07);
  }

  .profile-photo-wrap {
    padding: 16px 16px 0;
  }

  .profile-photo {
    display: block;
    width: 100% !important;
    height: 300px !important;
    margin: 0;
    border-radius: 7px;
    object-fit: cover;
    object-position: top center;
  }

  .profile-card-body {
    padding: 18px 20px 22px;
  }

  .profile-name {
    margin: 0 0 5px;
    color: var(--lijesh-purple);
    font-size: 25px;
    font-weight: 700;
    line-height: 1.15;
  }

  .profile-role {
    margin: 0 0 3px;
    color: var(--lijesh-muted);
    font-size: 14px;
    font-weight: 600;
  }

  .profile-affiliation {
    margin: 0;
    color: var(--lijesh-muted);
    font-size: 13px;
    line-height: 1.5;
  }

  .profile-divider {
    height: 1px;
    margin: 19px 0;
    background: var(--lijesh-border);
  }

  .contact-list {
    display: flex;
    flex-direction: column;
    gap: 5px;
  }

  .contact-item {
    display: grid;
    grid-template-columns: 33px minmax(0, 1fr);
    gap: 11px;
    align-items: center;
    padding: 9px 5px;
    border-radius: 6px;
    color: var(--lijesh-text) !important;
    text-decoration: none !important;
    transition:
      background-color 0.2s ease,
      transform 0.2s ease;
  }

  .contact-item:hover {
    background: var(--lijesh-purple-soft);
    transform: translateX(2px);
  }

  .icon-outline {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 25px;
    height: 25px;
    color: var(--lijesh-purple);
  }

  .icon-outline svg {
    width: 22px;
    height: 22px;
    fill: none;
    stroke: currentColor;
    stroke-width: 1.8;
    stroke-linecap: round;
    stroke-linejoin: round;
  }

  .contact-copy {
    min-width: 0;
  }

  .contact-label {
    display: block;
    margin-bottom: 1px;
    color: var(--lijesh-text);
    font-size: 13px;
    font-weight: 700;
  }

  .contact-value {
    display: block;
    color: var(--lijesh-muted);
    font-size: 12px;
    line-height: 1.4;
    overflow-wrap: anywhere;
  }

  .profile-links {
    display: flex;
    flex-direction: column;
  }

  .profile-link {
    display: grid;
    grid-template-columns: 30px minmax(0, 1fr) 18px;
    gap: 10px;
    align-items: center;
    padding: 11px 5px;
    border-bottom: 1px solid var(--lijesh-border);
    color: var(--lijesh-purple) !important;
    font-size: 13px;
    font-weight: 650;
    text-decoration: none !important;
    transition:
      color 0.2s ease,
      padding-left 0.2s ease;
  }

  .profile-link:last-child {
    border-bottom: 0;
  }

  .profile-link:hover {
    padding-left: 9px;
    color: var(--lijesh-purple-dark) !important;
  }

  .profile-link-arrow {
    color: var(--lijesh-purple);
    font-size: 18px;
    line-height: 1;
  }

  /* =========================================================
     CENTER BIOGRAPHY
     ========================================================= */

  .biography-panel {
    min-width: 0;
    padding-top: 6px;
  }

  .main-name {
  position: relative;
  margin: 0 0 28px;
  padding-bottom: 18px;
  color: var(--lijesh-text);
  font-size: clamp(32px, 3.2vw, 46px);
  font-weight: 700;
  letter-spacing: -0.025em;
  line-height: 1.1;
}
  }

  .main-name::after {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 62px;
    height: 4px;
    background: var(--lijesh-purple);
    border-radius: 999px;
    content: "";
  }

  .position-line {
    margin: 0 0 34px;
    color: var(--lijesh-muted);
    font-size: 16px;
    line-height: 1.6;
  }

  .position-highlight {
    color: var(--lijesh-purple);
    font-weight: 700;
  }

  .biography-copy {
    max-width: 850px;
  }

  .biography-copy p {
    margin: 0 0 21px;
    color: var(--lijesh-text);
    font-size: 16px;
    line-height: 1.8;
  }

  .biography-copy strong {
    color: var(--lijesh-purple-dark);
  }

  .research-section {
    margin-top: 35px;
    padding-top: 30px;
    border-top: 1px solid var(--lijesh-border);
  }

  .section-heading {
    display: flex;
    gap: 12px;
    align-items: center;
    margin: 0 0 21px;
    color: var(--lijesh-purple);
    font-size: 24px;
    font-weight: 700;
  }

  .section-heading .icon-outline {
    width: 26px;
    height: 26px;
  }

  .research-chips {
    display: grid;
    grid-template-columns: repeat(3, minmax(165px, 1fr));
    gap: 12px;
  }

  .research-chip {
    display: flex;
    gap: 10px;
    align-items: center;
    min-height: 47px;
    padding: 10px 14px;
    background: var(--lijesh-panel);
    border: 1px solid var(--lijesh-border);
    border-radius: 8px;
    color: var(--lijesh-text);
    font-size: 13px;
    font-weight: 600;
    line-height: 1.3;
    transition:
      border-color 0.2s ease,
      background-color 0.2s ease,
      transform 0.2s ease;
  }

  .research-chip:hover {
    background: var(--lijesh-purple-soft);
    border-color: rgba(70, 29, 124, 0.4);
    transform: translateY(-2px);
  }

  .research-chip .icon-outline {
    flex: 0 0 22px;
    width: 22px;
    height: 22px;
  }

  .research-chip .icon-outline svg {
    width: 19px;
    height: 19px;
  }

  /* =========================================================
     NEWS PANEL
     ========================================================= */

  .news-card {
    overflow: hidden;
    padding: 26px 27px;
    background: var(--lijesh-card);
    border: 1px solid var(--lijesh-border);
    border-radius: 10px;
    box-shadow: 0 6px 24px rgba(28, 20, 50, 0.06);
  }

  .news-heading {
    display: flex;
    gap: 12px;
    align-items: center;
    margin: 0 0 25px;
    color: var(--lijesh-purple);
    font-size: 24px;
    font-weight: 700;
  }

  .news-heading .icon-outline {
    width: 27px;
    height: 27px;
  }

  .news-entry {
    padding: 0 0 22px;
    margin-bottom: 22px;
    border-bottom: 1px solid var(--lijesh-border);
  }

  .news-entry:last-of-type {
    margin-bottom: 15px;
  }

  .news-meta {
    display: flex;
    gap: 8px;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 10px;
  }

  .news-year {
    color: var(--lijesh-purple);
    font-size: 14px;
    font-weight: 750;
  }

  .news-badge {
    display: inline-flex;
    gap: 5px;
    align-items: center;
    padding: 5px 9px;
    background: var(--lijesh-purple-soft);
    border-radius: 999px;
    color: var(--lijesh-purple);
    font-size: 10px;
    font-weight: 700;
    white-space: nowrap;
  }

  .news-badge .icon-outline {
    width: 14px;
    height: 14px;
  }

  .news-badge .icon-outline svg {
    width: 13px;
    height: 13px;
    stroke-width: 2;
  }

  .news-entry p {
    margin: 0;
    color: var(--lijesh-text);
    font-size: 14px;
    line-height: 1.7;
  }

  .news-more {
    display: inline-flex;
    gap: 8px;
    align-items: center;
    color: var(--lijesh-purple) !important;
    font-size: 13px;
    font-weight: 700;
    text-decoration: none !important;
  }

  .news-more:hover {
    color: var(--lijesh-purple-dark) !important;
  }

  /* =========================================================
     CUSTOM FOOTER
     ========================================================= */

  .academic-footer {
    display: grid;
    grid-template-columns: 1.4fr 1fr 1fr;
    gap: 30px;
    align-items: center;
    margin-top: 60px;
    padding: 25px 3%;
    background: var(--lijesh-panel);
    border-top: 1px solid var(--lijesh-border);
  }

  .footer-lsu {
    display: flex;
    gap: 18px;
    align-items: center;
  }

  .lsu-wordmark {
    color: var(--lijesh-purple);
    font-size: 34px;
    font-weight: 850;
    letter-spacing: -0.07em;
    line-height: 1;
  }

  .footer-affiliation {
    color: var(--lijesh-muted);
    font-size: 12px;
    line-height: 1.55;
  }

  .footer-copyright {
    color: var(--lijesh-muted);
    font-size: 12px;
    line-height: 1.55;
    text-align: center;
  }

  .footer-links {
    display: flex;
    gap: 12px;
    align-items: center;
    justify-content: flex-end;
  }

  .footer-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 39px;
    height: 39px;
    background: var(--lijesh-card);
    border: 1px solid var(--lijesh-border);
    border-radius: 50%;
    color: var(--lijesh-purple) !important;
    text-decoration: none !important;
    transition:
      background-color 0.2s ease,
      transform 0.2s ease;
  }

  .footer-link:hover {
    background: var(--lijesh-purple-soft);
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
      grid-template-columns: 285px minmax(0, 1fr);
      gap: 34px;
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

    .profile-card,
    .biography-panel,
    .news-card {
      margin-bottom: 30px;
    }

    .profile-photo {
      height: auto !important;
      max-height: 480px;
    }

    .main-name {
      margin-top: 8px;
      font-size: 39px;
    }

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

  @media screen and (max-width: 420px) {
    .profile-card-body {
      padding: 17px;
    }

    .main-name {
      font-size: 33px;
    }

    .position-line,
    .biography-copy p {
      font-size: 15px;
    }

    .news-card {
      padding: 21px;
    }
  }
</style>

<!-- Reusable inline SVG icon definitions -->
<svg
  xmlns="http://www.w3.org/2000/svg"
  style="position:absolute;width:0;height:0;overflow:hidden"
  aria-hidden="true"
>
  <symbol id="icon-mail" viewBox="0 0 24 24">
    <rect x="3" y="5" width="18" height="14" rx="2"></rect>
    <path d="m4 7 8 6 8-6"></path>
  </symbol>

  <symbol id="icon-phone" viewBox="0 0 24 24">
    <path d="M7 3h3l2 5-2 2a16 16 0 0 0 4 4l2-2 5 2v3a3 3 0 0 1-3 3C10 20 4 14 4 6a3 3 0 0 1 3-3z"></path>
  </symbol>

  <symbol id="icon-scholar" viewBox="0 0 24 24">
    <path d="m3 9 9-5 9 5-9 5-9-5z"></path>
    <path d="M7 12v5c3 2 7 2 10 0v-5"></path>
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
    <circle cx="4" cy="4" r="1"></circle>
    <circle cx="20" cy="20" r="1"></circle>
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
    <path d="M8 14h2M12 14h2M16 14h1M8 17h2M12 17h2"></path>
  </symbol>

  <symbol id="icon-book" viewBox="0 0 24 24">
    <path d="M4 5a3 3 0 0 1 3-2h5v17H7a3 3 0 0 0-3 2z"></path>
    <path d="M20 5a3 3 0 0 0-3-2h-5v17h5a3 3 0 0 1 3 2z"></path>
  </symbol>

  <symbol id="icon-patent" viewBox="0 0 24 24">
    <path d="M9 3h6l4 4v14H5V3z"></path>
    <path d="M15 3v5h5"></path>
    <circle cx="12" cy="14" r="3"></circle>
    <path d="m10 17-1 4 3-2 3 2-1-4"></path>
  </symbol>

  <symbol id="icon-research" viewBox="0 0 24 24">
    <circle cx="10" cy="10" r="6"></circle>
    <path d="m15 15 5 5"></path>
    <path d="M7 10h6M10 7v6"></path>
  </symbol>
</svg>

<div class="academic-home">

  <div class="academic-grid">

    <!-- LEFT PROFILE CARD -->
    <aside class="profile-card">

      <div class="profile-photo-wrap">
        <img
          src="{{ '/assets/img/lijesh_profile.jpg' | relative_url }}"
          alt="Dr. Lijesh Koottaparambil"
          class="profile-photo"
        >
      </div>

      <div class="profile-card-body">

        <div class="contact-list">

          <a class="contact-item" href="mailto:lijesh@lsu.edu">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-mail"></use></svg>
            </span>
            <span class="contact-copy">
              <span class="contact-label">LSU Email</span>
              <span class="contact-value">lijesh@lsu.edu</span>
            </span>
          </a>

          <a class="contact-item" href="mailto:lijesh_mech@yahoo.co.in">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-mail"></use></svg>
            </span>
            <span class="contact-copy">
              <span class="contact-label">Secondary Email</span>
              <span class="contact-value">lijesh_mech@yahoo.co.in</span>
            </span>
          </a>

          <a class="contact-item" href="tel:+16465499651">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-phone"></use></svg>
            </span>
            <span class="contact-copy">
              <span class="contact-label">Phone</span>
              <span class="contact-value">(646) 549-9651</span>
            </span>
          </a>

        </div>

        <div class="profile-divider"></div>

        <nav class="profile-links" aria-label="Professional profiles">

          <a
            class="profile-link"
            href="https://scholar.google.com/citations?user=h7tDdkwAAAAJ"
            target="_blank"
            rel="noopener noreferrer"
          >
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-scholar"></use></svg>
            </span>
            <span>Google Scholar</span>
            <span class="profile-link-arrow">→</span>
          </a>

          <a
            class="profile-link"
            href="https://www.linkedin.com/in/lijesh-koottaparambil-12270b95/"
            target="_blank"
            rel="noopener noreferrer"
          >
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-linkedin"></use></svg>
            </span>
            <span>LinkedIn</span>
            <span class="profile-link-arrow">→</span>
          </a>

          <a
            class="profile-link"
            href="https://www.researchgate.net/profile/Lijesh-P-2"
            target="_blank"
            rel="noopener noreferrer"
          >
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-researchgate"></use></svg>
            </span>
            <span>ResearchGate</span>
            <span class="profile-link-arrow">→</span>
          </a>

        </nav>

      </div>

    </aside>

    <!-- CENTER BIOGRAPHY -->
    <main class="biography-panel">

      <h1 class="main-name">Dr. Lijesh Koottaparambil</h1>

      <p class="position-line">
        <span class="position-highlight">Research Associate</span>
        | Center for Rotating Machinery (CeRoM), Louisiana State University
      </p>

      <div class="biography-copy">

        <p>
          I am <strong>Dr. Lijesh Koottaparambil</strong>, a Research Associate
          at the Center for Rotating Machinery (CeRoM), Louisiana State
          University (LSU), USA.
        </p>

        <p>
          My research focuses on thermodynamics-based degradation assessment,
          tribology, hydrogen embrittlement, corrosion, molecular dynamics,
          food-process monitoring, battery health diagnostics, and AI-enabled
          intelligent manufacturing.
        </p>

        <p>
          My work aims to develop physics-informed methods and advanced sensing
          technologies for predicting degradation, remaining useful life, and
          process quality across engineering and manufacturing systems.
        </p>

      </div>

      <section class="research-section">

        <h2 class="section-heading">
          <span class="icon-outline">
            <svg aria-hidden="true"><use href="#icon-flask"></use></svg>
          </span>
          Research Interests
        </h2>

        <div class="research-chips">

          <div class="research-chip">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-flask"></use></svg>
            </span>
            <span>Degradation Entropy Generation</span>
          </div>

          <div class="research-chip">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-chain"></use></svg>
            </span>
            <span>Tribology</span>
          </div>

          <div class="research-chip">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-hydrogen"></use></svg>
            </span>
            <span>Hydrogen Embrittlement</span>
          </div>

          <div class="research-chip">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-atom"></use></svg>
            </span>
            <span>Molecular Dynamics</span>
          </div>

          <div class="research-chip">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-process"></use></svg>
            </span>
            <span>Food Manufacturing</span>
          </div>

          <div class="research-chip">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-battery"></use></svg>
            </span>
            <span>Battery Diagnostics</span>
          </div>

        </div>

      </section>

    </main>

    <!-- RIGHT NEWS CARD -->
    <aside class="news-card">

      <h2 class="news-heading">
        <span class="icon-outline">
          <svg aria-hidden="true"><use href="#icon-calendar"></use></svg>
        </span>
        News &amp; Updates
      </h2>

      <article class="news-entry">
        <div class="news-meta">
          <span class="news-year">2026</span>
          <span class="news-badge">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-book"></use></svg>
            </span>
            Editorial Role
          </span>
        </div>
        <p>
          Appointed Associate Editor of the ASME Journal of Tribology.
        </p>
      </article>

      <article class="news-entry">
        <div class="news-meta">
          <span class="news-year">2025</span>
          <span class="news-badge">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-patent"></use></svg>
            </span>
            Patent
          </span>
        </div>
        <p>
          New U.S. patent granted for real-time food-process monitoring.
        </p>
      </article>

      <article class="news-entry">
        <div class="news-meta">
          <span class="news-year">2025</span>
          <span class="news-badge">
            <span class="icon-outline">
              <svg aria-hidden="true"><use href="#icon-research"></use></svg>
            </span>
            Research
          </span>
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
        <svg aria-hidden="true"><use href="#icon-scholar"></use></svg>
      </a>

      <a
        class="footer-link"
        href="https://www.linkedin.com/in/lijesh-koottaparambil-12270b95/"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="LinkedIn"
      >
        <svg aria-hidden="true"><use href="#icon-linkedin"></use></svg>
      </a>

      <a
        class="footer-link"
        href="https://www.researchgate.net/profile/Lijesh-P-2"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="ResearchGate"
      >
        <svg aria-hidden="true"><use href="#icon-researchgate"></use></svg>
      </a>

    </div>

  </footer>

</div>

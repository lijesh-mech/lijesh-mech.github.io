---
layout: page
title: Damage Assessment of Tribo-Systems
permalink: /patents/damage-assessment/
nav: false
description: "U.S. patent on thermodynamics-based damage assessment of tribo-systems."
---

<style>
:root {
  --patent-purple: #461d7c;
  --patent-purple-dark: #32105f;
  --patent-text: #242433;
  --patent-muted: #666678;
  --patent-border: #e1e1e8;
}

.post,
.post-content,
.container {
  width: 95% !important;
  max-width: 1450px !important;
}

.post-header > h1,
.post-header > .post-description {
  display: none !important;
}

.damage-patent-page {
  width: 100%;
  margin: 34px auto 70px;
  color: var(--patent-text);
}

.back-to-patents {
  display: inline-flex;
  align-items: center;
  margin-bottom: 16px;
  color: var(--patent-purple) !important;
  font-size: 13px;
  font-weight: 750;
  text-decoration: none !important;
}

.back-to-patents:hover {
  color: var(--patent-purple-dark) !important;
}

.damage-patent-hero {
  padding: 31px 35px;
  background: linear-gradient(
    135deg,
    var(--patent-purple),
    var(--patent-purple-dark)
  );
  border-radius: 12px;
  color: #ffffff;
  box-shadow: 0 10px 30px rgba(35, 20, 60, 0.13);
}

.damage-patent-hero h1 {
  margin: 0;
  color: #ffffff;
  font-size: clamp(32px, 4vw, 50px);
  font-weight: 780;
  letter-spacing: -0.03em;
  line-height: 1.15;
}

.damage-patent-hero p {
  margin: 9px 0 0;
  color: rgba(255, 255, 255, 0.84);
  font-size: 14px;
  line-height: 1.55;
}

.damage-patent-layout {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 310px;
  gap: 27px;
  align-items: start;
  margin-top: 29px;
}

.damage-main-card,
.damage-side-card,
.damage-related-card {
  background: #ffffff;
  border: 1px solid var(--patent-border);
  border-radius: 11px;
  box-shadow: 0 6px 22px rgba(28, 20, 50, 0.06);
}

.damage-main-card {
  overflow: hidden;
}

.damage-image-area {
  padding: 18px;
  background: #f4f6fa;
  border-bottom: 1px solid var(--patent-border);
}

.damage-image-button {
  display: block;
  width: 100%;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background: #ffffff;
  border: 1px solid #cfd4df;
  border-radius: 8px;
  box-shadow: 0 6px 20px rgba(28, 20, 50, 0.08);
  cursor: zoom-in;
}

.damage-image-button img {
  display: block;
  width: 100%;
  height: auto;
  margin: 0;
}

.damage-image-note {
  margin: 10px 0 0;
  color: var(--patent-muted);
  font-size: 11px;
  line-height: 1.45;
  text-align: center;
}

.damage-patent-content {
  padding: 23px;
}

.damage-topline {
  display: flex;
  gap: 12px;
  align-items: flex-start;
  justify-content: space-between;
  margin-bottom: 13px;
}

.damage-patent-number {
  color: var(--patent-purple);
  font-size: 12px;
  font-weight: 830;
  letter-spacing: 0.055em;
  text-transform: uppercase;
}

.damage-status {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-width: 78px;
  padding: 6px 10px;
  background: #edf7ee;
  border: 1px solid #cde8d0;
  border-radius: 999px;
  color: #2e7d32;
  font-size: 11px;
  font-weight: 820;
  line-height: 1;
}

.damage-title {
  margin: 0 0 17px;
  color: var(--patent-text);
  font-size: clamp(24px, 2.7vw, 33px);
  font-weight: 780;
  line-height: 1.3;
}

.damage-metadata {
  display: grid;
  grid-template-columns: 125px minmax(0, 1fr);
  gap: 9px 16px;
  margin: 0;
}

.damage-metadata dt {
  margin: 0;
  color: var(--patent-purple);
  font-size: 12px;
  font-weight: 820;
  line-height: 1.55;
}

.damage-metadata dd {
  margin: 0;
  color: var(--patent-text);
  font-size: 13px;
  line-height: 1.55;
}

.damage-side-card {
  position: sticky;
  top: 90px;
  padding: 22px;
}

.damage-side-card h2 {
  margin: 0 0 15px;
  color: var(--patent-purple);
  font-size: 20px;
  font-weight: 780;
}

.damage-document-button {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  min-height: 51px;
  padding: 11px 14px;
  background: var(--patent-purple);
  border: 1px solid var(--patent-purple);
  border-radius: 8px;
  color: #ffffff !important;
  font-size: 13px;
  font-weight: 760;
  line-height: 1.35;
  text-decoration: none !important;
  transition:
    background-color 0.2s ease,
    border-color 0.2s ease,
    transform 0.2s ease;
}

.damage-document-button:hover {
  background: var(--patent-purple-dark);
  border-color: var(--patent-purple-dark);
  transform: translateY(-1px);
}

.damage-side-note {
  margin: 15px 0 0;
  padding-top: 14px;
  border-top: 1px solid var(--patent-border);
  color: var(--patent-muted);
  font-size: 11px;
  line-height: 1.55;
}

.damage-related-card {
  margin-top: 31px;
  padding: 24px;
}

.damage-related-card h2 {
  margin: 0 0 18px;
  padding-bottom: 12px;
  border-bottom: 3px solid var(--patent-purple);
  color: var(--patent-purple);
  font-size: 24px;
  font-weight: 780;
}

.damage-related-empty {
  margin: 0;
  color: var(--patent-muted);
  font-size: 13px;
  line-height: 1.6;
}

/* Full-screen image viewer */

.damage-image-modal {
  position: fixed;
  inset: 0;
  z-index: 9999;
  display: none;
  align-items: center;
  justify-content: center;
  padding: 24px;
  background: rgba(15, 13, 23, 0.90);
}

.damage-image-modal.open {
  display: flex;
}

.damage-modal-sheet {
  position: relative;
  width: min(96vw, 1450px);
  max-height: 94vh;
  overflow: auto;
  background: #ffffff;
  border-radius: 7px;
  box-shadow: 0 22px 70px rgba(0, 0, 0, 0.42);
}

.damage-modal-sheet img {
  display: block;
  width: 100%;
  height: auto;
  margin: 0;
}

.damage-modal-close {
  position: sticky;
  top: 12px;
  float: right;
  z-index: 2;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  margin: 12px 12px -52px 0;
  padding: 0;
  background: rgba(50, 16, 95, 0.94);
  border: 0;
  border-radius: 50%;
  color: #ffffff;
  cursor: pointer;
  font-size: 25px;
  line-height: 1;
}

@media screen and (max-width: 1000px) {
  .damage-patent-layout {
    grid-template-columns: 1fr;
  }

  .damage-side-card {
    position: static;
  }
}

@media screen and (max-width: 700px) {
  .post,
  .post-content,
  .container {
    width: 94% !important;
  }

  .damage-patent-hero {
    padding: 24px 22px;
  }

  .damage-patent-content,
  .damage-related-card {
    padding: 19px;
  }

  .damage-metadata {
    grid-template-columns: 1fr;
    gap: 3px;
  }

  .damage-metadata dd {
    margin-bottom: 8px;
  }

  .damage-image-modal {
    padding: 8px;
  }
}
</style>

<div class="damage-patent-page">

  <a
    class="back-to-patents"
    href="{{ '/patents/' | relative_url }}"
  >
    ← Back to Patents
  </a>

  <header class="damage-patent-hero">

    <h1>Damage Assessment of Tribo-Systems</h1>

    <p>
      U.S. patent on thermodynamics-based degradation and damage assessment
      for tribological systems.
    </p>

  </header>

  <div class="damage-patent-layout">

    <main class="damage-main-card">

      <section class="damage-image-area">

        <button
          class="damage-image-button"
          id="open-damage-image"
          type="button"
          aria-label="Open a large view of the Damage Assessment patent image"
        >

          <img
            src="{{ '/assets/img/patents/damage_assessment.png' | relative_url }}"
            alt="Damage Assessment of Tribo-Systems patent overview"
          >

        </button>

        <p class="damage-image-note">
          Click the image to open a large view.
        </p>

      </section>

      <section class="damage-patent-content">

        <div class="damage-topline">

          <span class="damage-patent-number">
            US 11,488,420 B2
          </span>

          <span class="damage-status">
            Granted
          </span>

        </div>

        <h2 class="damage-title">
          Damage Assessment of Tribo-Systems
        </h2>

        <dl class="damage-metadata">

          <dt>Inventors</dt>
          <dd>M. M. Khonsari and Lijesh K. P.</dd>

          <dt>Jurisdiction</dt>
          <dd>United States</dd>

          <dt>Patent No.</dt>
          <dd>US 11,488,420 B2</dd>

          <dt>Status</dt>
          <dd>Granted</dd>

          <dt>Year</dt>
          <dd>2022</dd>

        </dl>

      </section>

    </main>

    <aside class="damage-side-card">

      <h2>Patent Document</h2>

      <a
        class="damage-document-button"
        href="{{ '/assets/pdf/patents/damage_assessment.pdf' | relative_url }}"
        target="_blank"
        rel="noopener noreferrer"
      >
        View Full Patent Document ↗
      </a>

      <p class="damage-side-note">
        The complete patent document opens in a separate browser tab.
      </p>

    </aside>

  </div>

  <section class="damage-related-card">

    <h2>Related Publications</h2>

    <p class="damage-related-empty">
      Related publications will be added here.
    </p>

  </section>

</div>

<div
  class="damage-image-modal"
  id="damage-image-modal"
  role="dialog"
  aria-modal="true"
  aria-label="Large view of the Damage Assessment patent image"
>

  <div class="damage-modal-sheet">

    <button
      class="damage-modal-close"
      id="close-damage-image"
      type="button"
      aria-label="Close image viewer"
    >
      ×
    </button>

    <img
      src="{{ '/assets/img/patents/damage_assessment.png' | relative_url }}"
      alt="Large view of the Damage Assessment of Tribo-Systems patent overview"
    >

  </div>

</div>

<script>
document.addEventListener("DOMContentLoaded", function () {

  const openButton =
    document.getElementById("open-damage-image");

  const closeButton =
    document.getElementById("close-damage-image");

  const modal =
    document.getElementById("damage-image-modal");

  if (!openButton || !closeButton || !modal) {
    return;
  }

  function openModal() {
    modal.classList.add("open");
    document.body.style.overflow = "hidden";
    closeButton.focus();
  }

  function closeModal() {
    modal.classList.remove("open");
    document.body.style.overflow = "";
    openButton.focus();
  }

  openButton.addEventListener("click", openModal);

  closeButton.addEventListener("click", closeModal);

  modal.addEventListener("click", function (event) {
    if (event.target === modal) {
      closeModal();
    }
  });

  document.addEventListener("keydown", function (event) {
    if (
      event.key === "Escape" &&
      modal.classList.contains("open")
    ) {
      closeModal();
    }
  });

});
</script>

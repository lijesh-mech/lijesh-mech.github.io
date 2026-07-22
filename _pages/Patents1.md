---
layout: page
title: Patents
permalink: /patents/
nav: false
nav_order: 5
description: "Granted and filed patents of Dr. Lijesh Koottaparambil"
---

<style>
:root{
  --purple:#461d7c;--purple-dark:#32105f;--purple-soft:#f6f2fb;
  --gold:#fdd023;--text:#242433;--muted:#666678;--border:#e1e1e8;
}
.post,.post-content,.container{width:95%!important;max-width:1450px!important}
.post-header>h1,.post-header>.post-description{display:none!important}
.patents-page{width:100%;margin:34px auto 70px;color:var(--text)}
.patents-hero{padding:32px 36px;background:linear-gradient(135deg,#461d7c,#32105f);
border-radius:12px;box-shadow:0 10px 30px rgba(35,20,60,.13)}
.patents-hero h1{margin:0;color:#fff;font-size:clamp(34px,4vw,52px);
font-weight:760;letter-spacing:-.03em}
.patent-section{margin-top:42px}
.patent-section-header{display:flex;gap:14px;align-items:center;margin-bottom:22px;
padding-bottom:13px;border-bottom:3px solid var(--purple)}
.patent-section-icon{display:inline-flex;align-items:center;justify-content:center;
width:42px;height:42px;flex:0 0 42px;background:var(--purple-soft);
border:1px solid rgba(70,29,124,.18);border-radius:50%;color:var(--purple)}
.patent-section-icon svg{width:22px;height:22px;fill:none;stroke:currentColor;
stroke-width:1.9;stroke-linecap:round;stroke-linejoin:round}
.patent-section-heading h2{margin:0;color:var(--purple);font-size:28px;font-weight:750}
.patent-section-heading p{margin:4px 0 0;color:var(--muted);font-size:13px}
.patent-grid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:24px}
.patent-card{overflow:hidden;background:#fff;border:1px solid var(--border);
border-radius:11px;box-shadow:0 6px 22px rgba(28,20,50,.06);
transition:.2s ease}
.patent-card:hover{border-color:rgba(70,29,124,.32);
box-shadow:0 10px 28px rgba(28,20,50,.10);transform:translateY(-2px)}
.patent-preview{width:100%;height:520px;overflow:hidden;background:#f0f1f5;
border-bottom:1px solid var(--border)}
.patent-preview iframe{display:block;width:100%;height:100%;border:0;background:#fff}
.patent-content{padding:21px 22px 22px}
.patent-topline{display:flex;gap:12px;align-items:flex-start;
justify-content:space-between;margin-bottom:12px}
.patent-number{color:var(--purple);font-size:12px;font-weight:800;
letter-spacing:.06em;text-transform:uppercase}
.patent-status{display:inline-flex;align-items:center;justify-content:center;
min-width:78px;padding:6px 10px;border-radius:999px;font-size:11px;
font-weight:800;line-height:1}
.patent-status.granted{background:#edf7ee;border:1px solid #cde8d0;color:#2e7d32}
.patent-status.filed{background:#fff7df;border:1px solid #f0d998;color:#9a6700}
.patent-title{margin:0 0 14px;color:var(--text);font-size:21px;font-weight:750;
line-height:1.35}
.patent-metadata{display:grid;grid-template-columns:106px minmax(0,1fr);
gap:8px 13px;margin:0}
.patent-metadata dt{margin:0;color:var(--purple);font-size:12px;font-weight:800;line-height:1.55}
.patent-metadata dd{margin:0;color:var(--text);font-size:13px;line-height:1.55}
.patent-actions{display:flex;flex-wrap:wrap;gap:10px;margin-top:18px}
.patent-button{display:inline-flex;gap:7px;align-items:center;justify-content:center;
padding:9px 13px;background:var(--purple);border:1px solid var(--purple);
border-radius:7px;color:#fff!important;font-size:12px;font-weight:750;
text-decoration:none!important}
.patent-button:hover{background:var(--purple-dark);border-color:var(--purple-dark)}
.patent-divider{position:relative;height:1px;margin:56px 0 8px;
background:linear-gradient(to right,transparent,rgba(70,29,124,.42),transparent)}
.patent-divider:after{position:absolute;top:50%;left:50%;width:46px;height:5px;
background:var(--gold);border-radius:999px;content:"";transform:translate(-50%,-50%)}
.filed-patent-grid{grid-template-columns:minmax(0,720px);justify-content:center}
@media(max-width:1100px){.patent-grid{grid-template-columns:1fr}.patent-preview{height:650px}}
@media(max-width:700px){
  .post,.post-content,.container{width:94%!important}
  .patents-hero{padding:25px 23px}.patent-preview{height:500px}
  .patent-content{padding:18px 17px 19px}.patent-title{font-size:18px}
  .patent-metadata{grid-template-columns:1fr;gap:3px}
  .patent-metadata dd{margin-bottom:8px}
}
@media(max-width:470px){.patent-preview{height:410px}}

/* Image-based patent preview */
.patent-image-preview{
  padding:16px;
  background:#f4f6fa;
  border-bottom:1px solid var(--border);
}
.patent-image-button{
  display:block;
  width:100%;
  margin:0;
  padding:0;
  overflow:hidden;
  background:#fff;
  border:1px solid #cfd4df;
  border-radius:8px;
  box-shadow:0 5px 18px rgba(28,20,50,.08);
  cursor:zoom-in;
}
.patent-image-button img{
  display:block;
  width:100%;
  height:auto;
  margin:0;
}
.patent-image-hint{
  margin:9px 0 0;
  color:var(--muted);
  font-size:11px;
  line-height:1.45;
  text-align:center;
}
.related-publication-block{
  margin-top:22px;
  padding-top:18px;
  border-top:1px solid var(--border);
}
.related-publication-block h4{
  margin:0 0 12px;
  color:var(--purple);
  font-size:16px;
  font-weight:780;
}
.related-publication-item{
  padding:13px 14px;
  background:var(--purple-soft);
  border:1px solid rgba(70,29,124,.18);
  border-radius:8px;
}
.related-publication-item h5{
  margin:0 0 6px;
  color:var(--text);
  font-size:14px;
  font-weight:750;
  line-height:1.45;
}
.related-publication-item p{
  margin:0 0 4px;
  color:var(--muted);
  font-size:12px;
  line-height:1.5;
}
.related-publication-item .journal{
  color:var(--purple);
  font-style:italic;
}
.related-publication-actions{
  display:flex;
  flex-wrap:wrap;
  gap:8px;
  margin-top:11px;
}
.publication-button{
  display:inline-flex;
  align-items:center;
  justify-content:center;
  padding:8px 11px;
  background:#fff;
  border:1px solid rgba(70,29,124,.28);
  border-radius:7px;
  color:var(--purple)!important;
  font-size:11px;
  font-weight:750;
  text-decoration:none!important;
}
.publication-button:hover{
  background:var(--purple);
  color:#fff!important;
}

/* Full-screen image viewer */
.patent-image-modal{
  position:fixed;
  inset:0;
  z-index:9999;
  display:none;
  align-items:center;
  justify-content:center;
  padding:24px;
  background:rgba(15,13,23,.9);
}
.patent-image-modal.open{display:flex}
.patent-image-modal-sheet{
  position:relative;
  width:min(96vw,1450px);
  max-height:94vh;
  overflow:auto;
  background:#fff;
  border-radius:7px;
  box-shadow:0 22px 70px rgba(0,0,0,.42);
}
.patent-image-modal-sheet img{
  display:block;
  width:100%;
  height:auto;
  margin:0;
}
.patent-image-modal-close{
  position:sticky;
  top:12px;
  float:right;
  z-index:2;
  display:flex;
  align-items:center;
  justify-content:center;
  width:40px;
  height:40px;
  margin:12px 12px -52px 0;
  padding:0;
  background:rgba(50,16,95,.94);
  border:0;
  border-radius:50%;
  color:#fff;
  cursor:pointer;
  font-size:25px;
  line-height:1;
}
@media(max-width:700px){
  .patent-image-modal{padding:8px}
  .related-publication-actions{flex-direction:column}
  .publication-button{width:100%}
}

</style>

<div class="patents-page">
  <header class="patents-hero"><h1>Patents</h1></header>

  <section class="patent-section">
    <div class="patent-section-header">
      <span class="patent-section-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24"><path d="m12 3 2.2 4.5 5 .7-3.6 3.5.9 5-4.5-2.4-4.5 2.4.9-5-3.6-3.5 5-.7L12 3z"/></svg>
      </span>
      <div class="patent-section-heading">
        <h2>Granted Patents</h2>
        <p>Granted U.S. and Indian patents</p>
      </div>
    </div>

<div class="patent-grid">

  <article class="patent-card">
    <div class="patent-preview">
      <iframe
        src="{{ '/assets/pdf/patents/damage_assessment.pdf' | relative_url }}#page=1&view=FitH"
        title="First page of Damage Assessment of Tribo-Systems"
        loading="lazy">
      </iframe>
    </div>

    <div class="patent-content">
      <div class="patent-topline">
        <span class="patent-number">US 11,488,420 B2</span>
        <span class="patent-status granted">Granted</span>
      </div>

      <h3 class="patent-title">Damage Assessment of Tribo-Systems</h3>

      <dl class="patent-metadata">
        
        <dt>Inventors</dt><dd>M. M. Khonsari and Lijesh K. P.</dd>
        <dt>Jurisdiction</dt><dd>United States</dd>
        <dt>Patent No.</dt><dd>US 11,488,420 B2</dd>
        <dt>Year</dt><dd>2022</dd>
      </dl>

      <div class="patent-actions">
        <a class="patent-button"
           href="{{ '/assets/pdf/patents/damage_assessment.pdf' | relative_url }}"
           target="_blank"
           rel="noopener noreferrer">
          View Patent Document ↗
        </a>
      </div>
    </div>
  </article>


  <article class="patent-card">
    <div class="patent-preview">
      <iframe
        src="{{ '/assets/pdf/patents/grease_evaluation.pdf' | relative_url }}#page=1&view=FitH"
        title="First page of Grease Evaluation Using Contact Angle"
        loading="lazy">
      </iframe>
    </div>

    <div class="patent-content">
      <div class="patent-topline">
        <span class="patent-number">US 2022/0074916</span>
        <span class="patent-status granted">Granted</span>
      </div>

      <h3 class="patent-title">Grease Evaluation Using Contact Angle</h3>

      <dl class="patent-metadata">
        
        <dt>Inventors</dt><dd>M. M. Khonsari and Lijesh K. P.</dd>
        <dt>Jurisdiction</dt><dd>United States</dd>
        <dt>Publication No.</dt><dd>US 2022/0074916</dd>
        <dt>Year</dt><dd>2023</dd>
      </dl>

      <div class="patent-actions">
        <a class="patent-button"
           href="{{ '/assets/pdf/patents/grease_evaluation.pdf' | relative_url }}"
           target="_blank"
           rel="noopener noreferrer">
          View Patent Document ↗
        </a>
      </div>
    </div>
  </article>


  <article class="patent-card">
    <div class="patent-preview">
      <iframe
        src="{{ '/assets/pdf/patents/peanut_butter_evaluation.pdf' | relative_url }}#page=1&view=FitH"
        title="First page of Food Evaluation"
        loading="lazy">
      </iframe>
    </div>

    <div class="patent-content">
      <div class="patent-topline">
        <span class="patent-number">US 11,994,505 B2</span>
        <span class="patent-status granted">Granted</span>
      </div>

      <h3 class="patent-title">Food Evaluation</h3>

      <dl class="patent-metadata">
        <dt>Technology</dt><dd>Peanut Butter Evaluation</dd>
        <dt>Inventors</dt><dd>M. M. Khonsari and Lijesh K. P.</dd>
        <dt>Jurisdiction</dt><dd>United States</dd>
        <dt>Patent No.</dt><dd>US 11,994,505 B2</dd>
        <dt>Year</dt><dd>2024</dd>
      </dl>

      <div class="patent-actions">
        <a class="patent-button"
           href="{{ '/assets/pdf/patents/peanut_butter_evaluation.pdf' | relative_url }}"
           target="_blank"
           rel="noopener noreferrer">
          View Patent Document ↗
        </a>
      </div>
    </div>
  </article>


  <article class="patent-card">
    <div class="patent-preview">
      <iframe
        src="{{ '/assets/pdf/patents/fluid_monitoring_grease.pdf' | relative_url }}#page=1&view=FitH"
        title="First page of Fluid Monitoring for Grease"
        loading="lazy">
      </iframe>
    </div>

    <div class="patent-content">
      <div class="patent-topline">
        <span class="patent-number">US 12,000,821 B2</span>
        <span class="patent-status granted">Granted</span>
      </div>

      <h3 class="patent-title">Fluid Monitoring for Grease</h3>

      <dl class="patent-metadata">
        
        <dt>Inventors</dt><dd>M. M. Khonsari and Lijesh K. P.</dd>
        <dt>Jurisdiction</dt><dd>United States</dd>
        <dt>Patent No.</dt><dd>US 12,000,821 B2</dd>
        <dt>Year</dt><dd>2024</dd>
      </dl>

      <div class="patent-actions">
        <a class="patent-button"
           href="{{ '/assets/pdf/patents/fluid_monitoring_grease.pdf' | relative_url }}"
           target="_blank"
           rel="noopener noreferrer">
          View Patent Document ↗
        </a>
      </div>
    </div>
  </article>


  <article class="patent-card">
    <div class="patent-preview">
      <iframe
        src="{{ '/assets/pdf/patents/fluid_monitoring_food.pdf' | relative_url }}#page=1&view=FitH"
        title="First page of Fluid Monitoring for Food"
        loading="lazy">
      </iframe>
    </div>

    <div class="patent-content">
      <div class="patent-topline">
        <span class="patent-number">US 12,298,293 B2</span>
        <span class="patent-status granted">Granted</span>
      </div>

      <h3 class="patent-title">Fluid Monitoring for Food</h3>

      <dl class="patent-metadata">
        
        <dt>Inventors</dt><dd>M. M. Khonsari and Lijesh K. P.</dd>
        <dt>Jurisdiction</dt><dd>United States</dd>
        <dt>Patent No.</dt><dd>US 12,298,293 B2</dd>
        <dt>Year</dt><dd>2025</dd>
      </dl>

      <div class="patent-actions">
        <a class="patent-button"
           href="{{ '/assets/pdf/patents/fluid_monitoring_food.pdf' | relative_url }}"
           target="_blank"
           rel="noopener noreferrer">
          View Patent Document ↗
        </a>
      </div>
    </div>
  </article>
  <article class="patent-card">

    <div class="patent-image-preview">
      <button
        class="patent-image-button"
        id="open-multi-material-image"
        type="button"
        aria-label="Open a large view of the Multi-Material Smart Structure image"
      >
        <img
          src="{{ '/assets/img/patents/multi_material_smart_structure.png' | relative_url }}"
          alt="Multi-Material Smart Structure patent overview"
        >
      </button>

      <p class="patent-image-hint">
        Click the image to open a large view.
      </p>
    </div>

    <div class="patent-content">

      <div class="patent-topline">
        <span class="patent-number">Indian Patent No. 505929</span>
        <span class="patent-status granted">Granted</span>
      </div>

      <h3 class="patent-title">
        Multi Material Structure with Controllable Multi Directional Property
      </h3>

      <dl class="patent-metadata">
        <dt>Application No.</dt><dd>201741027226</dd>
        <dt>Filing Date</dt><dd>August 1, 2017</dd>
        <dt>Publication Date</dt><dd>February 8, 2019</dd>
        <dt>Patent No.</dt><dd>505929</dd>
        <dt>Applicant</dt><dd>National Institute of Technology Karnataka</dd>
        <dt>Inventors</dt>
        <dd>
          K. V. Gangadharan, Rohit Rajpal, Lijesh K. P.,
          M. P. Arunkumar, and Susheel Kumar
        </dd>
      </dl>

      <div class="patent-actions">
        <a
          class="patent-button"
          href="{{ '/assets/pdf/patents/multi_material_smart_structure_doc.pdf' | relative_url }}"
          target="_blank"
          rel="noopener noreferrer"
        >
          View Full Patent Document ↗
        </a>
      </div>

      <section class="related-publication-block">
        <h4>Related Publications</h4>

        <article class="related-publication-item">
          <h5>
            Parametric Studies on Bending Stiffness and Damping Ratio
            of Sandwich Structures
          </h5>

          <p>Rohit Rajpal, Lijesh K. P., and K. V. Gangadharan</p>
          <p class="journal">Additive Manufacturing (2018)</p>

          <div class="related-publication-actions">

    <a
      class="publication-button"
      href="https://doi.org/10.1016/j.addma.2018.05.039"
      target="_blank"
      rel="noopener noreferrer">

      View on Journal Website ↗

    </a>

  </div>
  </article>
      </section>

    </div>
  </article>


  <article class="patent-card">
    <div class="patent-preview">
      <iframe
        src="{{ '/assets/pdf/patents/stator_design_patent.pdf' | relative_url }}#page=1&view=FitH"
        title="First page of Stator Design Patent for Magnetic Bearing"
        loading="lazy">
      </iframe>
    </div>

    <div class="patent-content">
      <div class="patent-topline">
        <span class="patent-number">Indian Design Patent 259883</span>
        <span class="patent-status granted">Granted</span>
      </div>

      <h3 class="patent-title">Stator Design Patent for Magnetic Bearing</h3>

      <dl class="patent-metadata">
        <dt>Institution</dt><dd>Indian Institute of Technology Delhi</dd>
        <dt>Inventors</dt><dd>Harish Hirani and Lijesh K. P.</dd>
        <dt>Jurisdiction</dt><dd>India</dd>
        <dt>Design No.</dt><dd>259883</dd>
        <dt>Year</dt><dd>2014</dd>
      </dl>

      <div class="patent-actions">
        <a class="patent-button"
           href="{{ '/assets/pdf/patents/stator_design_patent.pdf' | relative_url }}"
           target="_blank"
           rel="noopener noreferrer">
          View Patent Document ↗
        </a>
      </div>
    </div>
  </article>

</div>

  </section>

  <div class="patent-divider" aria-hidden="true"></div>

  <section class="patent-section">
    <div class="patent-section-header">
      <span class="patent-section-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24"><path d="M6 2h9l4 4v16H6z"/><path d="M14 2v5h5"/><path d="M9 12h6M9 16h6"/></svg>
      </span>
      <div class="patent-section-heading">
        <h2>Filed Patents</h2>
        <p>Patent applications currently filed</p>
      </div>
    </div>

<div class="patent-grid filed-patent-grid">

  <article class="patent-card">
    <div class="patent-preview">
      <iframe
        src="{{ '/assets/pdf/patents/battery_remaining_discharge.pdf' | relative_url }}#page=1&view=FitH"
        title="First page of Battery Remaining Discharge patent application"
        loading="lazy">
      </iframe>
    </div>

    <div class="patent-content">
      <div class="patent-topline">
        <span class="patent-number">Serial No. 63/827,104</span>
        <span class="patent-status filed">Filed</span>
      </div>

      <h3 class="patent-title">Battery Remaining Discharge</h3>

      <dl class="patent-metadata">
        <dt>Inventors</dt><dd>M. M. Khonsari and Lijesh K. P.</dd>
        <dt>Jurisdiction</dt><dd>United States</dd>
        <dt>LSU Reference</dt><dd>LSU-2025-045-01</dd>
        <dt>Serial No.</dt><dd>63/827,104</dd>
        <dt>Filing Date</dt><dd>June 20, 2025</dd>
      </dl>

      <div class="patent-actions">
        <a class="patent-button"
           href="{{ '/assets/pdf/patents/battery_remaining_discharge.pdf' | relative_url }}"
           target="_blank"
           rel="noopener noreferrer">
          View Filed Patent Document ↗
        </a>
      </div>
    </div>
  </article>

</div>

  </section>
</div>

<div
  class="patent-image-modal"
  id="multi-material-image-modal"
  role="dialog"
  aria-modal="true"
  aria-label="Large view of the Multi-Material Smart Structure patent image"
>
  <div class="patent-image-modal-sheet">
    <button
      class="patent-image-modal-close"
      id="close-multi-material-image"
      type="button"
      aria-label="Close image viewer"
    >
      ×
    </button>

<img
  src="{{ '/assets/img/patents/multi_material_smart_structure.png' | relative_url }}"
  alt="Large view of the Multi-Material Smart Structure patent overview"
>

  </div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const openButton = document.getElementById("open-multi-material-image");
  const closeButton = document.getElementById("close-multi-material-image");
  const modal = document.getElementById("multi-material-image-modal");

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
    if (event.key === "Escape" && modal.classList.contains("open")) {
      closeModal();
    }
  });
});
</script>

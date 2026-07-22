---
layout: page
title: "Battery Remaining Discharge"
permalink: /patents/battery-remaining-discharge/
nav: false
description: "A filed U.S. patent application concerning battery remaining-discharge assessment."
---

<style>
:root{
  --p:#461d7c;
  --pd:#32105f;
  --ps:#f6f2fb;
  --g:#fdd023;
  --t:#161622;
  --m:#3f3f4c;
  --b:#d8d8e2;
}
.post,.post-content,.container{
  width:95%!important;
  max-width:1450px!important;
}
.post-header>h1,
.post-header>.post-description{
  display:none!important;
}
.detail-wrap{
  width:100%;
  margin:34px auto 70px;
  color:var(--t);
}
.back-link{
  display:inline-flex;
  margin-bottom:14px;
  color:var(--p)!important;
  font-size:13px;
  font-weight:760;
  text-decoration:none!important;
}
.detail-hero{
  padding:30px 34px;
  background:linear-gradient(135deg,var(--p),var(--pd));
  border-radius:12px;
  color:#fff;
}
.detail-hero h1{
  margin:0;
  color:#fff;
  font-size:clamp(31px,4vw,49px);
  font-weight:800;
  letter-spacing:-.03em;
}
.detail-grid{
  display:grid;
  grid-template-columns:minmax(0,1fr) 330px;
  gap:26px;
  margin-top:28px;
  align-items:start;
}
.main,
.side{
  background:#fff;
  border:1px solid var(--b);
  border-radius:11px;
  box-shadow:0 6px 22px rgba(28,20,50,.07);
}
.main{
  overflow:hidden;
}
.image-area{
  padding:18px;
  background:#f3f5f9;
  border-bottom:1px solid var(--b);
}
.image-button{
  display:block;
  width:100%;
  padding:0;
  border:1px solid #c7cbd5;
  border-radius:8px;
  overflow:hidden;
  background:#fff;
  cursor:zoom-in;
}
.image-button img{
  display:block;
  width:100%;
  height:auto;
  margin:0;
}
.hint{
  margin:9px 0 0;
  color:var(--m);
  font-size:11px;
  text-align:center;
}
.content{
  padding:23px;
}
.topline{
  display:flex;
  justify-content:space-between;
  gap:12px;
  align-items:flex-start;
  margin-bottom:14px;
}
.number{
  color:var(--p);
  font-size:16px;
  font-weight:900;
  text-transform:uppercase;
  letter-spacing:.055em;
}
.status{
  min-width:104px;
  padding:9px 16px;
  border-radius:999px;
  font-size:14px;
  font-weight:900;
  text-align:center;
}
.status.filed{
  background:#fff4d6;
  border:1px solid #e7ca79;
  color:#8a5a00;
}
.title{
  margin:0 0 18px;
  color:var(--t);
  font-size:clamp(24px,2.5vw,33px);
  font-weight:800;
  line-height:1.28;
}
.meta{
  display:grid;
  grid-template-columns:125px minmax(0,1fr);
  gap:9px 15px;
  margin:0;
}
.meta dt{
  color:var(--p);
  font-size:12px;
  font-weight:850;
}
.meta dd{
  margin:0;
  color:var(--t);
  font-size:13px;
  line-height:1.55;
}
.side{
  position:sticky;
  top:90px;
  padding:22px;
}
.side h2{
  margin:0 0 15px;
  color:var(--p);
  font-size:20px;
  font-weight:800;
}
.action{
  display:flex;
  align-items:center;
  justify-content:center;
  width:100%;
  min-height:52px;
  padding:11px 13px;
  background:var(--p);
  border:1px solid var(--p);
  border-radius:8px;
  color:#fff!important;
  font-size:13px;
  font-weight:780;
  text-decoration:none!important;
}
.action:hover{
  background:var(--pd);
}
.related-inline{
  margin-top:24px;
  padding-top:20px;
  border-top:1px solid var(--b);
}
.related-inline h2{
  margin:0 0 16px;
  color:var(--p);
  font-size:22px;
  font-weight:800;
}
.pub-list{
  display:flex;
  flex-direction:column;
  gap:14px;
}
.pub{
  padding:15px 16px;
  background:var(--ps);
  border:1px solid rgba(70,29,124,.18);
  border-radius:8px;
}
.pub h3{
  margin:0 0 7px;
  color:var(--t);
  font-size:15px;
  font-weight:780;
  line-height:1.45;
}
.pub p{
  margin:0 0 5px;
  color:var(--m);
  font-size:12px;
  line-height:1.52;
}
.pub .journal{
  color:var(--p);
  font-style:italic;
}
.journal-link{
  display:inline-flex;
  margin-top:9px;
  padding:9px 12px;
  background:var(--p);
  border:1px solid var(--p);
  border-radius:7px;
  color:#fff!important;
  font-size:11px;
  font-weight:780;
  text-decoration:none!important;
}
.journal-link:hover{
  background:var(--pd);
  border-color:var(--pd);
}
.modal{
  position:fixed;
  inset:0;
  z-index:9999;
  display:none;
  align-items:center;
  justify-content:center;
  padding:24px;
  background:rgba(15,13,23,.9);
}
.modal.open{
  display:flex;
}
.sheet{
  position:relative;
  width:min(96vw,1450px);
  max-height:94vh;
  overflow:auto;
  background:#fff;
  border-radius:7px;
}
.sheet img{
  display:block;
  width:100%;
  height:auto;
  margin:0;
}
.close{
  position:sticky;
  top:12px;
  float:right;
  z-index:2;
  width:40px;
  height:40px;
  margin:12px 12px -52px 0;
  border:0;
  border-radius:50%;
  background:rgba(50,16,95,.94);
  color:#fff;
  font-size:25px;
  cursor:pointer;
}
@media(max-width:1000px){
  .detail-grid{
    grid-template-columns:1fr;
  }
  .side{
    position:static;
  }
}
@media(max-width:680px){
  .post,.post-content,.container{
    width:94%!important;
  }
  .detail-hero{
    padding:24px 22px;
  }
  .meta{
    grid-template-columns:1fr;
    gap:3px;
  }
  .meta dd{
    margin-bottom:8px;
  }
  .modal{
    padding:8px;
  }
}
</style>

<div class="detail-wrap">

  <a class="back-link" href="{{ '/patents/' | relative_url }}">
    ← Back to Patents
  </a>

  <header class="detail-hero">
    <h1>Battery Remaining Discharge</h1>
  </header>

  <div class="detail-grid">

<main class="main">

  <div class="image-area">

    <button
      class="image-button"
      id="open-main-image"
      type="button"
      aria-label="Open large Battery Remaining Discharge patent image"
    >
      <img
        src="{{ '/assets/img/patents/battery_remaining_discharge.jpg' | relative_url }}"
        alt="Battery Remaining Discharge patent overview"
      >
    </button>

    <p class="hint">
      Click the image to open a large view.
    </p>

  </div>

  <div class="content">

    <div class="topline">
      <span class="number">Serial No. 63/827,104</span>
      <span class="status filed">Filed</span>
    </div>

    <h2 class="title">
      Battery Remaining Discharge
    </h2>

    <dl class="meta">
      <dt>Inventors</dt>
      <dd>M. M. Khonsari and Lijesh K. P.</dd>

      <dt>Jurisdiction</dt>
      <dd>United States</dd>

      <dt>LSU Reference</dt>
      <dd>LSU-2025-045-01</dd>

      <dt>Serial No.</dt>
      <dd>63/827,104</dd>

      <dt>Status</dt>
      <dd>Filed</dd>

      <dt>Filing Date</dt>
      <dd>June 20, 2025</dd>
    </dl>

  </div>

</main>

<aside class="side">

  <h2>Patent Document</h2>

  <a
    class="action"
    href="{{ '/assets/pdf/patents/battery_remaining_discharge.pdf' | relative_url }}"
    target="_blank"
    rel="noopener noreferrer"
  >
    View Filed Patent Document ↗
  </a>

  <section class="related-inline">

    <h2>Related Publications</h2>

    <div class="pub-list">

      <article class="pub">
        <h3>
          A Thermodynamic Framework to Rapidly Determine Remaining Discharge Time in Li-Ion Batteries
        </h3>
        <p>Lijesh, K. P., and M. M. Khonsari</p>
        <p class="journal">Journal of Power Sources 655 (2025): 237922</p>
        <a
          class="journal-link"
          href="https://doi.org/10.1016/j.jpowsour.2025.237922"
          target="_blank"
          rel="noopener noreferrer"
        >
          View on Journal Website ↗
        </a>
      </article>

      <article class="pub">
        <h3>
          A Thermodynamic Approach for the Rapid Estimation of the Remaining Time to Discharge in Li-Ion Batteries
        </h3>
        <p>Lijesh, K. P., and M. M. Khonsari</p>
        <p class="journal">
          Sustainable Energy Technologies and Assessments 82 (2025): 104490
        </p>
        <a
          class="journal-link"
          href="https://doi.org/10.1016/j.seta.2025.104490"
          target="_blank"
          rel="noopener noreferrer"
        >
          View on Journal Website ↗
        </a>
      </article>

      <article class="pub">
        <h3>
          A Thermodynamic Approach for Characterizing the Degradation of Li-Ion Batteries
        </h3>
        <p>Lijesh, K. P., and M. M. Khonsari</p>
        <p class="journal">Journal of Energy Storage 82 (2024): 110565</p>
        <a
          class="journal-link"
          href="https://doi.org/10.1016/j.est.2024.110565"
          target="_blank"
          rel="noopener noreferrer"
        >
          View on Journal Website ↗
        </a>
      </article>

    </div>

  </section>

</aside>

  </div>

</div>

<div
  class="modal"
  id="main-image-modal"
  role="dialog"
  aria-modal="true"
  aria-label="Large Battery Remaining Discharge patent image"
>

  <div class="sheet">

<button
  class="close"
  id="close-main-image"
  type="button"
  aria-label="Close image viewer"
>
  ×
</button>

<img
  src="{{ '/assets/img/patents/battery_remaining_discharge.jpg' | relative_url }}"
  alt="Large view of the Battery Remaining Discharge patent overview"
>

  </div>

</div>

<script>
document.addEventListener("DOMContentLoaded", function () {

  const openButton = document.getElementById("open-main-image");
  const closeButton = document.getElementById("close-main-image");
  const modal = document.getElementById("main-image-modal");

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

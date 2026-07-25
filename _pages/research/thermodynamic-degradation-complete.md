---
layout: page
title: "Thermodynamics-Based Degradation and Failure"
permalink: /research/thermodynamic-degradation/
nav: false
description: "A unified thermodynamic framework for quantifying degradation, predicting failure thresholds, and estimating remaining useful life."
---

<style>
:root{
  --p:#461d7c; --pd:#32105f; --ps:#f5f1fa; --g:#fdd023;
  --t:#171722; --m:#4c4c58; --b:#ddd9e6; --w:#fff; --s:#f7f7fa;
}
.post,.post-content,.container{width:95%!important;max-width:1480px!important}
.post-header>h1,.post-header>.post-description{display:none!important}
.research-page{width:100%;margin:32px auto 72px;color:var(--t)}
.breadcrumb{display:flex;gap:8px;align-items:center;margin-bottom:15px;font-size:13px;font-weight:700}
.breadcrumb a{color:var(--p)!important;text-decoration:none!important}
.hero{padding:38px;border-radius:14px;background:linear-gradient(135deg,var(--p),var(--pd));color:#fff;box-shadow:0 12px 32px rgba(50,16,95,.18)}
.hero-kicker{margin:0 0 8px;color:var(--g);font-size:13px;font-weight:900;letter-spacing:.12em;text-transform:uppercase}
.hero h1{margin:0;color:#fff;font-size:clamp(34px,5vw,58px);font-weight:850;letter-spacing:-.035em;line-height:1.08}
.hero p{max-width:960px;margin:16px 0 0;color:rgba(255,255,255,.91);font-size:clamp(15px,1.55vw,20px);line-height:1.65}
.section{margin-top:30px;padding:28px;background:var(--w);border:1px solid var(--b);border-radius:13px;box-shadow:0 7px 24px rgba(30,23,52,.065)}
.section-heading{display:flex;align-items:center;gap:12px;margin-bottom:19px}
.section-heading:before{content:"";width:7px;height:31px;border-radius:5px;background:var(--g)}
.section-heading h2{margin:0;color:var(--p);font-size:clamp(25px,3vw,34px);font-weight:850;letter-spacing:-.025em}
.overview-grid{display:grid;grid-template-columns:minmax(0,1.05fr) minmax(380px,.95fr);gap:30px;align-items:center}
.overview-copy p{margin:0 0 14px;color:var(--m);font-size:15px;line-height:1.78}
.image-card{padding:12px;background:var(--s);border:1px solid var(--b);border-radius:11px}
.image-button{display:block;width:100%;padding:0;border:0;background:transparent;cursor:zoom-in}
.image-button img{display:block;width:100%;height:auto;margin:0;border-radius:7px}
.image-note{margin:9px 0 0;color:var(--m);font-size:11px;text-align:center}
.tag-row{display:flex;flex-wrap:wrap;gap:8px;margin-top:19px}
.tag{padding:8px 11px;border:1px solid rgba(70,29,124,.25);border-radius:999px;background:var(--ps);color:var(--p);font-size:11px;font-weight:800}
.framework-copy{max-width:1080px;margin:18px auto 0;color:var(--m);font-size:14px;line-height:1.75;text-align:center}
.grid3{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:16px}
.card{padding:19px;border:1px solid var(--b);border-radius:10px;background:linear-gradient(180deg,#fff,var(--ps))}
.card .index{display:inline-flex;align-items:center;justify-content:center;width:34px;height:34px;margin-bottom:11px;border-radius:50%;background:var(--p);color:#fff;font-size:13px;font-weight:900}
.card h3{margin:0 0 8px;color:var(--t);font-size:17px;font-weight:800}
.card p{margin:0;color:var(--m);font-size:12.5px;line-height:1.6}
.validation-list{display:grid;grid-template-columns:repeat(5,minmax(0,1fr));gap:11px;margin-top:18px}
.validation-item{padding:13px;border-radius:8px;background:var(--ps);border:1px solid rgba(70,29,124,.18);text-align:center}
.validation-item strong{display:block;color:var(--p);font-size:13px}
.validation-item span{display:block;margin-top:4px;color:var(--m);font-size:10.5px;line-height:1.4}
.app-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:14px}
.app{padding:17px;border:1px solid var(--b);border-radius:9px;background:#fff}
.app h3{margin:0 0 7px;color:var(--p);font-size:15px;font-weight:820}
.app p{margin:0;color:var(--m);font-size:12px;line-height:1.55}
.pub-list{display:flex;flex-direction:column;gap:14px}
.pub{padding:17px 18px;border:1px solid rgba(70,29,124,.18);border-radius:9px;background:var(--ps)}
.pub h3{margin:0 0 7px;color:var(--t);font-size:15px;font-weight:800;line-height:1.47}
.pub p{margin:0 0 5px;color:var(--m);font-size:12px;line-height:1.5}
.pub .journal{color:var(--p);font-style:italic}
.pub-link,.patent a,.next-area a{display:inline-flex;padding:9px 12px;border-radius:7px;background:var(--p);color:#fff!important;font-size:11px;font-weight:800;text-decoration:none!important}
.pub-link:hover,.patent a:hover,.next-area a:hover{background:var(--pd)}
.patent-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:15px}
.patent{padding:19px;border:1px solid var(--b);border-radius:10px;background:#fff}
.patent h3{margin:0 0 8px;color:var(--t);font-size:17px;font-weight:820}
.patent p{margin:0 0 13px;color:var(--m);font-size:12px;line-height:1.55}
.next-area{display:flex;justify-content:space-between;gap:16px;align-items:center;margin-top:30px;padding:23px 25px;border-radius:12px;background:linear-gradient(135deg,var(--ps),#fff);border:1px solid rgba(70,29,124,.2)}
.next-area h2{margin:0;color:var(--p);font-size:21px;font-weight:850}
.next-area p{margin:5px 0 0;color:var(--m);font-size:12px}
.modal{position:fixed;inset:0;z-index:9999;display:none;align-items:center;justify-content:center;padding:20px;background:rgba(13,11,20,.91)}
.modal.open{display:flex}
.modal-sheet{position:relative;width:min(97vw,1600px);max-height:94vh;overflow:auto;border-radius:8px;background:#fff}
.modal-sheet img{display:block;width:100%;height:auto;margin:0}
.modal-close{position:sticky;top:12px;float:right;z-index:2;width:42px;height:42px;margin:12px 12px -54px 0;border:0;border-radius:50%;background:rgba(50,16,95,.95);color:#fff;font-size:27px;cursor:pointer}
@media(max-width:1080px){.overview-grid{grid-template-columns:1fr}.grid3,.app-grid{grid-template-columns:repeat(2,minmax(0,1fr))}.validation-list{grid-template-columns:repeat(3,minmax(0,1fr))}}
@media(max-width:760px){.hero{padding:29px 23px}.section{padding:21px}.grid3,.app-grid,.patent-grid,.validation-list{grid-template-columns:1fr}.next-area{flex-direction:column;align-items:flex-start}}
</style>

<div class="research-page">
  <div class="breadcrumb">
    <a href="{{ '/research/' | relative_url }}">Research</a><span>›</span>
    <span>Thermodynamics-Based Degradation and Failure</span>
  </div>

  <header class="hero">
    <p class="hero-kicker">Research Area 01</p>
    <h1>Thermodynamics-Based Degradation and Failure</h1>
    <p>A unified physics-based framework for quantifying irreversible degradation, comparing damage severity, identifying failure thresholds, and estimating the remaining life of materials and engineering systems.</p>
  </header>

  <section class="section">
    <div class="section-heading"><h2>Research Overview</h2></div>
    <div class="overview-grid">
      <div class="overview-copy">
        <p>Permanent degradation in engineering systems is inherently irreversible and dissipative. Conventional failure models are often empirical, mechanism-specific, and developed for idealized operating conditions, making them difficult to extend to complex systems exposed to variable loads, speeds, voltages, temperatures, or environmental conditions.</p>
        <p>This research uses irreversible thermodynamics to establish entropy generation as a common measure of degradation. The Degradation Entropy Generation framework connects measurable damage with the entropy generated by the dominant irreversible process. For a given material and degradation mechanism, accumulated entropy generation increases proportionately with damage, enabling degradation severity to be compared across different operating histories.</p>
        <p>Building on this foundation, the Failure Entropy Threshold represents the accumulated entropy generation at a user-defined or definitive failure state. The framework has been experimentally examined across mechanical, electrochemical, electrical, and energy-storage systems, including wear, corrosion, fatigue, resistor degradation, batteries, hydrogen-assisted degradation, polymers, composites, and manufacturing processes.</p>
        <div class="tag-row">
          <span class="tag">Degradation Entropy Generation</span>
          <span class="tag">Degradation Coefficient B</span>
          <span class="tag">Failure Entropy Threshold</span>
          <span class="tag">Remaining Useful Life</span>
          <span class="tag">Variable Operating Conditions</span>
        </div>
      </div>
      <div class="image-card">
        <button class="image-button" type="button" data-modal-target="overview-modal">
          <img src="{{ '/assets/img/research/research_topic_entropy.png' | relative_url }}" alt="Representative overview of thermodynamics-based degradation research">
        </button>
        <p class="image-note">Click the image to open a larger view.</p>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="section-heading"><h2>Degradation Entropy Generation Framework</h2></div>
    <div class="image-card">
      <button class="image-button" type="button" data-modal-target="deg-modal">
        <img src="{{ '/assets/img/research/deg_framework.png' | relative_url }}" alt="Degradation Entropy Generation framework">
      </button>
      <p class="image-note">Click the framework to open a larger view.</p>
    </div>
    <p class="framework-copy">The framework begins with the identification of the dominant irreversible process and its associated entropy-generation mechanism. The degradation coefficient links entropy generation to a measurable damage parameter. Accumulated entropy then provides a physics-based measure of degradation severity that increases proportionately with damage for a given material and mechanism under constant and variable operating conditions.</p>
  </section>

  <section class="section">
    <div class="section-heading"><h2>Key Scientific Contributions</h2></div>
    <div class="grid3">
      <article class="card"><span class="index">1</span><h3>Unified Degradation Measure</h3><p>Uses entropy generation as a common physical quantity for describing irreversible degradation across mechanical, chemical, electrical, and energy systems.</p></article>
      <article class="card"><span class="index">2</span><h3>Degradation Coefficient B</h3><p>Links entropy generation to a measurable damage variable and provides a mechanism-specific descriptor of degradation severity.</p></article>
      <article class="card"><span class="index">3</span><h3>Failure Entropy Threshold</h3><p>Defines failure through accumulated entropy generation at a user-defined or definitive failure state for a specified material and mechanism.</p></article>
      <article class="card"><span class="index">4</span><h3>Variable-Condition Prediction</h3><p>Accounts for changes in loading sequence, speed, voltage, frequency, temperature, and environmental severity that challenge conventional empirical models.</p></article>
      <article class="card"><span class="index">5</span><h3>Remaining-Life Assessment</h3><p>Uses accumulated entropy relative to the failure threshold to estimate degradation progression, failure time, and remaining useful life.</p></article>
      <article class="card"><span class="index">6</span><h3>Scale-Spanning Framework</h3><p>Supports integration of atomistic simulations, material experiments, component testing, and industrial process monitoring through a common thermodynamic description.</p></article>
    </div>
  </section>

  <section class="section">
    <div class="section-heading"><h2>Validation Across Diverse Systems</h2></div>
    <div class="image-card">
      <button class="image-button" type="button" data-modal-target="validation-modal">
        <img src="{{ '/assets/img/research/fet_validation_systems.png' | relative_url }}" alt="Failure Entropy Threshold validation across wear, corrosion, fatigue, resistor failure, and lithium-ion batteries">
      </button>
      <p class="image-note">Click the validation figure to open a larger view.</p>
    </div>
    <div class="validation-list">
      <div class="validation-item"><strong>Wear</strong><span>Dry, abrasive, and lubricated sliding</span></div>
      <div class="validation-item"><strong>Corrosion</strong><span>Electrochemical material loss</span></div>
      <div class="validation-item"><strong>Fatigue</strong><span>Constant and variable cyclic loading</span></div>
      <div class="validation-item"><strong>Electrical Failure</strong><span>Thermal-electrical resistor degradation</span></div>
      <div class="validation-item"><strong>Li-Ion Batteries</strong><span>Charge-discharge degradation and life assessment</span></div>
    </div>
  </section>

  <section class="section">
    <div class="section-heading"><h2>Application Domains</h2></div>
    <div class="app-grid">
      <article class="app"><h3>Tribology and Wear</h3><p>Adhesive, abrasive, fretting, lubricated, and multi-mechanism wear.</p></article>
      <article class="app"><h3>Corrosion and Tribocorrosion</h3><p>Electrochemical material loss under potential, flow, and coupled mechanical effects.</p></article>
      <article class="app"><h3>Fatigue and Fracture</h3><p>Cyclic loading, sequence effects, tensile damage, and remaining-life prediction.</p></article>
      <article class="app"><h3>Battery Degradation</h3><p>Li-ion battery health characterization and rapid remaining-discharge estimation.</p></article>
      <article class="app"><h3>Hydrogen Embrittlement</h3><p>Entropy-based quantification of hydrogen-assisted damage and cracking.</p></article>
      <article class="app"><h3>Manufacturing and Processing</h3><p>Entropy-based monitoring of grease, food, and other industrial production processes.</p></article>
    </div>
  </section>

  <section class="section">
    <div class="section-heading"><h2>Selected Publications</h2></div>
    <div class="pub-list">
      <article class="pub">
        <h3>Entropy-Based Unified Theory of Failure Threshold of Degrading Systems</h3>
        <p><strong>Lijesh K. P.</strong> and M. M. Khonsari</p>
        <p class="journal">Newton 1, no. 3 (2025): 100035</p>
        <a class="pub-link" href="https://doi.org/10.1016/j.newton.2025.100035" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a>
      </article>
      <article class="pub">
        <h3>A Thermodynamic Framework to Rapidly Determine Remaining Discharge Time in Li-Ion Batteries</h3>
        <p><strong>Lijesh K. P.</strong> and M. M. Khonsari</p>
        <p class="journal">Journal of Power Sources 655 (2025): 237922</p>
        <a class="pub-link" href="https://doi.org/10.1016/j.jpowsour.2025.237922" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a>
      </article>
      <article class="pub">
        <h3>A Thermodynamic Approach for the Rapid Estimation of the Remaining Time to Discharge in Li-Ion Batteries</h3>
        <p><strong>Lijesh K. P.</strong> and M. M. Khonsari</p>
        <p class="journal">Sustainable Energy Technologies and Assessments 82 (2025): 104490</p>
        <a class="pub-link" href="https://doi.org/10.1016/j.seta.2025.104490" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a>
      </article>
      <article class="pub">
        <h3>Experimentally Verified Thermodynamic Framework for Corrosion</h3>
        <p><strong>Lijesh K. P.</strong>, A. Mahmoudi, and M. M. Khonsari</p>
        <p class="journal">Corrosion Science 233 (2024): 112063</p>
        <a class="pub-link" href="https://doi.org/10.1016/j.corsci.2024.112063" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a>
      </article>
      <article class="pub">
        <h3>A Thermodynamic Approach for Characterizing the Degradation of Li-Ion Batteries</h3>
        <p><strong>Lijesh K. P.</strong> and M. M. Khonsari</p>
        <p class="journal">Journal of Energy Storage 82 (2024): 110565</p>
        <a class="pub-link" href="https://doi.org/10.1016/j.est.2024.110565" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a>
      </article>
      <article class="pub">
        <h3>Application of Thermodynamics to Industrial Grease Production</h3>
        <p><strong>Lijesh K. P.</strong>, R. A. Miller, A. Sanford, J. Carroll, and M. M. Khonsari</p>
        <p class="journal">Chemical Engineering Journal 489 (2024): 151306</p>
        <a class="pub-link" href="https://doi.org/10.1016/j.cej.2024.151306" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a>
      </article>
    </div>
  </section>

  <section class="section">
    <div class="section-heading"><h2>Related Patents</h2></div>
    <div class="patent-grid">
      <article class="patent"><h3>Damage Assessment</h3><p>Thermodynamics-based characterization of accumulated degradation and failure in engineering materials and systems.</p><a href="{{ '/patents/damage-assessment/' | relative_url }}">View Patent Details →</a></article>
      <article class="patent"><h3>Entropy-Based Fluid Monitoring</h3><p>Real-time process and condition monitoring through entropy-generation analysis during grease and food production.</p><a href="{{ '/patents/fluid-monitoring-grease/' | relative_url }}">View Patent Details →</a></article>
      <article class="patent"><h3>Battery Remaining Discharge</h3><p>Rapid thermodynamic estimation of the remaining discharge time of lithium-ion batteries.</p><a href="{{ '/patents/battery-remaining-discharge/' | relative_url }}">View Patent Details →</a></article>
    </div>
  </section>

  <div class="next-area">
    <div><h2>Next Research Area: Tribology and Wear</h2><p>Explore the application of thermodynamic degradation principles to friction, lubrication, wear mechanisms, and tribological failure.</p></div>
    <a href="{{ '/research/tribology-wear/' | relative_url }}">Explore Next Area →</a>
  </div>
</div>

<div class="modal" id="overview-modal" role="dialog" aria-modal="true" aria-label="Research overview image">
  <div class="modal-sheet"><button class="modal-close" type="button" aria-label="Close image viewer">×</button><img src="{{ '/assets/img/research/research_topic_entropy.png' | relative_url }}" alt="Large research overview"></div>
</div>
<div class="modal" id="deg-modal" role="dialog" aria-modal="true" aria-label="DEG framework image">
  <div class="modal-sheet"><button class="modal-close" type="button" aria-label="Close image viewer">×</button><img src="{{ '/assets/img/research/deg_framework.png' | relative_url }}" alt="Large DEG framework"></div>
</div>
<div class="modal" id="validation-modal" role="dialog" aria-modal="true" aria-label="FET validation image">
  <div class="modal-sheet"><button class="modal-close" type="button" aria-label="Close image viewer">×</button><img src="{{ '/assets/img/research/fet_validation_systems.png' | relative_url }}" alt="Large FET validation systems figure"></div>
</div>

<script>
document.addEventListener("DOMContentLoaded",function(){
  const opens=document.querySelectorAll("[data-modal-target]");
  const modals=document.querySelectorAll(".modal");
  function closeModal(modal){modal.classList.remove("open");document.body.style.overflow=""}
  opens.forEach(function(button){
    button.addEventListener("click",function(){
      const modal=document.getElementById(button.getAttribute("data-modal-target"));
      if(modal){modal.classList.add("open");document.body.style.overflow="hidden";const close=modal.querySelector(".modal-close");if(close){close.focus()}}
    });
  });
  modals.forEach(function(modal){
    const close=modal.querySelector(".modal-close");
    if(close){close.addEventListener("click",function(){closeModal(modal)})}
    modal.addEventListener("click",function(event){if(event.target===modal){closeModal(modal)}});
  });
  document.addEventListener("keydown",function(event){
    if(event.key==="Escape"){modals.forEach(function(modal){if(modal.classList.contains("open")){closeModal(modal)}})}
  });
});
</script>

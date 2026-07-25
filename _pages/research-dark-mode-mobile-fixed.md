---
layout: page
title: "Research"
permalink: /research/
description: "Research areas spanning thermodynamics-based degradation, tribology, corrosion, batteries, intelligent manufacturing, and advanced materials."
nav: true
nav_order: 2
---

<style>
:root{
  --p:#461d7c;
  --pd:#32105f;
  --ps:#f6f2fb;
  --g:#fdd023;
  --t:#171722;
  --m:#4a4a56;
  --b:#ddd9e6;
  --w:#ffffff;
}
.post,.post-content,.container{
  width:95%!important;
  max-width:1480px!important;
}
.post-header>h1,
.post-header>.post-description{
  display:none!important;
}
.research-landing{
  width:100%;
  margin:32px auto 72px;
  color:var(--t);
}
.research-hero{
  padding:38px;
  border-radius:14px;
  background:linear-gradient(135deg,var(--p),var(--pd));
  box-shadow:0 12px 32px rgba(50,16,95,.18);
}
.research-hero .kicker{
  margin:0 0 8px;
  color:var(--g);
  font-size:13px;
  font-weight:900;
  letter-spacing:.12em;
  text-transform:uppercase;
}
.research-hero h1{
  margin:0;
  color:#fff;
  font-size:clamp(36px,5vw,60px);
  font-weight:850;
  letter-spacing:-.04em;
  line-height:1.05;
}
.research-hero p{
  max-width:980px;
  margin:16px 0 0;
  color:rgba(255,255,255,.91);
  font-size:clamp(15px,1.55vw,20px);
  line-height:1.65;
}
.research-intro{
  max-width:1120px;
  margin:24px auto 0;
  color:var(--m);
  font-size:15px;
  line-height:1.75;
  text-align:center;
}
.topic{
  display:grid;
  grid-template-columns:minmax(0,1.08fr) minmax(360px,.92fr);
  gap:28px;
  align-items:center;
  margin-top:30px;
  padding:27px;
  border:1px solid var(--b);
  border-radius:13px;
  background:var(--w);
  box-shadow:0 7px 24px rgba(30,23,52,.065);
}
.topic.reverse .topic-image{
  order:-1;
}
.topic-number{
  display:inline-flex;
  align-items:center;
  justify-content:center;
  min-width:42px;
  height:29px;
  margin-bottom:10px;
  padding:0 11px;
  border-radius:999px;
  background:var(--ps);
  color:var(--p);
  font-size:11px;
  font-weight:900;
  letter-spacing:.08em;
}
.topic h2{
  margin:0 0 12px;
  color:var(--p);
  font-size:clamp(25px,3vw,36px);
  font-weight:850;
  letter-spacing:-.025em;
  line-height:1.2;
}
.topic p{
  margin:0;
  color:var(--m);
  font-size:14px;
  line-height:1.72;
}
.tags{
  display:flex;
  flex-wrap:wrap;
  gap:8px;
  margin-top:16px;
}
.tag{
  padding:7px 10px;
  border:1px solid rgba(70,29,124,.23);
  border-radius:999px;
  background:var(--ps);
  color:var(--p);
  font-size:10.5px;
  font-weight:800;
}
.topic-action{
  display:inline-flex;
  margin-top:18px;
  padding:11px 15px;
  border-radius:8px;
  background:var(--p);
  color:#fff!important;
  font-size:12px;
  font-weight:850;
  text-decoration:none!important;
}
.topic-action:hover{
  background:var(--pd);
}
.topic-action.disabled{
  background:#eceaf0;
  color:#77727f!important;
  pointer-events:none;
}
.topic-image{
  padding:11px;
  border:1px solid var(--b);
  border-radius:10px;
  background:#f7f7fa;
}
.topic-image img{
  display:block;
  width:100%;
  height:auto;
  margin:0;
  border-radius:7px;
}
.placeholder{
  display:flex;
  min-height:260px;
  align-items:center;
  justify-content:center;
  padding:26px;
  border-radius:7px;
  background:
    radial-gradient(circle at top right,rgba(70,29,124,.14),transparent 35%),
    linear-gradient(135deg,#faf8fd,#f1ecf8);
  color:var(--p);
  text-align:center;
}
.placeholder strong{
  display:block;
  font-size:22px;
  line-height:1.35;
}
.placeholder span{
  display:block;
  margin-top:8px;
  color:var(--m);
  font-size:12px;
}
@media(max-width:980px){
  .topic{
    grid-template-columns:1fr;
  }
  .topic.reverse .topic-image{
    order:initial;
  }
}
@media(max-width:680px){
  .research-hero{
    padding:28px 23px;
  }
  .topic{
    padding:21px;
  }
}


/* =========================================================
   DARK-MODE AND MOBILE CONTRAST FIX
   ========================================================= */

html[data-theme="dark"]{
  --p:#b894e8;
  --pd:#d2b8f1;
  --ps:#30263b;
  --g:#fdd023;
  --t:#f3f2f7;
  --m:#c8c5d0;
  --b:#4a4652;
  --w:#202024;
}

body.dark,
body.dark-mode{
  --p:#b894e8;
  --pd:#d2b8f1;
  --ps:#30263b;
  --g:#fdd023;
  --t:#f3f2f7;
  --m:#c8c5d0;
  --b:#4a4652;
  --w:#202024;
}

html[data-theme="dark"] .topic,
body.dark .topic,
body.dark-mode .topic{
  background:var(--w);
  border-color:var(--b);
}

html[data-theme="dark"] .topic h2,
html[data-theme="dark"] .topic-number,
html[data-theme="dark"] .tag,
html[data-theme="dark"] .placeholder,
body.dark .topic h2,
body.dark .topic-number,
body.dark .tag,
body.dark .placeholder,
body.dark-mode .topic h2,
body.dark-mode .topic-number,
body.dark-mode .tag,
body.dark-mode .placeholder{
  color:var(--p);
}

html[data-theme="dark"] .topic p,
html[data-theme="dark"] .research-intro,
html[data-theme="dark"] .placeholder span,
body.dark .topic p,
body.dark .research-intro,
body.dark .placeholder span,
body.dark-mode .topic p,
body.dark-mode .research-intro,
body.dark-mode .placeholder span{
  color:var(--m);
}

html[data-theme="dark"] .topic-image,
body.dark .topic-image,
body.dark-mode .topic-image{
  background:#29282e;
  border-color:var(--b);
}

html[data-theme="dark"] .placeholder,
body.dark .placeholder,
body.dark-mode .placeholder{
  background:
    radial-gradient(circle at top right,rgba(184,148,232,.16),transparent 35%),
    linear-gradient(135deg,#26232c,#30283b);
}

html[data-theme="dark"] .tag,
html[data-theme="dark"] .topic-number,
body.dark .tag,
body.dark .topic-number,
body.dark-mode .tag,
body.dark-mode .topic-number{
  background:var(--ps);
  border-color:rgba(184,148,232,.3);
}

html[data-theme="dark"] .topic-action,
body.dark .topic-action,
body.dark-mode .topic-action{
  background:#68409a;
  color:#ffffff!important;
}

html[data-theme="dark"] .topic-action.disabled,
body.dark .topic-action.disabled,
body.dark-mode .topic-action.disabled{
  background:#34323a;
  color:#b9b5c1!important;
}

@media(max-width:680px){
  .research-intro,
  .topic p{
    font-size:14px;
    line-height:1.68;
  }

  .topic h2{
    font-size:24px;
  }

  .topic{
    padding:19px;
  }
}

</style>

<div class="research-landing">

  <header class="research-hero">
    <p class="kicker">Research Portfolio</p>
    <h1>Research</h1>
    <p>
      Developing thermodynamics-based theories, experimental methods, sensing
      technologies, and predictive tools for understanding degradation and
      improving the reliability of materials, machines, batteries, and
      manufacturing processes.
    </p>
  </header>

  <p class="research-intro">
    My research is organized around a common objective: transforming irreversible
    energy dissipation into measurable information about damage, degradation
    severity, failure, and remaining life. The six areas below represent the
    principal scientific and application domains of this work.
  </p>

  <section class="topic">

    <div class="topic-copy">
      <span class="topic-number">AREA 01</span>

      <h2>Thermodynamics-Based Degradation and Failure</h2>

      <p>
        Develops a unified thermodynamic framework for quantifying irreversible
        degradation, relating entropy generation to measurable damage, identifying
        failure thresholds, and estimating remaining useful life under constant
        and variable operating conditions. The framework spans mechanical,
        electrochemical, electrical, energy-storage, and manufacturing systems.
      </p>

      <div class="tags">
        <span class="tag">DEG Framework</span>
        <span class="tag">Degradation Coefficient B</span>
        <span class="tag">Failure Entropy Threshold</span>
        <span class="tag">Remaining Useful Life</span>
      </div>

      <a
        class="topic-action"
        href="{{ '/research/thermodynamic-degradation/' | relative_url }}"
      >
        Explore This Research →
      </a>
    </div>

    <div class="topic-image">
      <img
        src="{{ '/assets/img/research/research_topic_entropy.png' | relative_url }}"
        alt="Thermodynamics-based degradation and failure research"
      >
    </div>

  </section>

  <section class="topic reverse">

    <div class="topic-copy">
      <span class="topic-number">AREA 02</span>

      <h2>Tribology</h2>

      <p>
        Investigates friction, lubrication, abrasive and adhesive wear, fretting,
        oscillatory contacts, wear transitions, and the thermodynamic
        characterization of tribological degradation under realistic operating
        conditions.
      </p>

      <div class="tags">
        <span class="tag">Friction</span>
        <span class="tag">Wear</span>
        <span class="tag">Lubrication</span>
        <span class="tag">Fretting</span>
      </div>

      <span class="topic-action disabled">Detailed Page Coming Soon</span>
    </div>

    <div class="topic-image">
      <div class="placeholder">
        <div>
          <strong>Tribology</strong>
          <span>Representative research image will be added here.</span>
        </div>
      </div>
    </div>

  </section>

  <section class="topic">

    <div class="topic-copy">
      <span class="topic-number">AREA 03</span>

      <h2>Corrosion and Hydrogen Embrittlement</h2>

      <p>
        Examines electrochemical degradation, flow-assisted corrosion,
        tribocorrosion, hydrogen charging, hydrogen-assisted cracking, and
        entropy-based comparison of material susceptibility under coupled
        environmental and mechanical conditions.
      </p>

      <div class="tags">
        <span class="tag">Corrosion</span>
        <span class="tag">Hydrogen Embrittlement</span>
        <span class="tag">Electrochemistry</span>
        <span class="tag">Material Damage</span>
      </div>

      <span class="topic-action disabled">Detailed Page Coming Soon</span>
    </div>

    <div class="topic-image">
      <div class="placeholder">
        <div>
          <strong>Corrosion and Hydrogen Embrittlement</strong>
          <span>Representative research image will be added here.</span>
        </div>
      </div>
    </div>

  </section>

  <section class="topic reverse">

    <div class="topic-copy">
      <span class="topic-number">AREA 04</span>

      <h2>Intelligent Manufacturing and Process Monitoring</h2>

      <p>
        Develops non-invasive sensing and thermodynamic process analytics for
        real-time monitoring of grease, food, and industrial manufacturing,
        supporting consistency assessment, process control, quality prediction,
        and waste reduction.
      </p>

      <div class="tags">
        <span class="tag">Process Monitoring</span>
        <span class="tag">Sensors</span>
        <span class="tag">Grease Production</span>
        <span class="tag">Food Manufacturing</span>
      </div>

      <span class="topic-action disabled">Detailed Page Coming Soon</span>
    </div>

    <div class="topic-image">
      <div class="placeholder">
        <div>
          <strong>Intelligent Manufacturing</strong>
          <span>Representative research image will be added here.</span>
        </div>
      </div>
    </div>

  </section>

  <section class="topic">

    <div class="topic-copy">
      <span class="topic-number">AREA 05</span>

      <h2>Battery Diagnostics and Remaining Discharge Prediction</h2>

      <p>
        Establishes rapid thermodynamic methods for characterizing lithium-ion
        battery degradation, estimating remaining discharge time, comparing
        performance across battery formats, and enabling real-time battery
        diagnostics.
      </p>

      <div class="tags">
        <span class="tag">Li-Ion Batteries</span>
        <span class="tag">Remaining Discharge Time</span>
        <span class="tag">Battery Degradation</span>
        <span class="tag">Diagnostics</span>
      </div>

      <span class="topic-action disabled">Detailed Page Coming Soon</span>
    </div>

    <div class="topic-image">
      <div class="placeholder">
        <div>
          <strong>Battery Diagnostics</strong>
          <span>Representative research image will be added here.</span>
        </div>
      </div>
    </div>

  </section>

  <section class="topic reverse">

    <div class="topic-copy">
      <span class="topic-number">AREA 06</span>

      <h2>Advanced Materials and Additive Manufacturing</h2>

      <p>
        Studies degradation in metals, polymers, composites, coatings, smart
        structures, and additively manufactured materials using experimental,
        computational, and multiscale approaches.
      </p>

      <div class="tags">
        <span class="tag">Additive Manufacturing</span>
        <span class="tag">Polymers and Composites</span>
        <span class="tag">Molecular Dynamics</span>
        <span class="tag">Smart Materials</span>
      </div>

      <span class="topic-action disabled">Detailed Page Coming Soon</span>
    </div>

    <div class="topic-image">
      <div class="placeholder">
        <div>
          <strong>Advanced Materials</strong>
          <span>Representative research image will be added here.</span>
        </div>
      </div>
    </div>

  </section>

</div>

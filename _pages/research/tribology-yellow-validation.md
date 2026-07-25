---
layout: page
title: "Tribology"
permalink: /research/tribology/
description: "Tribology research spanning dry wear, lubricated contacts, multiple wear mechanisms, variable loading, wear maps, and thermodynamics-based degradation."
nav: false
---

<style>
:root{
  --p:#461d7c;--pd:#32105f;--ps:#f6f2fb;--g:#fdd023;
  --t:#242433;--m:#626273;--b:#ddd9e6;--w:#fff;--panel:#fafafd
}
.post,.post-content,.container{width:95%!important;max-width:1480px!important}
.post-header>h1,.post-header>.post-description{display:none!important}
.trib-page{width:100%;margin:32px auto 72px;color:var(--t)}
.hero{overflow:hidden;border-radius:15px;background:linear-gradient(135deg,var(--p),var(--pd));box-shadow:0 12px 34px rgba(38,21,67,.17)}
.hero-grid{display:grid;grid-template-columns:minmax(0,1.2fr) minmax(350px,.8fr)}
.hero-copy{padding:40px 42px 38px}.kicker{margin:0 0 9px;color:var(--g);font-size:12px;font-weight:900;letter-spacing:.13em;text-transform:uppercase}
.hero h1{margin:0;color:#fff;font-size:clamp(42px,6vw,70px);font-weight:850;letter-spacing:-.045em;line-height:1}
.hero-desc{max-width:820px;margin:18px 0 0;color:rgba(255,255,255,.92);font-size:clamp(15px,1.5vw,19px);line-height:1.65}
.tags{display:flex;flex-wrap:wrap;gap:9px;margin-top:25px}.tag{padding:8px 11px;border:1px solid rgba(255,255,255,.26);border-radius:999px;background:rgba(255,255,255,.1);color:#fff;font-size:11px;font-weight:800}
.hero-image{min-height:360px;background:#f3f1f7}.hero-image img{display:block;width:100%;height:100%;min-height:360px;margin:0;object-fit:cover;object-position:center;cursor:zoom-in}
.opening{display:grid;grid-template-columns:minmax(0,1.45fr) minmax(340px,.55fr);gap:28px;align-items:start;margin-top:30px}
.card,.validation,.theme,.pub-item,.highlight{border:1px solid var(--b);border-radius:12px;background:var(--w);box-shadow:0 6px 22px rgba(32,22,52,.06)}
.card{padding:28px 30px}.section-kicker{margin:0 0 7px;color:var(--p);font-size:11px;font-weight:900;letter-spacing:.1em;text-transform:uppercase}
.section-title{margin:0 0 14px;color:var(--p);font-size:clamp(25px,3vw,36px);font-weight:850;letter-spacing:-.025em;line-height:1.2}
.card p,.theme p{margin:0;color:var(--t);font-size:15px;line-height:1.78}
.validation{padding:25px;border:1px solid #E2C94C;border-top:6px solid var(--g);background:linear-gradient(145deg,#FFF7CC,#FFE98A);box-shadow:0 10px 28px rgba(180,150,20,.20)}
.badge{display:inline-flex;margin-bottom:13px;padding:7px 10px;border:1px solid rgba(255,255,255,.28);border-radius:999px;background:#461d7c;color:#fff;font-size:10px;font-weight:900;letter-spacing:.08em;text-transform:uppercase}
.validation h2{margin:0 0 11px;color:#2a1a55;font-size:23px;font-weight:850}.validation>p{margin:0 0 14px;color:#222;font-size:13px;line-height:1.65}
.validation ul{display:flex;flex-direction:column;gap:9px;margin:0;padding:0;list-style:none}.validation li{display:grid;grid-template-columns:22px 1fr;gap:9px;color:#222;font-size:13px;line-height:1.48}
.check{display:inline-flex;align-items:center;justify-content:center;width:20px;height:20px;border-radius:50%;background:#461d7c;color:#fff;font-weight:900}
.note{margin-top:15px!important;padding-top:13px;border-top:1px solid #D9C35B;color:#444!important;font-size:11px!important;font-style:normal}
.section{margin-top:38px;padding-top:34px;border-top:1px solid var(--b)}.section-head{max-width:960px;margin-bottom:22px}.section-head p{margin:0;color:var(--m);font-size:14px;line-height:1.7}
.contrib{display:grid;grid-template-columns:repeat(5,minmax(0,1fr));gap:14px}.contrib article{min-height:180px;padding:20px 18px;border:1px solid var(--b);border-radius:10px;background:var(--w)}
.num{display:inline-flex;align-items:center;justify-content:center;width:34px;height:34px;margin-bottom:15px;border-radius:50%;background:var(--ps);color:var(--p);font-size:12px;font-weight:900}
.contrib h3{margin:0 0 9px;color:var(--p);font-size:17px;font-weight:820}.contrib p{margin:0;color:var(--m);font-size:12px;line-height:1.62}
.theme{display:grid;grid-template-columns:minmax(0,1fr) minmax(360px,.9fr);gap:28px;align-items:center;margin-top:24px;padding:26px}.theme.reverse .theme-image{order:-1}
.theme h3{margin:0 0 11px;color:var(--p);font-size:clamp(23px,2.6vw,31px);font-weight:850}.theme p{font-size:14px;line-height:1.72}.chips{display:flex;flex-wrap:wrap;gap:8px;margin-top:17px}.chip{padding:7px 10px;border:1px solid rgba(70,29,124,.2);border-radius:999px;background:var(--ps);color:var(--p);font-size:10.5px;font-weight:800}
.theme-image{overflow:hidden;padding:9px;border:1px solid var(--b);border-radius:10px;background:#f6f5f9}.theme-image img{display:block;width:100%;height:auto;margin:0;border-radius:7px;cursor:zoom-in}
.placeholder{display:flex;min-height:260px;align-items:center;justify-content:center;padding:30px;border-radius:7px;background:linear-gradient(135deg,#faf8fd,#f0ebf7);color:var(--p);text-align:center}.placeholder strong{display:block;font-size:21px}.placeholder span{display:block;margin-top:8px;color:var(--m);font-size:12px}
.highlights{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:15px}.highlight{padding:21px;border-left:5px solid var(--p)}.highlight strong{display:block;margin-bottom:7px;color:var(--p);font-size:15px}.highlight span{color:var(--m);font-size:12px;line-height:1.6}
.tabs{display:flex;flex-wrap:wrap;gap:11px;margin-bottom:22px}.tab{min-width:150px;padding:12px 18px;border:1px solid var(--b);border-radius:999px;background:var(--w);color:var(--p);font-size:14px;font-weight:850;line-height:1.25;cursor:pointer}.tab.active,.tab:hover{background:var(--p);border-color:var(--p);color:#fff}
.pub-group{display:none}.pub-group.active{display:block}.pub-group h3{margin:0 0 14px;color:var(--p);font-size:24px}.pub-list{display:flex;flex-direction:column;gap:10px}.pub-item{display:grid;grid-template-columns:38px 1fr;gap:13px;padding:16px 18px}.pub-index{color:var(--p);font-size:12px;font-weight:900}.citation{color:var(--t);font-size:13px;line-height:1.65}.citation strong,.citation em{color:var(--p)}.doi{display:inline-flex;margin-top:9px;padding:7px 10px;border-radius:6px;background:var(--p);color:#fff!important;font-size:10.5px;font-weight:800;text-decoration:none!important}.doi:hover{background:var(--pd)}
.modal{position:fixed;inset:0;z-index:9999;display:none;align-items:center;justify-content:center;padding:24px;background:rgba(10,8,14,.9)}.modal.open{display:flex}.modal img{max-width:94vw;max-height:90vh;margin:0;border-radius:8px;background:#fff}.close{position:fixed;top:18px;right:22px;width:42px;height:42px;border:0;border-radius:50%;background:#fff;color:var(--pd);font-size:24px;cursor:pointer}
html[data-theme="dark"],body.dark,body.dark-mode{--p:#b894e8;--pd:#d2b8f1;--ps:#30263b;--t:#f3f2f7;--m:#c8c5d0;--b:#4a4652;--w:#202024;--panel:#29282e}
html[data-theme="dark"] .theme-image,body.dark .theme-image,body.dark-mode .theme-image{background:#29282e}.publication-tab{background:var(--w)}
@media(max-width:1120px){.hero-grid,.opening,.theme{grid-template-columns:1fr}.theme.reverse .theme-image{order:initial}.contrib{grid-template-columns:repeat(2,1fr)}}
@media(max-width:760px){.post,.post-content,.container{width:94%!important}.hero-copy{padding:30px 24px}.card,.validation,.theme{padding:21px}.contrib,.highlights{grid-template-columns:1fr}.pub-item{grid-template-columns:30px 1fr;padding:14px}.citation{font-size:12.5px}}
</style>

<div class="trib-page">
  <header class="hero">
    <div class="hero-grid">
      <div class="hero-copy">
        <p class="kicker">Research Area</p>
        <h1>Tribology</h1>
        <p class="hero-desc">Investigates the tribological performance, degradation, and failure of engineering components operating under dry and lubricated conditions, with particular emphasis on realistic operating conditions.</p>
        <div class="tags">
          <span class="tag">Dry Wear</span><span class="tag">Lubricated Contacts</span><span class="tag">Multiple Wear Mechanisms</span><span class="tag">Variable Load</span><span class="tag">Wear Maps</span>
        </div>
      </div>
      <div class="hero-image"><img class="zoomable" src="{{ '/assets/img/research/research_topic_tribology.png' | relative_url }}" alt="Tribology research overview"></div>
    </div>
  </header>

  <div class="opening">
    <section class="card">
      <p class="section-kicker">Research Overview</p>
      <h2 class="section-title">Tribological degradation under realistic operating conditions</h2>
      <p>Tribological systems rarely operate under constant loading or ideal laboratory conditions. Changes in load, sliding speed, lubrication regime, surface condition, contact geometry, and motion alter friction, material removal, surface transformation, and component life. This research combines experimental tribology, thermodynamic analysis, degradation modeling, and surface characterization to establish physically meaningful relationships among energy dissipation, wear progression, damage mechanisms, and useful life. The work spans adhesive wear, abrasive wear, fretting, oscillatory contacts, boundary and mixed lubrication, multiple wear mechanisms, loading-sequence effects, and thermodynamics-based wear maps.</p>
    </section>

    <aside class="validation">
      <span class="badge">Independent Study</span>
      <h2>Independent Comparative Validation</h2>
      <p>
        An independent comparative study evaluated five wear models, including
        Archard’s model, and reported that the DEG-theorem-based wear model
        [Lijesh et al. [a]] provided the strongest overall performance by:
      </p>
      <ul>
        <li><span class="check">✓</span><span>Reducing parameter uncertainty</span></li>
        <li><span class="check">✓</span><span>Minimizing parameterization requirements</span></li>
        <li><span class="check">✓</span><span>Decreasing dependence on specific loading conditions</span></li>
        <li><span class="check">✓</span><span>Improving computational efficiency</span></li>
      </ul>
      <p class="note">
        [a] Lijesh, K. P., M. M. Khonsari, and Satish V. Kailas. (2018)
        <em>Wear</em> 408–409, 138–150.
      </p>
    </aside>
  </div>

  <section class="section">
    <div class="section-head"><p class="section-kicker">Research Philosophy</p><h2 class="section-title">From frictional energy dissipation to wear and failure</h2><p>The central objective is to move beyond purely empirical wear correlations by describing tribological degradation through irreversible energy dissipation. Thermodynamic quantities are used to quantify damage accumulation, compare operating conditions, identify transitions among wear mechanisms, and predict useful life under constant and variable loading histories.</p></div>
    <div class="contrib">
      <article><span class="num">01</span><h3>Thermodynamic Framework</h3><p>Links frictional dissipation and entropy generation to wear progression, degradation rate, and failure.</p></article>
      <article><span class="num">02</span><h3>Dry Wear</h3><p>Characterizes adhesive wear, abrasive wear, fretting, transient wear, and wear-resistant materials.</p></article>
      <article><span class="num">03</span><h3>Lubricated Contacts</h3><p>Examines boundary and mixed lubrication, oscillatory contacts, journal bearings, and textured systems.</p></article>
      <article><span class="num">04</span><h3>Variable Conditions</h3><p>Evaluates degradation under changing load, speed, motion, and loading sequence.</p></article>
      <article><span class="num">05</span><h3>Wear Maps</h3><p>Identifies dominant and interacting wear mechanisms across realistic operating domains.</p></article>
    </div>
  </section>

  <section class="section">
    <div class="theme"><div><p class="section-kicker">Research Theme 01</p><h3>Thermodynamics-Based Tribology</h3><p>This work applies the degradation entropy generation framework to establish a unified treatment of tribological degradation. The degradation coefficient relates entropy generation to measurable wear, enabling comparison across operating conditions, materials, contact configurations, and degradation mechanisms. The framework also supports failure-threshold identification, remaining-life estimation, and thermodynamics-based wear maps.</p><div class="chips"><span class="chip">DEG Framework</span><span class="chip">Degradation Coefficient</span><span class="chip">Failure Threshold Entropy</span><span class="chip">Useful Life</span></div></div><div class="theme-image"><img class="zoomable" src="{{ '/assets/img/research/tribology_framework.png' | relative_url }}" alt="Tribology framework from operating conditions to degradation, performance, and useful life"></div></div>

    <div class="theme reverse"><div><p class="section-kicker">Research Theme 02</p><h3>Dry Wear</h3><p>Dry-contact studies investigate adhesive wear, abrasive wear, fretting, transient wear evolution, variable loading, loading-sequence effects, surface coatings, and wear-resistant materials. Experimental measurements are integrated with surface characterization and thermodynamic analysis to distinguish wear stages, quantify degradation, and identify transitions from transient to steady-state behavior.</p><div class="chips"><span class="chip">Adhesive Wear</span><span class="chip">Abrasive Wear</span><span class="chip">Fretting</span><span class="chip">Surface Engineering</span></div></div><div class="theme-image"><div class="placeholder"><div><strong>Dry-Contact Tribology</strong><span>Upload tribology_dry_wear.png to assets/img/research/.</span></div></div></div></div>

    <div class="theme"><div><p class="section-kicker">Research Theme 03</p><h3>Lubricated Contacts</h3><p>Lubricated-contact research examines tribological degradation in boundary and mixed lubrication regimes, oscillatory sliding, journal bearings, hybrid bearings, and surface-textured contacts. The approach captures how lubricant films, asperity interactions, friction, and oscillatory motion collectively influence degradation and service life.</p><div class="chips"><span class="chip">Boundary Lubrication</span><span class="chip">Mixed Lubrication</span><span class="chip">Oscillatory Motion</span><span class="chip">Journal Bearings</span></div></div><div class="theme-image"><div class="placeholder"><div><strong>Lubricated Tribology</strong><span>Upload tribology_lubricated.png to assets/img/research/.</span></div></div></div></div>

    <div class="theme reverse"><div><p class="section-kicker">Research Theme 04</p><h3>Variable Load and Sliding Conditions</h3><p>Engineering components commonly experience changing loads, speeds, and motion histories rather than a single constant condition. This research develops formulations that retain the effect of operating history and loading sequence, enabling wear progression, friction response, temperature evolution, and useful life to be evaluated under realistic service conditions.</p><div class="chips"><span class="chip">Variable Load</span><span class="chip">Variable Speed</span><span class="chip">Loading Sequence</span><span class="chip">Trend Analysis</span></div></div><div class="theme-image"><img class="zoomable" src="{{ '/assets/img/research/variable_load_generalized.png' | relative_url }}" alt="Generalized tribological response under variable load conditions"></div></div>

    <div class="theme"><div><p class="section-kicker">Research Theme 05</p><h3>Multiple Wear Mechanisms and Wear Maps</h3><p>Wear rarely develops through a single isolated mechanism. Depending on load, speed, material response, and surface condition, abrasion, delamination, severe plastic deformation, surface fatigue, and oxidative wear can coexist or transition from one regime to another. Thermodynamics-based wear maps provide a unified representation of these domains and their transitions.</p><div class="chips"><span class="chip">Multiple Wear</span><span class="chip">Mechanism Transition</span><span class="chip">Wear Regimes</span><span class="chip">Wear Maps</span></div></div><div class="theme-image"><img class="zoomable" src="{{ '/assets/img/research/wear_map.png' | relative_url }}" alt="Wear map showing multiple wear mechanisms and transition regions"></div></div>
  </section>

  <section class="section">
    <div class="section-head"><p class="section-kicker">Research Highlights</p><h2 class="section-title">Selected scientific contributions</h2></div>
    <div class="highlights">
      <div class="highlight"><strong>Unified thermodynamic wear model</strong><span>Establishes a physics-informed relationship among frictional dissipation, entropy generation, degradation rate, and accumulated wear.</span></div>
      <div class="highlight"><strong>Variable-loading formulation</strong><span>Retains operating-history and loading-sequence effects when predicting wear progression and useful life.</span></div>
      <div class="highlight"><strong>Multiple-mechanism characterization</strong><span>Uses thermodynamic descriptors to compare and map coexisting or transitioning wear mechanisms.</span></div>
      <div class="highlight"><strong>Dry and lubricated systems</strong><span>Extends the same degradation philosophy across dry contacts, boundary lubrication, mixed lubrication, and oscillatory motion.</span></div>
      <div class="highlight"><strong>Failure and useful-life assessment</strong><span>Connects accumulated entropy generation with failure thresholds and service-life estimation.</span></div>
      <div class="highlight"><strong>Independent comparative validation</strong><span>External comparison reported reduced uncertainty, fewer parameters, lower loading-condition dependence, and improved efficiency.</span></div>
    </div>
  </section>

  <section class="section" id="tribology-publications">
    <div class="section-head"><p class="section-kicker">Publications</p><h2 class="section-title">Selected Tribology Publications</h2><p>Publications are organized into conceptual contributions, dry-contact studies, and lubricated-contact studies.</p></div>
    <div class="tabs"><button class="tab active" type="button" data-target="conceptual">Conceptual</button><button class="tab" type="button" data-target="dry">Dry Wear</button><button class="tab" type="button" data-target="lubricated">Lubricated Contacts</button></div>

    <div class="pub-group active" id="group-conceptual"><h3>Conceptual</h3><div class="pub-list">
      <article class="pub-item"><div class="pub-index">01</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “Failure Threshold Entropy and Its Application in Tribology.” <em>Encyclopedia of Tribology and Lubrication</em>. Elsevier, 2026.<br><a class="doi" href="https://doi.org/10.1016/B978-0-443-30138-4.00022-4" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">02</div><div class="citation"><strong>Lijesh, K. P.</strong>, and Michael M. Khonsari. “Wear Maps Derived from Thermodynamic Principles.” <em>Wear</em> (2026): 206694.<br><a class="doi" href="https://doi.org/10.1016/j.wear.2026.206694" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">03</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “Entropy-Based Unified Theory of Failure Threshold of Degrading Systems.” <em>Newton</em> 1, no. 3 (2025): 100035.<br><a class="doi" href="https://doi.org/10.1016/j.newton.2025.100035" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">04</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “A Unified Treatment of Tribo-Components Degradation Using Thermodynamics Framework: A Review on Adhesive Wear.” <em>Entropy</em> 23, no. 10 (2021): 1329.<br><a class="doi" href="https://doi.org/10.3390/e23101329" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">05</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “Characterization of Multiple Wear Mechanisms through Entropy.” <em>Tribology International</em> 152 (2020): 106548.<br><a class="doi" href="https://doi.org/10.1016/j.triboint.2020.106548" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
    </div></div>

    <div class="pub-group" id="group-dry"><h3>Dry Wear</h3><div class="pub-list">
      <article class="pub-item"><div class="pub-index">01</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “Thermodynamic Characterization of Fretting-Induced Material Degradation Using Degradation Entropy Generation Framework.” <em>Wear</em> (2025): 206341.<br><a class="doi" href="https://doi.org/10.1016/j.wear.2025.206341" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">02</div><div class="citation">Adibi, Noushin, Ehsan Bagheri, <strong>Lijesh K. P.</strong>, Saeid Zavari, Hamed Ghadimi, Michael Khonsari, and Shengmin Guo. “High-Frequency Fatigue, Tribological Performance, and Corrosion Resistance of Al 2050 Prepared by Additive Friction Stir Deposition.” <em>The International Journal of Advanced Manufacturing Technology</em> (2026): 1–13.<br><a class="doi" href="https://doi.org/10.1007/s00170-026-18296-y" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">03</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “Characterization of Abrasive Wear Using Degradation Coefficient.” <em>Wear</em> 450–451 (2020): 203220.<br><a class="doi" href="https://doi.org/10.1016/j.wear.2020.203220" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">04</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “On the Onset of Steady State during Transient Adhesive Wear.” <em>Tribology International</em> 130 (2019): 378–386.<br><a class="doi" href="https://doi.org/10.1016/j.triboint.2018.10.004" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">05</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “On the Useful Life of Tribo-Pairs Experiencing Variable Loading and Sliding Speed.” <em>Wear</em> 416–417 (2018): 103–114.<br><a class="doi" href="https://doi.org/10.1016/j.wear.2018.10.005" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">06</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “On the Modeling of Adhesive Wear with Consideration of Loading Sequence.” <em>Tribology Letters</em> 66 (2018): 105.<br><a class="doi" href="https://doi.org/10.1007/s11249-018-1058-2" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">07</div><div class="citation"><strong>Lijesh, K. P.</strong>, M. M. Khonsari, and Satish V. Kailas. “On the Integrated Degradation Coefficient for Adhesive Wear: A Thermodynamic Approach.” <em>Wear</em> 408–409 (2018): 138–150.<br><a class="doi" href="https://doi.org/10.1016/j.wear.2018.05.004" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">08</div><div class="citation">Madhu, H. C., Vimal Edachery, <strong>K. P. Lijesh</strong>, Chandra Shekhar Perugu, and Satish V. Kailas. “Fabrication of Wear-Resistant Ti₃AlC₂/Al₃Ti Hybrid Aluminum Composites by Friction Stir Processing.” <em>Metallurgical and Materials Transactions A</em> 51, no. 8 (2020): 4086–4099.<br><a class="doi" href="https://doi.org/10.1007/s11661-020-05821-1" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">09</div><div class="citation">Anderson, N. J., Bin Zhang, A. C. Meng, Xiaoman Zhang, <strong>K. P. Lijesh</strong>, M. M. Khonsari, and W. J. Meng. “Cr-Containing Diamond-Like Carbon Coatings Deposited on 316 Stainless Steel Substrates: Characterization and Interfacial Fracture-Toughness Measurements.” <em>Surface and Coatings Technology</em> 462 (2023): 129462.<br><a class="doi" href="https://doi.org/10.1016/j.surfcoat.2023.129462" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">10</div><div class="citation">Lokhande, Rohan, Sitesh Kumar Mishra, Deepak Ronanki, Piyush Shakya, Vimal Edachery, and <strong>Lijesh K. P.</strong> “Review on Tribological and Vibration Aspects in Mechanical Bearings of Electric Vehicles: Effect of Bearing Current, Shaft Voltage, and Electric Discharge Material Spalling Current.” <em>Lubricants</em> 13, no. 8 (2025): 349.<br><a class="doi" href="https://doi.org/10.3390/lubricants13080349" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
    </div></div>

    <div class="pub-group" id="group-lubricated"><h3>Lubricated Contacts</h3><div class="pub-list">
      <article class="pub-item"><div class="pub-index">01</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “Application of Thermodynamic Principles in Determining the Degradation of Tribo-Components Subjected to Oscillating Motion in Boundary and Mixed Lubrication Regimes.” <em>Wear</em> 436–437 (2019): 203002.<br><a class="doi" href="https://doi.org/10.1016/j.wear.2019.203002" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">02</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “On the Degradation of Tribo-Components Undergoing Oscillating Sliding Contact.” <em>Tribology International</em> 135 (2019): 18–28.<br><a class="doi" href="https://doi.org/10.1016/j.triboint.2019.02.016" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">03</div><div class="citation">Chaichi, Ardalan, Alisha Prasad, <strong>Lijesh K. P.</strong>, Shahensha Shaik, Ali Hemmasian Ettefagh, Vinod Dasa, S. M. Guo, et al. “Improvement of Tribological and Biocompatibility Properties of Orthopedic Materials Using Piezoelectric Direct Discharge Plasma Surface Modification.” <em>ACS Biomaterials Science &amp; Engineering</em> 5 (2019): 2147–2159.<br><a class="doi" href="https://doi.org/10.1021/acsbiomaterials.9b00009" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">04</div><div class="citation"><strong>Lijesh, K. P.</strong>, and M. M. Khonsari. “On the Degradation of Tribo-Components in Boundary and Mixed Lubrication Regimes.” <em>Tribology Letters</em> 67, no. 1 (2019): 12.<br><a class="doi" href="https://doi.org/10.1007/s11249-018-1125-8" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">05</div><div class="citation">Anand, P., P. Ramkumar, <strong>K. P. Lijesh</strong>, and Vimal Edachery. “Tribological Performance of Laser-Based Surface-Textured Nonconformal Contacts.” <em>Advances in Tribology</em> 2024 (2024).<br><a class="doi" href="https://doi.org/10.1155/2024/1424767" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">06</div><div class="citation"><strong>Lijesh, K. P.</strong>, and Harish Hirani. “Design and Development of Permanent Magnet-Hydrodynamic Hybrid Journal Bearing.” <em>Journal of Tribology</em> 139, no. 4 (2017): 044501.<br><a class="doi" href="https://doi.org/10.1115/1.4035153" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">07</div><div class="citation"><strong>Lijesh, K. P.</strong>, S. M. Muzakkir, and Harish Hirani. “Control on Wear of Journal Bearing Operating in Mixed Lubrication Regime Using Grooving Arrangements.” <em>Industrial Lubrication and Tribology</em> 68, no. 4 (2016): 458–465.<br><a class="doi" href="https://doi.org/10.1108/ILT-11-2015-0162" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">08</div><div class="citation">Muzakkir, S. M., <strong>Lijesh K. P.</strong>, and Harish Hirani. “Effect of Cylindricity on the Tribological Performance of Heavily Loaded Slow-Speed Journal Bearing.” <em>Proceedings of the Institution of Mechanical Engineers, Part J: Journal of Engineering Tribology</em> 229, no. 2 (2015): 178–195.<br><a class="doi" href="https://doi.org/10.1177/1350650114548053" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
      <article class="pub-item"><div class="pub-index">09</div><div class="citation">Muzakkir, S. M., <strong>Lijesh K. P.</strong>, and Harish Hirani. “Tribological Failure Analysis of a Heavily Loaded Slow-Speed Hybrid Journal Bearing.” <em>Engineering Failure Analysis</em> 40 (2014): 97–113.<br><a class="doi" href="https://doi.org/10.1016/j.engfailanal.2014.02.016" target="_blank" rel="noopener noreferrer">View on Journal Website ↗</a></div></article>
    </div></div>
  </section>
</div>

<div class="modal" id="image-modal" aria-hidden="true"><button class="close" id="modal-close" type="button" aria-label="Close enlarged image">×</button><img id="modal-image" src="" alt=""></div>

<script>
document.addEventListener("DOMContentLoaded",function(){
  const tabs=[...document.querySelectorAll(".tab")],groups=[...document.querySelectorAll(".pub-group")];
  tabs.forEach(tab=>tab.addEventListener("click",()=>{tabs.forEach(x=>x.classList.remove("active"));groups.forEach(x=>x.classList.remove("active"));tab.classList.add("active");const g=document.getElementById("group-"+tab.dataset.target);if(g)g.classList.add("active")}));
  const modal=document.getElementById("image-modal"),img=document.getElementById("modal-image"),close=document.getElementById("modal-close");
  const shut=()=>{modal.classList.remove("open");modal.setAttribute("aria-hidden","true");img.src="";document.body.style.overflow=""};
  document.querySelectorAll(".zoomable").forEach(x=>x.addEventListener("click",()=>{img.src=x.src;img.alt=x.alt||"Enlarged research image";modal.classList.add("open");modal.setAttribute("aria-hidden","false");document.body.style.overflow="hidden"}));
  close.addEventListener("click",shut);modal.addEventListener("click",e=>{if(e.target===modal)shut()});document.addEventListener("keydown",e=>{if(e.key==="Escape")shut()});
});
</script>

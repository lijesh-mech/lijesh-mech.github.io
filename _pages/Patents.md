---
layout: page
title: Patents
permalink: /patents/
nav: true
nav_order: 5
description: "Granted and filed patents of Dr. Lijesh Koottaparambil"
---

<style>
:root{
  --p:#461d7c;
  --pd:#32105f;
  --t:#242433;
  --m:#666678;
  --b:#e1e1e8;
}

.post,
.post-content,
.container{
  width:95%!important;
  max-width:1250px!important;
}

.patents-wrap{
  margin:34px auto 70px;
  color:var(--t);
}

.patents-hero{
  padding:30px 34px;
  background:linear-gradient(135deg,var(--p),var(--pd));
  border-radius:12px;
  color:#fff;
}

.patents-hero h1{
  margin:0;
  color:#fff;
  font-size:clamp(32px,4vw,50px);
  font-weight:780;
}

.patents-hero p{
  margin:10px 0 0;
  color:rgba(255,255,255,.88);
  font-size:14px;
}

.patent-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
  gap:26px;
  margin-top:28px;
}

.patent-card{
  overflow:hidden;
  background:#fff;
  border:1px solid var(--b);
  border-radius:12px;
  box-shadow:0 6px 22px rgba(28,20,50,.07);
}

.patent-image-link{
  display:block;
  padding:16px;
  background:#f4f6fa;
  border-bottom:1px solid var(--b);
  text-decoration:none!important;
}

.patent-image-link img{
  display:block;
  width:100%;
  height:auto;
  margin:0;
  background:#fff;
  border:1px solid #cfd4df;
  border-radius:8px;
}

.patent-content{
  padding:22px;
}

.patent-topline{
  display:flex;
  justify-content:space-between;
  align-items:center;
  gap:12px;
  margin-bottom:12px;
}

.patent-number{
  color:var(--p);
  font-size:12px;
  font-weight:820;
  text-transform:uppercase;
}

.patent-status{
  padding:6px 10px;
  background:#edf7ee;
  border:1px solid #cde8d0;
  border-radius:999px;
  color:#2e7d32;
  font-size:11px;
  font-weight:820;
}

.patent-title{
  margin:0 0 12px;
  font-size:clamp(22px,2.4vw,30px);
}

.patent-meta{
  margin:0 0 18px;
  color:var(--m);
  font-size:13px;
  line-height:1.65;
}

.patent-button{
  display:inline-flex;
  align-items:center;
  justify-content:center;
  min-height:46px;
  padding:10px 15px;
  background:var(--p);
  border-radius:8px;
  color:#fff!important;
  font-size:13px;
  font-weight:760;
  text-decoration:none!important;
}

@media(max-width:680px){
  .post,
  .post-content,
  .container{
    width:94%!important;
  }

  .patents-hero{
    padding:24px 22px;
  }
}
</style>

<div class="patents-wrap">

  <header class="patents-hero">
    <h1>Patents</h1>
    <p>Granted and filed intellectual-property developments.</p>
  </header>

  <section class="patent-grid">

<article class="patent-card">

  <a
    class="patent-image-link"
    href="{{ '/patents/damage-assessment/' | relative_url }}"
    aria-label="Open Damage Assessment of Tribo-Systems"
  >
    <img
      src="{{ '/assets/img/patents/damage_assessment.png' | relative_url }}"
      alt="Damage Assessment of Tribo-Systems"
    >
  </a>

  <div class="patent-content">

    <div class="patent-topline">
      <span class="patent-number">US 11,488,420 B2</span>
      <span class="patent-status">Granted</span>
    </div>

    <h2 class="patent-title">Damage Assessment of Tribo-Systems</h2>

    <p class="patent-meta">
      Inventors: M. M. Khonsari and Lijesh K. P.<br>
      United States · 2022
    </p>

    <a
      class="patent-button"
      href="{{ '/patents/damage-assessment/' | relative_url }}"
    >
      View Patent Details →
    </a>

  </div>

</article>

  </section>

</div>

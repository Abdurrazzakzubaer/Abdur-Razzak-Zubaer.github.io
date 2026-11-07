---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---
<!-- Remove these imports if already loaded through _includes/head/custom.html. -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap-grid.min.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
<style>
/* Scoped to this page to avoid Jekyll/Academic Pages theme conflicts. */
.arz-projects{--navy:#102d50;--blue:#1c4a77;--accent:#2778c4;--muted:#61758b;--line:#e0e9f2;--soft:#f6f9fd;color:#273b50}
.arz-projects *, .arz-projects *::before,.arz-projects *::after{box-sizing:border-box}
.arz-projects .pj-hero{position:relative;overflow:hidden;isolation:isolate;background:linear-gradient(125deg,#102d50 0%,#1a4675 63%,#286f9f 100%);color:white;border-radius:18px;padding:44px 35px;margin-bottom:25px}
.arz-projects .pj-hero::after{content:"";position:absolute;right:-90px;top:-100px;width:260px;height:260px;border:1px solid #ffffff30;border-radius:50%;box-shadow:0 0 0 38px #ffffff0a,0 0 0 78px #ffffff07;z-index:-1}
.arz-projects .pj-kicker{display:flex;align-items:center;gap:8px;color:#bbdfff;letter-spacing:1.2px;text-transform:uppercase;font-size:.75rem;font-weight:750;margin-bottom:14px}
.arz-projects .pj-hero h1{color:#fff;margin:0 0 13px;padding:0;border:0;font-size:clamp(1.9rem,3.8vw,2.6rem);line-height:1.15;font-weight:800}
.arz-projects .pj-hero p{max-width:720px;color:#e0ebf7;font-size:.97rem;line-height:1.8;margin:0}
.arz-projects .pj-stats{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:12px;margin:0 0 30px}
.arz-projects .pj-stat{padding:17px 18px;background:var(--soft);border:1px solid var(--line);border-radius:12px}
.arz-projects .pj-stat strong{display:block;color:var(--navy);font-size:1.4rem;line-height:1.3}
.arz-projects .pj-stat span{color:var(--muted);font-size:.8rem}
.arz-projects .pj-controls{padding:20px;margin-bottom:15px;background:#f8fbff;border:1px solid var(--line);border-radius:14px}
.arz-projects .pj-label{display:block;font-size:.82rem;font-weight:700;color:var(--navy);margin:0 0 8px}
.arz-projects .pj-search-wrap{position:relative}
.arz-projects .pj-search-wrap .bi-search{position:absolute;left:15px;top:50%;transform:translateY(-50%);color:#627b96;pointer-events:none}
.arz-projects .pj-search{display:block;width:100%;min-height:45px;padding:11px 13px 11px 42px;background:#fff;border:1px solid #cad9e9;border-radius:9px;font:inherit;font-size:.92rem;color:var(--navy);outline:none;transition:border-color .2s,box-shadow .2s}
.arz-projects .pj-search:focus{border-color:#2778c4;box-shadow:0 0 0 3px #2778c429}
.arz-projects .pj-filterbar{display:flex;flex-wrap:wrap;gap:8px;margin-top:15px}
.arz-projects .pj-filter{font:inherit;padding:8px 13px;border:1px solid #ccdaea;background:white;border-radius:999px;color:#36556f;font-size:.81rem;font-weight:650;cursor:pointer;transition:background-color .2s,border-color .2s,transform .2s,color .2s}
.arz-projects .pj-filter:hover{border-color:#79a8d3;transform:translateY(-1px)}
.arz-projects .pj-filter[aria-pressed="true"]{background:var(--navy);color:white;border-color:var(--navy)}
.arz-projects .pj-results{display:flex;align-items:center;justify-content:space-between;gap:15px;margin:0 0 15px;color:var(--muted);font-size:.85rem}
.arz-projects .pj-reset{border:0;background:transparent;color:#185e9c;font:inherit;font-size:.84rem;font-weight:700;cursor:pointer;text-decoration:underline;text-underline-offset:3px}
.arz-projects .pj-grid{align-items:stretch}
.arz-projects .pj-card{display:flex;flex-direction:column;height:100%;background:#fff;border:1px solid var(--line);border-radius:14px;padding:23px;box-shadow:0 4px 15px #102d500a;transition:border-color .27s,box-shadow .27s,transform .27s}
.arz-projects .pj-card:hover,.arz-projects .pj-card:focus-within{transform:translateY(-4px);border-color:#bad3e9;box-shadow:0 15px 30px #102d5017}
.arz-projects .pj-card[hidden]{display:none!important}
.arz-projects .pj-cardtop{display:flex;justify-content:space-between;align-items:center;gap:10px;margin-bottom:15px}
.arz-projects .pj-index{display:inline-flex;align-items:center;justify-content:center;width:38px;height:38px;background:#eaf3ff;border-radius:10px;color:#1e5c99;font-size:.83rem;font-weight:800}
.arz-projects .pj-type{display:inline-flex;gap:6px;align-items:center;border-radius:999px;padding:5px 10px;background:#eff6fc;color:#2d668b;font-size:.73rem;font-weight:700}
.arz-projects .pj-type[data-type="Energy"]{background:#fff5e8;color:#966216}
.arz-projects .pj-type[data-type="Environment"]{background:#edf7f1;color:#277750}
.arz-projects .pj-type[data-type="Research"]{background:#f3effb;color:#7452a5}
.arz-projects .pj-card h3{margin:0 0 17px;padding:0;color:var(--navy);font-size:clamp(1rem,1.3vw,1.15rem);line-height:1.48;font-weight:750}
.arz-projects .pj-meta{display:grid;gap:10px;margin:0 0 19px}
.arz-projects .pj-meta>div{display:grid;grid-template-columns:93px minmax(0,1fr);gap:9px}
.arz-projects .pj-meta dt{color:#718298;font-size:.76rem;font-weight:700}
.arz-projects .pj-meta dd{margin:0;color:#43596d;font-size:.82rem;line-height:1.55;overflow-wrap:anywhere}
.arz-projects .pj-details{margin-top:auto;border-top:1px solid var(--line);padding-top:14px}
.arz-projects .pj-details summary{display:flex;justify-content:space-between;align-items:center;gap:12px;color:#1d5c9c;font-size:.85rem;font-weight:750;cursor:pointer;list-style:none;user-select:none}
.arz-projects .pj-details summary::-webkit-details-marker{display:none}
.arz-projects .pj-details summary .bi{transition:transform .2s}
.arz-projects .pj-details[open] summary .bi{transform:rotate(180deg)}
.arz-projects .pj-details ul{margin:16px 0 0;padding-left:19px;color:#4a6073;font-size:.84rem;line-height:1.7}
.arz-projects .pj-details li{margin-bottom:7px}
.arz-projects .pj-empty{padding:30px;background:var(--soft);border:1px dashed #a7bfd6;border-radius:13px;text-align:center;color:var(--muted)}
.arz-projects .pj-empty h3{border:0;color:var(--navy);margin:10px 0;font-size:1.1rem}
.arz-projects button:focus-visible,.arz-projects summary:focus-visible{outline:3px solid #73b5f6;outline-offset:3px}
.arz-projects .pj-enter{animation:pj-rise .58s both}
@keyframes pj-rise{from{opacity:0;transform:translateY(14px)}to{opacity:1;transform:translateY(0)}}
@media(max-width:767px){.arz-projects .pj-hero{padding:31px 22px}.arz-projects .pj-stats{gap:7px}.arz-projects .pj-stat{padding:12px}.arz-projects .pj-stat strong{font-size:1.2rem}.arz-projects .pj-stat span{font-size:.7rem}.arz-projects .pj-controls,.arz-projects .pj-card{padding:18px}.arz-projects .pj-meta>div{grid-template-columns:78px minmax(0,1fr)}}
@media(prefers-reduced-motion:reduce){.arz-projects *, .arz-projects *::before,.arz-projects *::after{animation:none!important;transition:none!important;scroll-behavior:auto!important}}
<section class="arz-projects" aria-label="Professional and research projects">
  <header class="pj-hero pj-enter">
    <div class="pj-kicker"><i class="bi bi-diagram-3" aria-hidden="true"></i> Selected professional and academic work</div>
    <h1>Projects</h1>
    <p>This section highlights my professional experience in environmental and social impact assessment, renewable energy, transportation infrastructure, environmental monitoring, and academic research.</p>
  </header>
<div class="pj-stats" aria-label="Projects at a glance">
    <div class="pj-stat"><strong>16</strong><span>Projects</span></div>
    <div class="pj-stat"><strong>4</strong><span>Focus areas</span></div>
    <div class="pj-stat"><strong>2020–2025</strong><span>Project periods</span></div>
  </div>
<div class="pj-controls">
    <label class="pj-label" for="pj-search">Search projects, clients, funding, or activities</label>
    <div class="pj-search-wrap">
      <i class="bi bi-search" aria-hidden="true"></i>
      <input class="pj-search" id="pj-search" type="search" placeholder="Try EIA, ADB, railway, solar, monitoring…" autocomplete="off">
    </div>
    <div class="pj-filterbar" role="group" aria-label="Filter projects by focus area">
      <button class="pj-filter" type="button" data-filter="All" aria-pressed="true">All projects (16)</button>
      <button class="pj-filter" type="button" data-filter="Energy" aria-pressed="false">Energy (3)</button>
      <button class="pj-filter" type="button" data-filter="Transport" aria-pressed="false">Transport (9)</button>
      <button class="pj-filter" type="button" data-filter="Environment" aria-pressed="false">Environment (2)</button>
      <button class="pj-filter" type="button" data-filter="Research" aria-pressed="false">Research (2)</button>
    </div>
  </div>
<div class="pj-results">
    <span id="pj-count" role="status" aria-live="polite" aria-atomic="true">Showing 16 of 16 projects</span>
    <button class="pj-reset" id="pj-reset" type="button">Clear filters</button>
  </div>
<div class="container-fluid px-0"><div class="row g-3 pj-grid" id="pj-grid">
    <div class="col-12 col-xl-6 pj-item" data-category="Energy">
      <article class="pj-card" aria-labelledby="pj-title-1">
        <div class="pj-cardtop"><span class="pj-index">01</span><span class="pj-type" data-type="Energy"><i class="bi bi-lightning-charge" aria-hidden="true"></i> Energy</span></div>
        <h3 id="pj-title-1">Consultancy Services for Environmental and Social Assessment and Mitigation Measures for the Gas Sector Energy Efficiency Improvement Project</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Bakhrabad Gas Distribution Company Limited (BGDCL)</dd></div>
          <div><dt>Funding</dt><dd>Asian Infrastructure Investment Bank (AIIB)</dd></div>
          <div><dt>Duration</dt><dd>November 2024 – January 2025 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted Environmental Impact Assessments (EIAs) and Initial Environmental Examinations (IEEs).</li>
            <li>Reviewed baseline environmental data covering air, water, soil, biodiversity, and socioeconomic conditions.</li>
            <li>Collected primary data through environmental quality surveys.</li>
            <li>Engaged with clients, regulatory authorities, local communities, and other stakeholders.</li>
            <li>Recommended mitigation measures and developed environmental monitoring plans.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Energy">
      <article class="pj-card" aria-labelledby="pj-title-2">
        <div class="pj-cardtop"><span class="pj-index">02</span><span class="pj-type" data-type="Energy"><i class="bi bi-sun" aria-hidden="true"></i> Energy</span></div>
        <h3 id="pj-title-2">Floating Solar PV Project at Bakreshwar Reservoir, Birbhum District, West Bengal, India</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>West Bengal Power Development Corporation Limited (WBPDCL)</dd></div>
          <div><dt>Funding</dt><dd>Asian Development Bank (ADB)</dd></div>
          <div><dt>Duration</dt><dd>August 2024 – January 2025 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted EIAs and IEEs to identify potential environmental risks.</li>
            <li>Reviewed baseline environmental and socioeconomic data.</li>
            <li>Coordinated multidisciplinary environmental and social assessment activities.</li>
            <li>Engaged with stakeholders and regulatory authorities.</li>
            <li>Prepared mitigation recommendations, monitoring plans, and technical reports.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Environment">
      <article class="pj-card" aria-labelledby="pj-title-3">
        <div class="pj-cardtop"><span class="pj-index">03</span><span class="pj-type" data-type="Environment"><i class="bi bi-recycle" aria-hidden="true"></i> Environment</span></div>
        <h3 id="pj-title-3">Expansion of Matuail Sanitary Landfill Including Land Development Project</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Dhaka South City Corporation (DSCC)</dd></div>
          <div><dt>Funding</dt><dd>Government of Bangladesh</dd></div>
          <div><dt>Duration</dt><dd>June 2024 – January 2025 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Planned and managed EIA and IEE activities, including scoping, consultation, data collection, and reporting.</li>
            <li>Assessed baseline environmental conditions and potential impacts.</li>
            <li>Coordinated multidisciplinary teams and managed project deliverables.</li>
            <li>Evaluated compliance with applicable environmental regulations.</li>
            <li>Developed mitigation measures and environmental monitoring plans.</li>
            <li>Prepared technical reports and environmental assessment findings.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Transport">
      <article class="pj-card" aria-labelledby="pj-title-4">
        <div class="pj-cardtop"><span class="pj-index">04</span><span class="pj-type" data-type="Transport"><i class="bi bi-train-front" aria-hidden="true"></i> Transport</span></div>
        <h3 id="pj-title-4">Railway Connectivity Improvement Preparatory Facility Project</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Bangladesh Railway (BR)</dd></div>
          <div><dt>Funding</dt><dd>Asian Development Bank (ADB)</dd></div>
          <div><dt>Duration</dt><dd>April 2024 – January 2025 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted EIAs and IEEs and reviewed baseline environmental conditions.</li>
            <li>Coordinated environmental assessment activities and multidisciplinary teams.</li>
            <li>Assessed compliance with environmental regulations and standards.</li>
            <li>Developed mitigation measures and environmental monitoring plans.</li>
            <li>Organized public consultations and incorporated stakeholder feedback into environmental management plans.</li>
            <li>Prepared technical reports and presented findings to clients and regulatory authorities.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Energy">
      <article class="pj-card" aria-labelledby="pj-title-5">
        <div class="pj-cardtop"><span class="pj-index">05</span><span class="pj-type" data-type="Energy"><i class="bi bi-sun" aria-hidden="true"></i> Energy</span></div>
        <h3 id="pj-title-5">Environmental and Social Impact Assessment for Gazaria 50 (±10%) MW Solar PV Power Plant Project, Munshiganj</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Rural Power Company Limited (RPCL)</dd></div>
          <div><dt>Duration</dt><dd>April 2024 – January 2025 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted EIAs and IEEs to identify environmental risks and mitigation measures.</li>
            <li>Reviewed baseline data on air, water, soil, biodiversity, and socioeconomic conditions.</li>
            <li>Supported assessment planning, data collection, and report preparation.</li>
            <li>Coordinated environmental assessment activities and project deliverables.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Transport">
      <article class="pj-card" aria-labelledby="pj-title-6">
        <div class="pj-cardtop"><span class="pj-index">06</span><span class="pj-type" data-type="Transport"><i class="bi bi-bus-front" aria-hidden="true"></i> Transport</span></div>
        <h3 id="pj-title-6">Comprehensive Transport Master Plan and Pre-Feasibility Study of Mass Transit Network and Multimodal Hub for Narayanganj City Corporation</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Narayanganj City Corporation (NCC)</dd></div>
          <div><dt>Duration</dt><dd>March 2023 – June 2024 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted EIAs and IEEs and reviewed baseline environmental data.</li>
            <li>Supported stakeholder consultations, data collection, and environmental assessment planning.</li>
            <li>Evaluated environmental risks and recommended mitigation measures.</li>
            <li>Developed environmental monitoring plans and contributed to technical reporting.</li>
            <li>Coordinated with multidisciplinary teams to integrate environmental considerations into transport planning.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Transport">
      <article class="pj-card" aria-labelledby="pj-title-7">
        <div class="pj-cardtop"><span class="pj-index">07</span><span class="pj-type" data-type="Transport"><i class="bi bi-signpost-split" aria-hidden="true"></i> Transport</span></div>
        <h3 id="pj-title-7">Detailed Feasibility Study and Design of Six Important Bridges</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Roads and Highways Department (RHD)</dd></div>
          <div><dt>Funding</dt><dd>Islamic Development Bank (IsDB)</dd></div>
          <div><dt>Duration</dt><dd>March 2023 – March 2024 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Coordinated desktop studies focusing on environmental components.</li>
            <li>Estimated budgets for baseline environmental monitoring.</li>
            <li>Developed methodologies and Terms of Reference (ToR) for environmental quality surveys.</li>
            <li>Prepared and reviewed ToRs for EIAs.</li>
            <li>Drafted, reviewed, and finalized environmental components of feasibility reports.</li>
            <li>Compiled IEE reports and recommended mitigation measures.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Transport">
      <article class="pj-card" aria-labelledby="pj-title-8">
        <div class="pj-cardtop"><span class="pj-index">08</span><span class="pj-type" data-type="Transport"><i class="bi bi-signpost-split" aria-hidden="true"></i> Transport</span></div>
        <h3 id="pj-title-8">Feasibility Study, Detailed Design, and Preparatory Study of the Dhaka–Chattogram National Highway</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Roads and Highways Department (RHD)</dd></div>
          <div><dt>Funding</dt><dd>Asian Development Bank (ADB)</dd></div>
          <div><dt>Duration</dt><dd>November 2023 – January 2024 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted reconnaissance surveys to identify environmental features and constraints.</li>
            <li>Performed desktop studies and analyzed environmental information.</li>
            <li>Prepared ToRs for environmental quality surveys.</li>
            <li>Prepared environmental components of feasibility reports and recommended sustainable development measures.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Transport">
      <article class="pj-card" aria-labelledby="pj-title-9">
        <div class="pj-cardtop"><span class="pj-index">09</span><span class="pj-type" data-type="Transport"><i class="bi bi-train-front" aria-hidden="true"></i> Transport</span></div>
        <h3 id="pj-title-9">UAE–Oman Railway Link Project (Abu Dhabi–Sohar): Environmental Impact Assessment and Environmental Management Plan</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Ministry of Transport and Communications, Oman Rail</dd></div>
          <div><dt>Duration</dt><dd>September 2023 – October 2023 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Prepared EIA documentation and identified potential environmental impacts.</li>
            <li>Developed mitigation strategies to address environmental risks.</li>
            <li>Coordinated the preparation of Environmental Management Plans.</li>
            <li>Supported environmental monitoring, reporting, and regulatory compliance.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Transport">
      <article class="pj-card" aria-labelledby="pj-title-10">
        <div class="pj-cardtop"><span class="pj-index">10</span><span class="pj-type" data-type="Transport"><i class="bi bi-signpost-split" aria-hidden="true"></i> Transport</span></div>
        <h3 id="pj-title-10">Feasibility Study and Detailed Design of the Second Sultana Kamal Bridge and Upgrading of Two Highway Intersections</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Roads and Highways Department (RHD)</dd></div>
          <div><dt>Duration</dt><dd>March 2023 – August 2023 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted desktop studies and analyzed environmental data.</li>
            <li>Developed methodologies for Initial Environmental Examinations.</li>
            <li>Estimated budgets for baseline environmental monitoring.</li>
            <li>Contributed to environmental risk assessment and feasibility reports.</li>
            <li>Recommended environmental considerations for sustainable infrastructure planning.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Transport">
      <article class="pj-card" aria-labelledby="pj-title-11">
        <div class="pj-cardtop"><span class="pj-index">11</span><span class="pj-type" data-type="Transport"><i class="bi bi-signpost-split" aria-hidden="true"></i> Transport</span></div>
        <h3 id="pj-title-11">Feasibility Study, Preliminary Design, and Detailed Design of Eight Important Bridges in Mymensingh Zone</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Roads and Highways Department (RHD)</dd></div>
          <div><dt>Funding</dt><dd>Islamic Development Bank (IsDB)</dd></div>
          <div><dt>Duration</dt><dd>March 2023 – August 2023 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted desktop studies to assess environmental conditions and potential impacts.</li>
            <li>Estimated budgets for baseline environmental monitoring.</li>
            <li>Contributed to the environmental component of the draft feasibility report.</li>
            <li>Identified environmental risks and recommended mitigation measures.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Transport">
      <article class="pj-card" aria-labelledby="pj-title-12">
        <div class="pj-cardtop"><span class="pj-index">12</span><span class="pj-type" data-type="Transport"><i class="bi bi-signpost" aria-hidden="true"></i> Transport</span></div>
        <h3 id="pj-title-12">Dhaka Outer Ring Road Project</h3>
        <dl class="pj-meta">
          <div><dt>Duration</dt><dd>January 2023 – February 2023</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted desktop studies to evaluate environmental conditions and potential impacts.</li>
            <li>Prepared the environmental component of the draft feasibility report.</li>
            <li>Contributed to the finalization of the environmental component of the final feasibility report.</li>
            <li>Prepared ToRs for environmental quality surveys.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Transport">
      <article class="pj-card" aria-labelledby="pj-title-13">
        <div class="pj-cardtop"><span class="pj-index">13</span><span class="pj-type" data-type="Transport"><i class="bi bi-train-front" aria-hidden="true"></i> Transport</span></div>
        <h3 id="pj-title-13">New Broad Gauge Railway Line from Darshana to Meherpur via Damurhuda and Mujibnagar (DMMRP)</h3>
        <dl class="pj-meta">
          <div><dt>Client</dt><dd>Bangladesh Railway (BR)</dd></div>
          <div><dt>Duration</dt><dd>October 2022 – December 2022</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Prepared and finalized environmental components of feasibility reports.</li>
            <li>Coordinated environmental data collection and analysis.</li>
            <li>Conducted EIAs to identify and evaluate potential environmental impacts.</li>
            <li>Recommended mitigation measures to support regulatory compliance and sustainable development.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Environment">
      <article class="pj-card" aria-labelledby="pj-title-14">
        <div class="pj-cardtop"><span class="pj-index">14</span><span class="pj-type" data-type="Environment"><i class="bi bi-recycle" aria-hidden="true"></i> Environment</span></div>
        <h3 id="pj-title-14">Rehabilitation of BSCIC Industrial Park</h3>
        <dl class="pj-meta">
          <div><dt>Location</dt><dd>Munshiganj</dd></div>
          <div><dt>Duration</dt><dd>July 2021 – March 2022</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Identified and assessed environmental risks and hazards.</li>
            <li>Recommended environmentally friendly mitigation measures.</li>
            <li>Conducted environmental audits to evaluate compliance with environmental standards and regulations.</li>
            <li>Provided recommendations to improve environmental performance and sustainability.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Research">
      <article class="pj-card" aria-labelledby="pj-title-15">
        <div class="pj-cardtop"><span class="pj-index">15</span><span class="pj-type" data-type="Research"><i class="bi bi-journal-text" aria-hidden="true"></i> Research</span></div>
        <h3 id="pj-title-15">Feasibility Study on Concrete Dust as a Substitute for Filling Sand in Road Construction</h3>
        <dl class="pj-meta">
          <div><dt>Duration</dt><dd>January 2020 – June 2021 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted literature reviews and compiled relevant technical information.</li>
            <li>Assisted in designing and implementing surveys, experiments, and field studies.</li>
            <li>Collected and analyzed qualitative and quantitative data.</li>
            <li>Prepared graphs, charts, and visualizations to communicate research findings.</li>
            <li>Interpreted results and contributed to research reports and academic publications.</li>
          </ul>
        </details>
      </article>
    </div>
    <div class="col-12 col-xl-6 pj-item" data-category="Research">
      <article class="pj-card" aria-labelledby="pj-title-16">
        <div class="pj-cardtop"><span class="pj-index">16</span><span class="pj-type" data-type="Research"><i class="bi bi-journal-text" aria-hidden="true"></i> Research</span></div>
        <h3 id="pj-title-16">An Overview of Foot Overbridges in Dhaka City</h3>
        <dl class="pj-meta">
          <div><dt>Duration</dt><dd>January 2020 – June 2021 (Intermittent)</dd></div>
        </dl>
        <details class="pj-details">
          <summary>Activities performed <i class="bi bi-chevron-down" aria-hidden="true"></i></summary>
          <ul>
            <li>Conducted literature reviews on foot overbridges in Dhaka City.</li>
            <li>Assisted in survey design and primary and secondary data collection.</li>
            <li>Analyzed data and prepared visualizations.</li>
            <li>Contributed to research reports and academic publications.</li>
            <li>Coordinated research activities and maintained project documentation.</li>
          </ul>
        </details>
      </article>
    </div>
  </div></div>
  <div class="pj-empty" id="pj-empty" hidden>
    <i class="bi bi-search" aria-hidden="true"></i>
    <h3>No matching projects</h3>
    <p>Try a different keyword or clear the selected category.</p>
  </div>
</section>
<script>
/* Progressive enhancement: all 16 project cards are visible without JavaScript. */
(function () {
  function initProjects() {
    const root = document.querySelector('.arz-projects');
    if (!root) return;
    const search = root.querySelector('#pj-search');
    const buttons = Array.from(root.querySelectorAll('[data-filter]'));
    const items = Array.from(root.querySelectorAll('.pj-item'));
    const count = root.querySelector('#pj-count');
    const empty = root.querySelector('#pj-empty');
    const reset = root.querySelector('#pj-reset');
    let category = 'All';
    const normalizedText = items.map(item => item.textContent.toLocaleLowerCase());

    function update() {
      const words = search.value.trim().toLocaleLowerCase().split(/\s+/).filter(Boolean);
      let visible = 0;
      items.forEach((item, i) => {
        const categoryMatches = category === 'All' || item.dataset.category === category;
        const textMatches = words.every(word => normalizedText[i].includes(word));
        const show = categoryMatches && textMatches;
        item.hidden = !show;
        if (show) visible += 1;
      });
      count.textContent = 'Showing ' + visible + ' of ' + items.length + ' projects';
      empty.hidden = visible !== 0;
    }

    buttons.forEach(button => button.addEventListener('click', () => {
      category = button.dataset.filter;
      buttons.forEach(b => b.setAttribute('aria-pressed', String(b === button)));
      update();
    }));
    search.addEventListener('input', update);
    reset.addEventListener('click', () => {
      category = 'All';
      search.value = '';
      buttons.forEach(b => b.setAttribute('aria-pressed', String(b.dataset.filter === 'All')));
      update();
      search.focus();
    });
    update();
  }
  if (document.readyState === 'loading') document.addEventListener('DOMContentLoaded', initProjects);
  else initProjects();
})();

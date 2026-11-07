---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---
<!-- Delete these two link tags if Bootstrap Grid and Icons are already loaded globally. -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap-grid.min.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
<style>
/* Scoped project-page design: no JavaScript, filters, search, or hidden activities. */
.arz-proj-simple {
  --navy:#112f52; --blue:#1d5081; --accent:#2778c4;
  --muted:#61758b; --border:#dfe8f1; --soft:#f5f9fd;
  width:100%; color:#293e53;
}
.arz-proj-simple *, .arz-proj-simple *::before, .arz-proj-simple *::after {box-sizing:border-box}
.arz-proj-simple .ps-hero {
  position:relative; overflow:hidden; isolation:isolate;
  padding:44px 36px; margin:0 0 22px; border-radius:18px;
  color:#fff; background:linear-gradient(126deg,#102d50 0%,#1b497a 65%,#2876a9 100%);
  animation:ps-appear .6s both;
}
.arz-proj-simple .ps-hero::after {
  content:""; position:absolute; right:-95px; top:-110px; z-index:-1;
  width:260px; height:260px; border-radius:50%; border:1px solid #ffffff38;
  box-shadow:0 0 0 42px #ffffff0a,0 0 0 83px #ffffff08; pointer-events:none;
}
.arz-proj-simple .ps-eyebrow {display:flex;align-items:center;gap:8px;margin-bottom:12px;color:#b9dcff;letter-spacing:1.1px;text-transform:uppercase;font-size:.75rem;font-weight:700}
.arz-proj-simple .ps-hero h1 {margin:0 0 12px;padding:0;border:0;color:#fff;font-weight:800;font-size:clamp(1.8rem,3.5vw,2.5rem);line-height:1.25}
.arz-proj-simple .ps-hero p {max-width:720px;color:#e2edfa;margin:0;font-size:.96rem;line-height:1.8}
.arz-proj-simple .ps-overview {display:flex;flex-wrap:wrap;gap:10px;margin:0 0 28px}
.arz-proj-simple .ps-overview span {display:inline-flex;align-items:center;gap:8px;padding:9px 13px;background:#f1f6fc;border:1px solid var(--border);border-radius:999px;color:#365c7a;font-size:.8rem;font-weight:650}
.arz-proj-simple .ps-overview i {color:var(--accent)}
.arz-proj-simple .ps-heading {display:flex;align-items:center;gap:10px;color:var(--navy);margin:0 0 18px}
.arz-proj-simple .ps-heading h2 {margin:0;padding:0;border:0;color:var(--navy);font-size:1.33rem;font-weight:800}
.arz-proj-simple .ps-heading i {color:var(--accent)}
.arz-proj-simple .ps-list {display:grid;grid-template-columns:minmax(0,1fr);gap:18px}
.arz-proj-simple .ps-card {
  display:block; min-width:0; padding:27px 28px; background:#fff;
  border:1px solid var(--border); border-radius:15px;
  box-shadow:0 4px 18px rgba(17,47,82,.045);
  transition:transform .3s cubic-bezier(.2,.8,.2,1),border-color .3s,box-shadow .3s;
  animation:ps-appear .65s both;
}
.arz-proj-simple .ps-card:hover {transform:translateY(-3px);border-color:#bdd6ed;box-shadow:0 12px 30px rgba(17,47,82,.11)}
.arz-proj-simple .ps-card-title {display:flex;align-items:flex-start;gap:15px;margin:0 0 16px}
.arz-proj-simple .ps-num {flex:0 0 40px;display:inline-flex;align-items:center;justify-content:center;min-width:40px;height:40px;border-radius:11px;background:#e9f3ff;color:#215e99;font-size:.9rem;font-weight:800}
.arz-proj-simple .ps-card h3 {margin:2px 0 0;padding:0;color:var(--navy);font-size:1.08rem;font-weight:750;line-height:1.5;overflow-wrap:anywhere}
.arz-proj-simple .ps-meta {display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:10px 18px;margin:0 0 19px;padding:15px 17px;background:#f7fafd;border:1px solid #e5edf5;border-radius:11px}
.arz-proj-simple .ps-meta div {min-width:0}
.arz-proj-simple .ps-meta dt {margin:0 0 2px;color:#6c8197;font-size:.73rem;font-weight:750;letter-spacing:.02em}
.arz-proj-simple .ps-meta dd {margin:0;color:#35506a;font-size:.86rem;line-height:1.55;overflow-wrap:anywhere}
.arz-proj-simple .ps-activities-title {margin:0 0 10px;color:var(--blue);font-size:.87rem;font-weight:800;display:flex;align-items:center;gap:8px}
.arz-proj-simple .ps-activities-title i {color:var(--accent)}
.arz-proj-simple .ps-activities {margin:0;padding-left:21px;color:#455d72;font-size:.88rem;line-height:1.73}
.arz-proj-simple .ps-activities li {padding-left:2px;margin:0 0 6px}
.arz-proj-simple .ps-activities li:last-child {margin-bottom:0}
.arz-proj-simple .ps-activities li::marker {color:var(--accent)}
@keyframes ps-appear {from{opacity:0;transform:translateY(15px)}to{opacity:1;transform:translateY(0)}}
@media(max-width:767px) {
  .arz-proj-simple .ps-hero {padding:33px 23px;border-radius:14px}
  .arz-proj-simple .ps-card {padding:21px 19px}
  .arz-proj-simple .ps-card-title {gap:10px}
  .arz-proj-simple .ps-num {min-width:34px;flex-basis:34px;height:34px;font-size:.82rem}
  .arz-proj-simple .ps-card h3 {font-size:1rem}
  .arz-proj-simple .ps-meta {grid-template-columns:minmax(0,1fr);padding:13px 14px}
  .arz-proj-simple .ps-activities {font-size:.85rem}
}
@media(prefers-reduced-motion:reduce) {
  .arz-proj-simple *, .arz-proj-simple *::before, .arz-proj-simple *::after {animation:none!important;transition:none!important}
}
<section class="arz-proj-simple" aria-label="Professional and academic projects">
  <header class="ps-hero">
    <div class="ps-eyebrow"><i class="bi bi-briefcase" aria-hidden="true"></i> Professional and academic portfolio</div>
    <h1>Projects</h1>
    <p>This section highlights my professional experience in environmental and social impact assessment, renewable energy, transportation infrastructure, environmental monitoring, and academic research.</p>
  </header>
<div class="ps-overview" aria-label="Project overview">
    <span><i class="bi bi-collection" aria-hidden="true"></i> 16 Projects</span>
    <span><i class="bi bi-calendar3" aria-hidden="true"></i> 2020–2025</span>
    <span><i class="bi bi-journal-check" aria-hidden="true"></i> Consultancy and Research</span>
  </div>
<div class="ps-heading"><i class="bi bi-list-check" aria-hidden="true"></i><h2>Project Portfolio</h2></div>
  <div class="ps-list">
    <article class="ps-card" aria-labelledby="ps-title-1">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">01</span>
        <h3 id="ps-title-1">Consultancy Services for Environmental and Social Assessment and Mitigation Measures for the Gas Sector Energy Efficiency Improvement Project</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Bakhrabad Gas Distribution Company Limited (BGDCL)</dd></div>
        <div><dt>Funding</dt><dd>Asian Infrastructure Investment Bank (AIIB)</dd></div>
        <div><dt>Duration</dt><dd>November 2024 – January 2025 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted Environmental Impact Assessments (EIAs) and Initial Environmental Examinations (IEEs).</li>
        <li>Reviewed baseline environmental data covering air, water, soil, biodiversity, and socioeconomic conditions.</li>
        <li>Collected primary data through environmental quality surveys.</li>
        <li>Engaged with clients, regulatory authorities, local communities, and other stakeholders.</li>
        <li>Recommended mitigation measures and developed environmental monitoring plans.</li>
      </ul>
    </article>
    <article class="ps-card" aria-labelledby="ps-title-2">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">02</span>
        <h3 id="ps-title-2">Floating Solar PV Project at Bakreshwar Reservoir, Birbhum District, West Bengal, India</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>West Bengal Power Development Corporation Limited (WBPDCL)</dd></div>
        <div><dt>Funding</dt><dd>Asian Development Bank (ADB)</dd></div>
        <div><dt>Duration</dt><dd>August 2024 – January 2025 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted EIAs and IEEs to identify potential environmental risks.</li>
        <li>Reviewed baseline environmental and socioeconomic data.</li>
        <li>Coordinated multidisciplinary environmental and social assessment activities.</li>
        <li>Engaged with stakeholders and regulatory authorities.</li>
        <li>Prepared mitigation recommendations, monitoring plans, and technical reports.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-3">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">03</span>
        <h3 id="ps-title-3">Expansion of Matuail Sanitary Landfill Including Land Development Project</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Dhaka South City Corporation (DSCC)</dd></div>
        <div><dt>Funding</dt><dd>Government of Bangladesh</dd></div>
        <div><dt>Duration</dt><dd>June 2024 – January 2025 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Planned and managed EIA and IEE activities, including scoping, consultation, data collection, and reporting.</li>
        <li>Assessed baseline environmental conditions and potential impacts.</li>
        <li>Coordinated multidisciplinary teams and managed project deliverables.</li>
        <li>Evaluated compliance with applicable environmental regulations.</li>
        <li>Developed mitigation measures and environmental monitoring plans.</li>
        <li>Prepared technical reports and environmental assessment findings.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-4">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">04</span>
        <h3 id="ps-title-4">Railway Connectivity Improvement Preparatory Facility Project</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Bangladesh Railway (BR)</dd></div>
        <div><dt>Funding</dt><dd>Asian Development Bank (ADB)</dd></div>
        <div><dt>Duration</dt><dd>April 2024 – January 2025 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted EIAs and IEEs and reviewed baseline environmental conditions.</li>
        <li>Coordinated environmental assessment activities and multidisciplinary teams.</li>
        <li>Assessed compliance with environmental regulations and standards.</li>
        <li>Developed mitigation measures and environmental monitoring plans.</li>
        <li>Organized public consultations and incorporated stakeholder feedback into environmental management plans.</li>
        <li>Prepared technical reports and presented findings to clients and regulatory authorities.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-5">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">05</span>
        <h3 id="ps-title-5">Environmental and Social Impact Assessment for Gazaria 50 (±10%) MW Solar PV Power Plant Project, Munshiganj</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Rural Power Company Limited (RPCL)</dd></div>
        <div><dt>Duration</dt><dd>April 2024 – January 2025 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted EIAs and IEEs to identify environmental risks and mitigation measures.</li>
        <li>Reviewed baseline data on air, water, soil, biodiversity, and socioeconomic conditions.</li>
        <li>Supported assessment planning, data collection, and report preparation.</li>
        <li>Coordinated environmental assessment activities and project deliverables.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-6">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">06</span>
        <h3 id="ps-title-6">Comprehensive Transport Master Plan and Pre-Feasibility Study of Mass Transit Network and Multimodal Hub for Narayanganj City Corporation</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Narayanganj City Corporation (NCC)</dd></div>
        <div><dt>Duration</dt><dd>March 2023 – June 2024 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted EIAs and IEEs and reviewed baseline environmental data.</li>
        <li>Supported stakeholder consultations, data collection, and environmental assessment planning.</li>
        <li>Evaluated environmental risks and recommended mitigation measures.</li>
        <li>Developed environmental monitoring plans and contributed to technical reporting.</li>
        <li>Coordinated with multidisciplinary teams to integrate environmental considerations into transport planning.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-7">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">07</span>
        <h3 id="ps-title-7">Detailed Feasibility Study and Design of Six Important Bridges</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Roads and Highways Department (RHD)</dd></div>
        <div><dt>Funding</dt><dd>Islamic Development Bank (IsDB)</dd></div>
        <div><dt>Duration</dt><dd>March 2023 – March 2024 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Coordinated desktop studies focusing on environmental components.</li>
        <li>Estimated budgets for baseline environmental monitoring.</li>
        <li>Developed methodologies and Terms of Reference (ToR) for environmental quality surveys.</li>
        <li>Prepared and reviewed ToRs for EIAs.</li>
        <li>Drafted, reviewed, and finalized environmental components of feasibility reports.</li>
        <li>Compiled IEE reports and recommended mitigation measures.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-8">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">08</span>
        <h3 id="ps-title-8">Feasibility Study, Detailed Design, and Preparatory Study of the Dhaka–Chattogram National Highway</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Roads and Highways Department (RHD)</dd></div>
        <div><dt>Funding</dt><dd>Asian Development Bank (ADB)</dd></div>
        <div><dt>Duration</dt><dd>November 2023 – January 2024 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted reconnaissance surveys to identify environmental features and constraints.</li>
        <li>Performed desktop studies and analyzed environmental information.</li>
        <li>Prepared ToRs for environmental quality surveys.</li>
        <li>Prepared environmental components of feasibility reports and recommended sustainable development measures.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-9">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">09</span>
        <h3 id="ps-title-9">UAE–Oman Railway Link Project (Abu Dhabi–Sohar): Environmental Impact Assessment and Environmental Management Plan</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Ministry of Transport and Communications, Oman Rail</dd></div>
        <div><dt>Duration</dt><dd>September 2023 – October 2023 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Prepared EIA documentation and identified potential environmental impacts.</li>
        <li>Developed mitigation strategies to address environmental risks.</li>
        <li>Coordinated the preparation of Environmental Management Plans.</li>
        <li>Supported environmental monitoring, reporting, and regulatory compliance.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-10">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">10</span>
        <h3 id="ps-title-10">Feasibility Study and Detailed Design of the Second Sultana Kamal Bridge and Upgrading of Two Highway Intersections</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Roads and Highways Department (RHD)</dd></div>
        <div><dt>Duration</dt><dd>March 2023 – August 2023 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted desktop studies and analyzed environmental data.</li>
        <li>Developed methodologies for Initial Environmental Examinations.</li>
        <li>Estimated budgets for baseline environmental monitoring.</li>
        <li>Contributed to environmental risk assessment and feasibility reports.</li>
        <li>Recommended environmental considerations for sustainable infrastructure planning.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-11">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">11</span>
        <h3 id="ps-title-11">Feasibility Study, Preliminary Design, and Detailed Design of Eight Important Bridges in Mymensingh Zone</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Roads and Highways Department (RHD)</dd></div>
        <div><dt>Funding</dt><dd>Islamic Development Bank (IsDB)</dd></div>
        <div><dt>Duration</dt><dd>March 2023 – August 2023 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted desktop studies to assess environmental conditions and potential impacts.</li>
        <li>Estimated budgets for baseline environmental monitoring.</li>
        <li>Contributed to the environmental component of the draft feasibility report.</li>
        <li>Identified environmental risks and recommended mitigation measures.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-12">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">12</span>
        <h3 id="ps-title-12">Dhaka Outer Ring Road Project</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Duration</dt><dd>January 2023 – February 2023</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted desktop studies to evaluate environmental conditions and potential impacts.</li>
        <li>Prepared the environmental component of the draft feasibility report.</li>
        <li>Contributed to the finalization of the environmental component of the final feasibility report.</li>
        <li>Prepared ToRs for environmental quality surveys.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-13">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">13</span>
        <h3 id="ps-title-13">New Broad Gauge Railway Line from Darshana to Meherpur via Damurhuda and Mujibnagar (DMMRP)</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Client</dt><dd>Bangladesh Railway (BR)</dd></div>
        <div><dt>Duration</dt><dd>October 2022 – December 2022</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Prepared and finalized environmental components of feasibility reports.</li>
        <li>Coordinated environmental data collection and analysis.</li>
        <li>Conducted EIAs to identify and evaluate potential environmental impacts.</li>
        <li>Recommended mitigation measures to support regulatory compliance and sustainable development.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-14">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">14</span>
        <h3 id="ps-title-14">Rehabilitation of BSCIC Industrial Park</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Location</dt><dd>Munshiganj</dd></div>
        <div><dt>Duration</dt><dd>July 2021 – March 2022</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Identified and assessed environmental risks and hazards.</li>
        <li>Recommended environmentally friendly mitigation measures.</li>
        <li>Conducted environmental audits to evaluate compliance with environmental standards and regulations.</li>
        <li>Provided recommendations to improve environmental performance and sustainability.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-15">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">15</span>
        <h3 id="ps-title-15">Feasibility Study on Concrete Dust as a Substitute for Filling Sand in Road Construction</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Duration</dt><dd>January 2020 – June 2021 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted literature reviews and compiled relevant technical information.</li>
        <li>Assisted in designing and implementing surveys, experiments, and field studies.</li>
        <li>Collected and analyzed qualitative and quantitative data.</li>
        <li>Prepared graphs, charts, and visualizations to communicate research findings.</li>
        <li>Interpreted results and contributed to research reports and academic publications.</li>
      </ul>
    </article>

    <article class="ps-card" aria-labelledby="ps-title-16">
      <div class="ps-card-title">
        <span class="ps-num" aria-hidden="true">16</span>
        <h3 id="ps-title-16">An Overview of Foot Overbridges in Dhaka City</h3>
      </div>
      <dl class="ps-meta">
        <div><dt>Duration</dt><dd>January 2020 – June 2021 (Intermittent)</dd></div>
      </dl>
      <h4 class="ps-activities-title"><i class="bi bi-check2-circle" aria-hidden="true"></i> Activities Performed</h4>
      <ul class="ps-activities">
        <li>Conducted literature reviews on foot overbridges in Dhaka City.</li>
        <li>Assisted in survey design and primary and secondary data collection.</li>
        <li>Analyzed data and prepared visualizations.</li>
        <li>Contributed to research reports and academic publications.</li>
        <li>Coordinated research activities and maintained project documentation.</li>
      </ul>
    </article>

</div>
</section>

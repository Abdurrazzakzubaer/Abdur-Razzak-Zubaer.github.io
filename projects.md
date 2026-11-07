
---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

<!-- Bootstrap 5 Grid -->
<link rel="stylesheet"
href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap-grid.min.css">

<!-- Bootstrap Icons -->
<link rel="stylesheet"
href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">

<style>
/* =========================================
   PROJECT PORTFOLIO
   Abdur Razzak Zubaer
========================================= */

.arz-projects {
  --navy: #102d50;
  --primary: #173b68;
  --blue: #2877c7;
  --teal: #168b89;
  --text: #283b50;
  --muted: #60758a;
  --line: #dfe8f1;
  --surface: #f6f9fd;

  width: 100%;
  color: var(--text);
  font-family: inherit;
}

.arz-projects *,
.arz-projects *::before,
.arz-projects *::after {
  box-sizing: border-box;
}

/* HERO */

.arz-projects .project-hero {
  position: relative;
  overflow: hidden;
  margin-bottom: 30px;
  padding: 42px 34px;
  border-radius: 18px;
  background: linear-gradient(
    130deg,
    #102d50,
    #194777 65%,
    #2875ad
  );
  color: #fff;
}

.arz-projects .project-hero::after {
  content: "";
  position: absolute;
  width: 230px;
  height: 230px;
  top: -95px;
  right: -95px;
  border-radius: 50%;
  border: 1px solid rgba(255,255,255,.18);
  box-shadow:
    0 0 0 35px rgba(255,255,255,.035),
    0 0 0 70px rgba(255,255,255,.025);
  pointer-events: none;
}

.arz-projects .hero-label {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  margin-bottom: 12px;
  color: #b9ddff;
  font-size: .76rem;
  font-weight: 700;
  letter-spacing: 1.1px;
  text-transform: uppercase;
}

.arz-projects .project-hero h1 {
  margin: 0 0 14px;
  padding: 0;
  border: 0;
  color: #fff;
  font-size: clamp(1.8rem, 3.8vw, 2.6rem);
  font-weight: 800;
  line-height: 1.2;
}

.arz-projects .project-hero p {
  position: relative;
  z-index: 1;
  max-width: 700px;
  margin: 0;
  color: #e2effb;
  font-size: .96rem;
  line-height: 1.85;
}

/* SUMMARY */

.arz-projects .summary-grid {
  margin-bottom: 32px;
}

.arz-projects .summary-item {
  display: flex;
  align-items: center;
  gap: 13px;
  height: 100%;
  padding: 17px 18px;
  border: 1px solid var(--line);
  border-radius: 12px;
  background: var(--surface);
}

.arz-projects .summary-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  width: 43px;
  height: 43px;
  border-radius: 11px;
  color: var(--blue);
  background: #e5f0fc;
  font-size: 1.2rem;
}

.arz-projects .summary-item strong {
  display: block;
  color: var(--navy);
  font-size: 1.12rem;
  font-weight: 800;
}

.arz-projects .summary-item span {
  display: block;
  color: var(--muted);
  font-size: .79rem;
}

/* SECTION HEADING */

.arz-projects .projects-heading {
  display: flex;
  align-items: center;
  gap: 12px;
  margin: 0 0 22px;
}

.arz-projects .projects-heading i {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 42px;
  height: 42px;
  border-radius: 11px;
  background: #e9f3ff;
  color: var(--blue);
  font-size: 1.2rem;
}

.arz-projects .projects-heading h2 {
  margin: 0;
  padding: 0;
  border: none;
  color: var(--navy);
  font-size: 1.35rem;
  font-weight: 750;
}

/* PROJECT CARDS */

.arz-projects .project-card {
  position: relative;
  overflow: hidden;
  height: 100%;
  padding: 26px;
  border: 1px solid var(--line);
  border-radius: 15px;
  background: #fff;
  box-shadow: 0 4px 18px rgba(20,48,82,.045);
  transition:
    transform .3s ease,
    box-shadow .3s ease,
    border-color .3s ease;
}

.arz-projects .project-card::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 3px;
  background: linear-gradient(
    90deg,
    var(--blue),
    var(--teal)
  );
}

.arz-projects .project-card:hover {
  transform: translateY(-4px);
  border-color: #bfd5eb;
  box-shadow: 0 15px 32px rgba(20,48,82,.11);
}

.arz-projects .project-top {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 12px;
  margin-bottom: 15px;
}

.arz-projects .project-number {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-width: 43px;
  height: 39px;
  padding: 0 9px;
  border-radius: 10px;
  background: #eaf3ff;
  color: var(--primary);
  font-size: .94rem;
  font-weight: 800;
}

.arz-projects .project-type {
  display: inline-flex;
  padding: 6px 10px;
  border-radius: 50px;
  background: #edf7f5;
  color: #21796c;
  font-size: .72rem;
  font-weight: 700;
  text-align: center;
}

.arz-projects .project-title {
  margin: 0 0 17px;
  padding: 0;
  color: var(--navy);
  font-size: 1.12rem;
  font-weight: 750;
  line-height: 1.5;
}

/* METADATA */

.arz-projects .project-meta {
  display: flex;
  flex-direction: column;
  gap: 10px;
  margin-bottom: 21px;
  padding: 15px;
  border-radius: 10px;
  background: var(--surface);
}

.arz-projects .meta-row {
  display: flex;
  align-items: flex-start;
  gap: 9px;
  color: #526980;
  font-size: .84rem;
  line-height: 1.65;
  overflow-wrap: anywhere;
}

.arz-projects .meta-row i {
  flex-shrink: 0;
  margin-top: 3px;
  color: var(--blue);
  font-size: .97rem;
}

.arz-projects .meta-row strong {
  color: #284866;
  font-weight: 700;
}

/* ACTIVITIES */

.arz-projects .activities-title {
  display: flex;
  align-items: center;
  gap: 9px;
  margin: 0 0 12px;
  color: var(--primary);
  font-size: .92rem;
  font-weight: 750;
}

.arz-projects .activities-title i {
  color: var(--teal);
  font-size: 1rem;
}

.arz-projects .activities {
  margin: 0;
  padding: 0;
  list-style: none;
}

.arz-projects .activities li {
  position: relative;
  margin-bottom: 11px;
  padding-left: 19px;
  color: #52667a;
  font-size: .86rem;
  line-height: 1.75;
}

.arz-projects .activities li:last-child {
  margin-bottom: 0;
}

.arz-projects .activities li::before {
  content: "";
  position: absolute;
  top: .65em;
  left: 1px;
  width: 7px;
  height: 7px;
  border-radius: 50%;
  background: var(--teal);
}

/* FOOTER */

.arz-projects .project-footer {
  display: flex;
  align-items: flex-start;
  gap: 13px;
  margin-top: 31px;
  padding: 22px;
  border: 1px solid var(--line);
  border-radius: 13px;
  background: var(--surface);
}

.arz-projects .project-footer i {
  color: var(--blue);
  font-size: 1.25rem;
}

.arz-projects .project-footer p {
  margin: 0;
  color: var(--muted);
  font-size: .89rem;
  line-height: 1.8;
}

/* ANIMATION */

.arz-projects .fade-up {
  animation: projectFadeUp .65s ease both;
}

.arz-projects .delay-1 {
  animation-delay: .08s;
}

.arz-projects .delay-2 {
  animation-delay: .16s;
}

.arz-projects .delay-3 {
  animation-delay: .24s;
}

@keyframes projectFadeUp {
  from {
    opacity: 0;
    transform: translateY(15px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* MOBILE */

@media (max-width: 767px) {
  .arz-projects .project-hero {
    padding: 32px 22px;
    border-radius: 14px;
  }

  .arz-projects .project-card {
    padding: 21px;
  }

  .arz-projects .project-title {
    font-size: 1.04rem;
  }

  .arz-projects .summary-item {
    padding: 15px;
  }
}

/* ACCESSIBILITY */

@media (prefers-reduced-motion: reduce) {
  .arz-projects *,
  .arz-projects *::before,
  .arz-projects *::after {
    animation: none !important;
    transition: none !important;
  }
}
</style>

<div class="arz-projects">

<!-- HERO -->

<header class="project-hero fade-up">
  <div class="hero-label">
    <i class="bi bi-diagram-3"></i>
    Professional &amp; Academic Portfolio
  </div>

  <h1>Projects</h1>

  <p>
    Selected professional and academic projects encompassing
    environmental and social impact assessment, renewable
    energy, transportation infrastructure, environmental
    monitoring, industrial environmental management, and
    applied research.
  </p>
</header>

<!-- SUMMARY -->

<div class="container-fluid px-0 summary-grid">
  <div class="row g-3">

    <div class="col-12 col-sm-6">
      <div class="summary-item">
        <div class="summary-icon">
          <i class="bi bi-briefcase"></i>
        </div>
        <div>
          <strong>16</strong>
          <span>Professional &amp; Research Projects</span>
        </div>
      </div>
    </div>

    <div class="col-12 col-sm-6">
      <div class="summary-item">
        <div class="summary-icon">
          <i class="bi bi-calendar-range"></i>
        </div>
        <div>
          <strong>2020–2025</strong>
          <span>Project Engagement Periods</span>
        </div>
      </div>
    </div>

  </div>
</div>

<!-- PROJECT LIST -->

<section aria-labelledby="project-list-heading">

  <div class="projects-heading">
    <i class="bi bi-collection"></i>
    <h2 id="project-list-heading">
      Professional &amp; Research Projects
    </h2>
  </div>

  <div class="container-fluid px-0">
    <div class="row g-4">

      <!-- PROJECT 01 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-1">

          <div class="project-top">
            <span class="project-number">01</span>
            <span class="project-type">Energy</span>
          </div>

          <h3 class="project-title">
            Consultancy Services for Environmental and Social
            Assessment and Mitigation Measures for the Gas
            Sector Energy Efficiency Improvement Project
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Bakhrabad Gas Distribution Company Limited (BGDCL)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-bank"></i>
              <span><strong>Funding Agency:</strong>
              Asian Infrastructure Investment Bank (AIIB)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              November 2024 – January 2025 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted Environmental Impact Assessments (EIAs) and Initial Environmental Examinations (IEEs).</li>
            <li>Reviewed baseline environmental data covering air, water, soil, biodiversity, and socioeconomic conditions.</li>
            <li>Collected primary data through environmental quality surveys.</li>
            <li>Engaged with clients, regulatory authorities, local communities, and other stakeholders.</li>
            <li>Recommended mitigation measures and developed environmental monitoring plans.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 02 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-2">

          <div class="project-top">
            <span class="project-number">02</span>
            <span class="project-type">Renewable Energy</span>
          </div>

          <h3 class="project-title">
            Floating Solar PV Project at Bakreshwar Reservoir,
            Birbhum District, West Bengal, India
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              West Bengal Power Development Corporation Limited (WBPDCL)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-bank"></i>
              <span><strong>Funding Agency:</strong>
              Asian Development Bank (ADB)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              August 2024 – January 2025 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted EIAs and IEEs to identify potential environmental risks.</li>
            <li>Reviewed baseline environmental and socioeconomic data.</li>
            <li>Coordinated multidisciplinary environmental and social assessment activities.</li>
            <li>Engaged with stakeholders and regulatory authorities.</li>
            <li>Prepared mitigation recommendations, monitoring plans, and technical reports.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 03 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-1">

          <div class="project-top">
            <span class="project-number">03</span>
            <span class="project-type">Waste Management</span>
          </div>

          <h3 class="project-title">
            Expansion of Matuail Sanitary Landfill Including
            Land Development Project
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Dhaka South City Corporation (DSCC)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-bank"></i>
              <span><strong>Funding Agency:</strong>
              Government of Bangladesh</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              June 2024 – January 2025 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Planned and managed EIA and IEE activities, including scoping, consultation, data collection, and reporting.</li>
            <li>Assessed baseline environmental conditions and potential impacts.</li>
            <li>Coordinated multidisciplinary teams and managed project deliverables.</li>
            <li>Evaluated compliance with applicable environmental regulations.</li>
            <li>Developed mitigation measures and environmental monitoring plans.</li>
            <li>Prepared technical reports and environmental assessment findings.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 04 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-2">

          <div class="project-top">
            <span class="project-number">04</span>
            <span class="project-type">Railway</span>
          </div>

          <h3 class="project-title">
            Railway Connectivity Improvement Preparatory
            Facility Project
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Bangladesh Railway (BR)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-bank"></i>
              <span><strong>Funding Agency:</strong>
              Asian Development Bank (ADB)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              April 2024 – January 2025 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted EIAs and IEEs and reviewed baseline environmental conditions.</li>
            <li>Coordinated environmental assessment activities and multidisciplinary teams.</li>
            <li>Assessed compliance with environmental regulations and standards.</li>
            <li>Developed mitigation measures and environmental monitoring plans.</li>
            <li>Organized public consultations and incorporated stakeholder feedback into environmental management plans.</li>
            <li>Prepared technical reports and presented findings to clients and regulatory authorities.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 05 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-1">

          <div class="project-top">
            <span class="project-number">05</span>
            <span class="project-type">Renewable Energy</span>
          </div>

          <h3 class="project-title">
            Environmental and Social Impact Assessment
            for Gazaria 50 (&plusmn;10%) MW Solar PV Power
            Plant Project, Munshiganj
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Rural Power Company Limited (RPCL)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              April 2024 – January 2025 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted EIAs and IEEs to identify environmental risks and mitigation measures.</li>
            <li>Reviewed baseline data on air, water, soil, biodiversity, and socioeconomic conditions.</li>
            <li>Supported assessment planning, data collection, and report preparation.</li>
            <li>Coordinated environmental assessment activities and project deliverables.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 06 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-2">

          <div class="project-top">
            <span class="project-number">06</span>
            <span class="project-type">Urban Transport</span>
          </div>

          <h3 class="project-title">
            Comprehensive Transport Master Plan and
            Pre-Feasibility Study of Mass Transit Network
            and Multimodal Hub for Narayanganj City Corporation
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Narayanganj City Corporation (NCC)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              March 2023 – June 2024 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted EIAs and IEEs and reviewed baseline environmental data.</li>
            <li>Supported stakeholder consultations, data collection, and environmental assessment planning.</li>
            <li>Evaluated environmental risks and recommended mitigation measures.</li>
            <li>Developed environmental monitoring plans and contributed to technical reporting.</li>
            <li>Coordinated with multidisciplinary teams to integrate environmental considerations into transport planning.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 07 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-1">

          <div class="project-top">
            <span class="project-number">07</span>
            <span class="project-type">Bridge Infrastructure</span>
          </div>

          <h3 class="project-title">
            Detailed Feasibility Study and Design
            of Six Important Bridges
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Roads and Highways Department (RHD)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-bank"></i>
              <span><strong>Funding Agency:</strong>
              Islamic Development Bank (IsDB)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              March 2023 – March 2024 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Coordinated desktop studies focusing on environmental components.</li>
            <li>Estimated budgets for baseline environmental monitoring.</li>
            <li>Developed methodologies and Terms of Reference (ToR) for environmental quality surveys.</li>
            <li>Prepared and reviewed ToRs for EIAs.</li>
            <li>Drafted, reviewed, and finalized environmental components of feasibility reports.</li>
            <li>Compiled IEE reports and recommended mitigation measures.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 08 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-2">

          <div class="project-top">
            <span class="project-number">08</span>
            <span class="project-type">Highway</span>
          </div>

          <h3 class="project-title">
            Feasibility Study, Detailed Design, and
            Preparatory Study of the Dhaka–Chattogram
            National Highway
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Roads and Highways Department (RHD)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-bank"></i>
              <span><strong>Funding Agency:</strong>
              Asian Development Bank (ADB)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              November 2023 – January 2024 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted reconnaissance surveys to identify environmental features and constraints.</li>
            <li>Performed desktop studies and analyzed environmental information.</li>
            <li>Prepared ToRs for environmental quality surveys.</li>
            <li>Prepared environmental components of feasibility reports and recommended sustainable development measures.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 09 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-1">

          <div class="project-top">
            <span class="project-number">09</span>
            <span class="project-type">International Railway</span>
          </div>

          <h3 class="project-title">
            UAE–Oman Railway Link Project (Abu Dhabi–Sohar):
            Environmental Impact Assessment and
            Environmental Management Plan
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Ministry of Transport and Communications, Oman Rail</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              September 2023 – October 2023 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Prepared EIA documentation and identified potential environmental impacts.</li>
            <li>Developed mitigation strategies to address environmental risks.</li>
            <li>Coordinated the preparation of Environmental Management Plans.</li>
            <li>Supported environmental monitoring, reporting, and regulatory compliance.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 10 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-2">

          <div class="project-top">
            <span class="project-number">10</span>
            <span class="project-type">Bridge &amp; Highway</span>
          </div>

          <h3 class="project-title">
            Feasibility Study and Detailed Design of
            the Second Sultana Kamal Bridge and
            Upgrading of Two Highway Intersections
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Roads and Highways Department (RHD)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              March 2023 – August 2023 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted desktop studies and analyzed environmental data.</li>
            <li>Developed methodologies for Initial Environmental Examinations.</li>
            <li>Estimated budgets for baseline environmental monitoring.</li>
            <li>Contributed to environmental risk assessment and feasibility reports.</li>
            <li>Recommended environmental considerations for sustainable infrastructure planning.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 11 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-1">

          <div class="project-top">
            <span class="project-number">11</span>
            <span class="project-type">Bridge Infrastructure</span>
          </div>

          <h3 class="project-title">
            Feasibility Study, Preliminary Design, and
            Detailed Design of Eight Important Bridges
            in Mymensingh Zone
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Roads and Highways Department (RHD)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-bank"></i>
              <span><strong>Funding Agency:</strong>
              Islamic Development Bank (IsDB)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              March 2023 – August 2023 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted desktop studies to assess environmental conditions and potential impacts.</li>
            <li>Estimated budgets for baseline environmental monitoring.</li>
            <li>Contributed to the environmental component of the draft feasibility report.</li>
            <li>Identified environmental risks and recommended mitigation measures.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 12 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-2">

          <div class="project-top">
            <span class="project-number">12</span>
            <span class="project-type">Road Infrastructure</span>
          </div>

          <h3 class="project-title">
            Dhaka Outer Ring Road Project
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              January 2023 – February 2023</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted desktop studies to evaluate environmental conditions and potential impacts.</li>
            <li>Prepared the environmental component of the draft feasibility report.</li>
            <li>Contributed to the finalization of the environmental component of the final feasibility report.</li>
            <li>Prepared ToRs for environmental quality surveys.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 13 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-1">

          <div class="project-top">
            <span class="project-number">13</span>
            <span class="project-type">Railway</span>
          </div>

          <h3 class="project-title">
            New Broad Gauge Railway Line from Darshana
            to Meherpur via Damurhuda and Mujibnagar (DMMRP)
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-building"></i>
              <span><strong>Client:</strong>
              Bangladesh Railway (BR)</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              October 2022 – December 2022</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Prepared and finalized environmental components of feasibility reports.</li>
            <li>Coordinated environmental data collection and analysis.</li>
            <li>Conducted EIAs to identify and evaluate potential environmental impacts.</li>
            <li>Recommended mitigation measures to support regulatory compliance and sustainable development.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 14 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-2">

          <div class="project-top">
            <span class="project-number">14</span>
            <span class="project-type">Industrial Environment</span>
          </div>

          <h3 class="project-title">
            Rehabilitation of BSCIC Industrial Park
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-geo-alt"></i>
              <span><strong>Location:</strong>
              Munshiganj</span>
            </div>

            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              July 2021 – March 2022</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Identified and assessed environmental risks and hazards.</li>
            <li>Recommended environmentally friendly mitigation measures.</li>
            <li>Conducted environmental audits to evaluate compliance with environmental standards and regulations.</li>
            <li>Provided recommendations to improve environmental performance and sustainability.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 15 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-1">

          <div class="project-top">
            <span class="project-number">15</span>
            <span class="project-type">Academic Research</span>
          </div>

          <h3 class="project-title">
            Feasibility Study on Concrete Dust as a
            Substitute for Filling Sand in Road Construction
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              January 2020 – June 2021 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted literature reviews and compiled relevant technical information.</li>
            <li>Assisted in designing and implementing surveys, experiments, and field studies.</li>
            <li>Collected and analyzed qualitative and quantitative data.</li>
            <li>Prepared graphs, charts, and visualizations to communicate research findings.</li>
            <li>Interpreted results and contributed to research reports and academic publications.</li>
          </ul>

        </article>
      </div>

      <!-- PROJECT 16 -->

      <div class="col-12 col-xl-6">
        <article class="project-card fade-up delay-2">

          <div class="project-top">
            <span class="project-number">16</span>
            <span class="project-type">Academic Research</span>
          </div>

          <h3 class="project-title">
            An Overview of Foot Overbridges in Dhaka City
          </h3>

          <div class="project-meta">
            <div class="meta-row">
              <i class="bi bi-calendar3"></i>
              <span><strong>Duration:</strong>
              January 2020 – June 2021 (Intermittent)</span>
            </div>
          </div>

          <h4 class="activities-title">
            <i class="bi bi-check2-circle"></i>
            Activities Performed
          </h4>

          <ul class="activities">
            <li>Conducted literature reviews on foot overbridges in Dhaka City.</li>
            <li>Assisted in survey design and primary and secondary data collection.</li>
            <li>Analyzed data and prepared visualizations.</li>
            <li>Contributed to research reports and academic publications.</li>
            <li>Coordinated research activities and maintained project documentation.</li>
          </ul>

        </article>
      </div>

    </div>
  </div>

</section>

<!-- FOOTER -->

<footer class="project-footer">
  <i class="bi bi-info-circle"></i>
  <p>
    The projects presented above reflect professional
    engagements and academic research activities involving
    environmental assessment, infrastructure feasibility,
    environmental monitoring, regulatory considerations,
    technical reporting, and interdisciplinary collaboration.
  </p>
</footer>

</div>

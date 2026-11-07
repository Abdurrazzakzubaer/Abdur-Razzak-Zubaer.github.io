---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

<!-- Bootstrap Responsive Grid -->
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap-grid.min.css"
>

<!-- Bootstrap Icons -->
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css"
>

<style>
/* ==========================================
   ABDUR RAZZAK ZUBAER
   RESEARCH INTERESTS PAGE
========================================== */

.arz-research {
  --rs-navy: #102d50;
  --rs-primary: #173b68;
  --rs-blue: #2877c7;
  --rs-teal: #168b89;
  --rs-text: #293e53;
  --rs-muted: #61768a;
  --rs-border: #e0e8f1;
  --rs-light: #f6f9fd;

  width: 100%;
  color: var(--rs-text);
  font-family: inherit;
}

.arz-research *,
.arz-research *::before,
.arz-research *::after {
  box-sizing: border-box;
}

/* ==========================
   HERO
========================== */

.arz-research .rs-hero {
  position: relative;
  isolation: isolate;
  overflow: hidden;
  padding: 46px 36px;
  margin-bottom: 30px;
  border-radius: 19px;

  background: linear-gradient(
    130deg,
    #102d50 0%,
    #194777 62%,
    #286ea5 100%
  );

  color: #ffffff;
}

.arz-research .rs-hero::after {
  content: "";
  position: absolute;
  top: -105px;
  right: -95px;
  width: 250px;
  height: 250px;
  border: 1px solid rgba(255,255,255,.18);
  border-radius: 50%;

  box-shadow:
    0 0 0 40px rgba(255,255,255,.035),
    0 0 0 80px rgba(255,255,255,.025);

  pointer-events: none;
  z-index: -1;
}

.arz-research .rs-eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 9px;
  margin-bottom: 14px;
  color: #b9ddff;
  font-size: .76rem;
  font-weight: 700;
  letter-spacing: 1.3px;
  text-transform: uppercase;
}

.arz-research .rs-hero h1 {
  margin: 0 0 15px;
  padding: 0;
  border: 0;
  color: #ffffff;
  font-size: clamp(1.8rem, 3.8vw, 2.55rem);
  font-weight: 800;
  line-height: 1.2;
  letter-spacing: -.025em;
}

.arz-research .rs-hero p {
  max-width: 690px;
  margin: 0;
  color: #e0edf9;
  font-size: .98rem;
  line-height: 1.85;
}

/* ==========================
   OVERVIEW
========================== */

.arz-research .rs-overview {
  margin-bottom: 35px;
}

.arz-research .rs-overview-card {
  display: flex;
  align-items: center;
  gap: 13px;
  height: 100%;
  padding: 18px;
  border: 1px solid var(--rs-border);
  border-radius: 13px;
  background: var(--rs-light);

  transition:
    transform .3s ease,
    border-color .3s ease,
    box-shadow .3s ease;
}

.arz-research .rs-overview-card:hover {
  transform: translateY(-4px);
  border-color: #bdd4ec;
  box-shadow: 0 9px 22px rgba(20,48,82,.07);
}

.arz-research .rs-overview-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  width: 46px;
  height: 46px;
  border-radius: 12px;
  background: #e5f0fc;
  color: var(--rs-blue);
  font-size: 1.35rem;
}

.arz-research .rs-overview-card strong {
  display: block;
  margin-bottom: 4px;
  color: var(--rs-navy);
  font-size: .9rem;
  font-weight: 750;
}

.arz-research .rs-overview-card span {
  display: block;
  color: var(--rs-muted);
  font-size: .79rem;
  line-height: 1.5;
}

/* ==========================
   SECTION HEADING
========================== */

.arz-research .rs-section-heading {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-bottom: 23px;
}

.arz-research .rs-section-heading .rs-heading-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  width: 43px;
  height: 43px;
  border-radius: 11px;
  background: #eaf3ff;
  color: var(--rs-blue);
  font-size: 1.2rem;
}

.arz-research .rs-section-heading h2 {
  margin: 0;
  padding: 0;
  border: 0;
  color: var(--rs-navy);
  font-size: 1.36rem;
  font-weight: 750;
}

/* ==========================
   RESEARCH CARDS
========================== */

.arz-research .rs-card {
  position: relative;
  display: flex;
  flex-direction: column;
  height: 100%;
  min-width: 0;
  overflow: hidden;
  padding: 28px;
  border: 1px solid var(--rs-border);
  border-radius: 16px;
  background: #ffffff;

  box-shadow: 0 4px 20px rgba(20,48,82,.045);

  transition:
    transform .32s cubic-bezier(.2,.8,.2,1),
    box-shadow .32s ease,
    border-color .32s ease;
}

.arz-research .rs-card::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 4px;
  background: var(--card-accent);
}

.arz-research .rs-card:hover {
  transform: translateY(-5px);
  border-color: #c4d8eb;
  box-shadow: 0 16px 35px rgba(20,48,82,.11);
}

.arz-research .rs-eia {
  --card-accent: #2877c7;
  --card-icon-bg: #e9f3ff;
}

.arz-research .rs-wash {
  --card-accent: #168b89;
  --card-icon-bg: #e5f6f3;
}

.arz-research .rs-air {
  --card-accent: #6e70b8;
  --card-icon-bg: #eeeeff;
}

/* ==========================
   CARD HEADER
========================== */

.arz-research .rs-card-top {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  margin-bottom: 20px;
}

.arz-research .rs-card-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 61px;
  height: 61px;
  border-radius: 14px;
  background: var(--card-icon-bg);
  color: var(--card-accent);
  font-size: 1.8rem;

  transition: transform .3s ease;
}

.arz-research .rs-card:hover .rs-card-icon {
  transform: scale(1.075);
}

.arz-research .rs-number {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 39px;
  height: 39px;
  border-radius: 10px;
  background: var(--rs-light);
  color: var(--rs-muted);
  font-size: .86rem;
  font-weight: 750;
}

/* ==========================
   CARD CONTENT
========================== */

.arz-research .rs-card h3 {
  margin: 0 0 12px;
  padding: 0;
  border: 0;
  color: var(--rs-navy);
  font-size: 1.24rem;
  font-weight: 800;
  line-height: 1.45;
}

.arz-research .rs-card-description {
  margin: 0 0 22px;
  color: var(--rs-muted);
  font-size: .88rem;
  line-height: 1.8;
}

.arz-research .rs-focus-title {
  display: flex;
  align-items: center;
  gap: 9px;
  margin: 0 0 14px;
  color: var(--rs-primary);
  font-size: .88rem;
  font-weight: 750;
}

.arz-research .rs-focus-title i {
  color: var(--card-accent);
  font-size: 1.05rem;
}

/* ==========================
   RESEARCH TOPIC LIST
========================== */

.arz-research .rs-topics {
  margin: 0;
  padding: 0;
  list-style: none;
}

.arz-research .rs-topics li {
  position: relative;
  margin-bottom: 14px;
  padding-left: 22px;
  color: #526a80;
  font-size: .87rem;
  line-height: 1.75;
}

.arz-research .rs-topics li:last-child {
  margin-bottom: 0;
}

.arz-research .rs-topics li::before {
  content: "";
  position: absolute;
  top: .63em;
  left: 2px;
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: var(--card-accent);
}

/* ==========================
   CLOSING NOTE
========================== */

.arz-research .rs-note {
  display: flex;
  align-items: flex-start;
  gap: 15px;
  margin-top: 34px;
  padding: 24px;
  border: 1px solid var(--rs-border);
  border-radius: 14px;
  background: var(--rs-light);
}

.arz-research .rs-note > i {
  flex-shrink: 0;
  margin-top: 2px;
  color: var(--rs-blue);
  font-size: 1.35rem;
}

.arz-research .rs-note h3 {
  margin: 0 0 8px;
  color: var(--rs-navy);
  font-size: 1rem;
  font-weight: 750;
}

.arz-research .rs-note p {
  margin: 0;
  color: var(--rs-muted);
  font-size: .88rem;
  line-height: 1.8;
}

/* ==========================
   ENTRANCE ANIMATION
========================== */

.arz-research .rs-fade {
  animation: rsFadeUp .7s ease both;
}

.arz-research .rs-delay-1 {
  animation-delay: .08s;
}

.arz-research .rs-delay-2 {
  animation-delay: .16s;
}

.arz-research .rs-delay-3 {
  animation-delay: .24s;
}

@keyframes rsFadeUp {
  from {
    opacity: 0;
    transform: translateY(19px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* ==========================
   MOBILE RESPONSIVENESS
========================== */

@media (max-width: 767px) {

  .arz-research .rs-hero {
    padding: 35px 23px;
    border-radius: 15px;
  }

  .arz-research .rs-card {
    padding: 23px;
  }

  .arz-research .rs-card h3 {
    font-size: 1.12rem;
  }

  .arz-research .rs-note {
    padding: 20px;
  }

  .arz-research .rs-section-heading h2 {
    font-size: 1.23rem;
  }
}

/* ==========================
   ACCESSIBILITY
========================== */

@media (prefers-reduced-motion: reduce) {
  .arz-research *,
  .arz-research *::before,
  .arz-research *::after {
    animation: none !important;
    transition: none !important;
  }
}
</style>

<div class="arz-research">

  <!-- HERO SECTION -->

  <header class="rs-hero rs-fade">

    <div class="rs-eyebrow">
      <i class="bi bi-journal-text"
         aria-hidden="true"></i>
      Academic Research Portfolio
    </div>

    <h1>Research Interests</h1>

    <p>
      My research interests focus on environmental assessment,
      water, sanitation and hygiene (WASH), and air pollution.
      These areas encompass regulatory implementation,
      environmental and social risk assessment, service
      evaluation, and quantitative environmental analysis.
    </p>

  </header>

  <!-- RESEARCH OVERVIEW -->

  <section class="rs-overview"
           aria-label="Research overview">

    <div class="container-fluid px-0">
      <div class="row g-3">

        <div class="col-12 col-md-4">

          <div class="rs-overview-card rs-fade rs-delay-1">

            <div class="rs-overview-icon">
              <i class="bi bi-clipboard-data"
                 aria-hidden="true"></i>
            </div>

            <div>
              <strong>Environmental Assessment</strong>
              <span>Impact assessment &amp; governance</span>
            </div>

          </div>

        </div>

        <div class="col-12 col-md-4">

          <div class="rs-overview-card rs-fade rs-delay-2">

            <div class="rs-overview-icon">
              <i class="bi bi-droplet-half"
                 aria-hidden="true"></i>
            </div>

            <div>
              <strong>WASH</strong>
              <span>Water &amp; sanitation services</span>
            </div>

          </div>

        </div>

        <div class="col-12 col-md-4">

          <div class="rs-overview-card rs-fade rs-delay-3">

            <div class="rs-overview-icon">
              <i class="bi bi-wind"
                 aria-hidden="true"></i>
            </div>

            <div>
              <strong>Air Pollution</strong>
              <span>Air quality &amp; prediction</span>
            </div>

          </div>

        </div>

      </div>
    </div>

  </section>

  <!-- RESEARCH AREAS -->

  <section aria-labelledby="rs-areas-heading">

    <div class="rs-section-heading">
      <div class="rs-heading-icon">
        <i class="bi bi-diagram-3"
           aria-hidden="true"></i>
      </div>

      <h2 id="rs-areas-heading">
        Research Focus Areas
      </h2>
    </div>

    <div class="container-fluid px-0">
      <div class="row g-4">

        <!-- RESEARCH AREA 01: EIA -->

        <div class="col-12 col-lg-6">

          <article class="rs-card rs-eia rs-fade rs-delay-1">

            <div class="rs-card-top">

              <div class="rs-card-icon">
                <i class="bi bi-clipboard-check"
                   aria-hidden="true"></i>
              </div>

              <span class="rs-number">01</span>

            </div>

            <h3>
              Environmental and Social
              Impact Assessment
            </h3>

            <p class="rs-card-description">
              Research concerning environmental and social
              assessment processes, infrastructure-related
              impacts, regulatory implementation, and
              environmental considerations in development
              planning.
            </p>

            <h4 class="rs-focus-title">
              <i class="bi bi-list-check"
                 aria-hidden="true"></i>
              Research Topics
            </h4>

            <ul class="rs-topics">

              <li>
                Environmental and socioeconomic impacts
                of transport infrastructure.
              </li>

              <li>
                Environmental assessment practices and
                regulatory implementation.
              </li>

              <li>
                Environmental considerations in
                infrastructure planning.
              </li>

              <li>
                Assessment of environmental and social
                risks associated with development projects.
              </li>

            </ul>

          </article>

        </div>

        <!-- RESEARCH AREA 02: WASH -->

        <div class="col-12 col-lg-6">

          <article class="rs-card rs-wash rs-fade rs-delay-2">

            <div class="rs-card-top">

              <div class="rs-card-icon">
                <i class="bi bi-droplet-fill"
                   aria-hidden="true"></i>
              </div>

              <span class="rs-number">02</span>

            </div>

            <h3>
              Water, Sanitation, and Hygiene
              (WASH)
            </h3>

            <p class="rs-card-description">
              Research focusing on drinking water and
              sanitation services, urban environmental
              conditions, service quality, and progress
              toward sustainable water and sanitation
              development.
            </p>

            <h4 class="rs-focus-title">
              <i class="bi bi-list-check"
                 aria-hidden="true"></i>
              Research Topics
            </h4>

            <ul class="rs-topics">

              <li>
                Evaluation of drinking water and
                sanitation services.
              </li>

              <li>
                Water and sanitation conditions
                in urban areas.
              </li>

              <li>
                Bangladesh's progress toward
                Sustainable Development Goal 6.
              </li>

              <li>
                Assessment of water and sanitation
                service quality.
              </li>

            </ul>

          </article>

        </div>

        <!-- RESEARCH AREA 03: AIR POLLUTION -->

        <div class="col-12">

          <article class="rs-card rs-air rs-fade rs-delay-3">

            <div class="rs-card-top">

              <div class="rs-card-icon">
                <i class="bi bi-wind"
                   aria-hidden="true"></i>
              </div>

              <span class="rs-number">03</span>

            </div>

            <h3>
              Air Pollution
            </h3>

            <p class="rs-card-description">
              Research involving ambient air quality
              assessment, particulate matter monitoring,
              spatial and temporal pollution patterns,
              emission-related factors, and statistical
              and machine learning approaches to
              air quality prediction.
            </p>

            <h4 class="rs-focus-title">
              <i class="bi bi-list-check"
                 aria-hidden="true"></i>
              Research Topics
            </h4>

            <ul class="rs-topics">

              <li>
                Assessment of ambient air quality and
                air pollution levels in urban areas.
              </li>

              <li>
                Prediction and forecasting of
                PM₂.₅ and PM₁₀ concentrations in Dhaka
                and other major cities in Bangladesh.
              </li>

              <li>
                Spatiotemporal analysis of particulate
                matter concentrations and air pollution
                hotspots.
              </li>

              <li>
                Evaluation of meteorological,
                traffic-related, industrial, and land-use
                factors influencing PM₂.₅ and PM₁₀ levels.
              </li>

              <li>
                Application of machine learning and
                statistical models for air quality
                prediction and pollution trend analysis.
              </li>

            </ul>

          </article>

        </div>

      </div>
    </div>

  </section>

  <!-- RESEARCH SUMMARY -->

  <footer class="rs-note rs-fade rs-delay-3">

    <i class="bi bi-info-circle"
       aria-hidden="true"></i>

    <div>

      <h3>Interdisciplinary Research Interests</h3>

      <p>
        These research interests connect environmental
        engineering, assessment and regulatory practice,
        urban water and sanitation services, and
        data-driven environmental analysis.
      </p>

    </div>

  </footer>

</div>

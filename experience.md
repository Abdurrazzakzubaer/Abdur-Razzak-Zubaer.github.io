---
layout: single
title: "Professional Experience"
permalink: /experience/
author_profile: true
---

<!-- Bootstrap 5 Responsive Grid -->
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
/* =========================================
   PROFESSIONAL EXPERIENCE
   Abdur Razzak Zubaer
   Academic Portfolio
========================================= */

.pe-page {
  --pe-navy: #102d50;
  --pe-primary: #173b68;
  --pe-accent: #2877c7;
  --pe-teal: #178b89;
  --pe-text: #293d52;
  --pe-muted: #64778b;
  --pe-border: #e2eaf2;
  --pe-soft: #f6f9fd;

  width: 100%;
  color: var(--pe-text);
  font-family: inherit;
}

.pe-page *,
.pe-page *::before,
.pe-page *::after {
  box-sizing: border-box;
}

/* HERO SECTION */

.pe-page .pe-hero {
  position: relative;
  isolation: isolate;
  overflow: hidden;
  padding: 46px 36px;
  margin-bottom: 32px;
  border-radius: 19px;
  background: linear-gradient(
    130deg,
    #102d50 0%,
    #194777 62%,
    #266da4 100%
  );
  color: #fff;
}

.pe-page .pe-hero::after {
  content: "";
  position: absolute;
  top: -100px;
  right: -95px;
  width: 250px;
  height: 250px;
  border: 1px solid rgba(255,255,255,.2);
  border-radius: 50%;
  box-shadow:
    0 0 0 38px rgba(255,255,255,.035),
    0 0 0 76px rgba(255,255,255,.025);
  z-index: -1;
  pointer-events: none;
}

.pe-page .pe-eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 9px;
  margin-bottom: 15px;
  color: #b9ddff;
  font-size: .75rem;
  font-weight: 700;
  letter-spacing: 1.35px;
  text-transform: uppercase;
}

.pe-page .pe-hero h1 {
  margin: 0 0 13px;
  padding: 0;
  border: none;
  color: #fff;
  font-size: clamp(1.75rem, 3.5vw, 2.45rem);
  font-weight: 800;
  letter-spacing: -.03em;
  line-height: 1.2;
}

.pe-page .pe-hero p {
  max-width: 650px;
  margin: 0;
  color: #e0eefa;
  font-size: .96rem;
  line-height: 1.85;
}

/* SUMMARY */

.pe-page .pe-summary {
  margin-bottom: 36px;
}

.pe-page .pe-summary-card {
  display: flex;
  align-items: center;
  gap: 14px;
  height: 100%;
  padding: 20px;
  background: var(--pe-soft);
  border: 1px solid var(--pe-border);
  border-radius: 13px;
}

.pe-page .pe-summary-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  width: 46px;
  height: 46px;
  border-radius: 12px;
  background: #e6f0fb;
  color: var(--pe-accent);
  font-size: 1.35rem;
}

.pe-page .pe-summary-value {
  display: block;
  margin-bottom: 4px;
  color: var(--pe-navy);
  font-size: 1.15rem;
  font-weight: 800;
  line-height: 1.3;
}

.pe-page .pe-summary-label {
  display: block;
  color: var(--pe-muted);
  font-size: .81rem;
  line-height: 1.4;
}

/* SECTION HEADING */

.pe-page .pe-section-heading {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-bottom: 24px;
}

.pe-page .pe-section-heading i {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 42px;
  height: 42px;
  flex-shrink: 0;
  border-radius: 11px;
  background: #eaf3ff;
  color: var(--pe-accent);
  font-size: 1.2rem;
}

.pe-page .pe-section-heading h2 {
  margin: 0;
  padding: 0;
  border: none;
  color: var(--pe-navy);
  font-size: 1.4rem;
  font-weight: 750;
}

/* CAREER TIMELINE */

.pe-page .pe-timeline {
  position: relative;
  padding-left: 35px;
}

.pe-page .pe-timeline::before {
  content: "";
  position: absolute;
  top: 16px;
  bottom: 35px;
  left: 14px;
  width: 2px;
  background: linear-gradient(
    to bottom,
    var(--pe-accent),
    #a8cbe8,
    #e0eaf4
  );
}

.pe-page .pe-entry {
  position: relative;
  margin-bottom: 20px;
}

.pe-page .pe-entry:last-child {
  margin-bottom: 0;
}

.pe-page .pe-entry::before {
  content: "";
  position: absolute;
  top: 26px;
  left: -27px;
  width: 13px;
  height: 13px;
  border: 3px solid #fff;
  border-radius: 50%;
  background: var(--pe-accent);
  box-shadow: 0 0 0 2px #bad5ef;
  z-index: 1;
}

.pe-page .pe-entry.pe-current::before {
  background: var(--pe-teal);
  box-shadow: 0 0 0 3px #cdece6;
}

/* EXPERIENCE CARD */

.pe-page .pe-card {
  position: relative;
  overflow: hidden;
  padding: 26px 27px;
  background: #fff;
  border: 1px solid var(--pe-border);
  border-radius: 15px;
  box-shadow: 0 4px 18px rgba(20,48,82,.045);

  transition:
    transform .3s cubic-bezier(.2,.8,.2,1),
    box-shadow .3s ease,
    border-color .3s ease;
}

.pe-page .pe-card::after {
  content: "";
  position: absolute;
  inset: 0 auto 0 0;
  width: 3px;
  background: var(--pe-accent);
  transform: scaleY(0);
  transform-origin: bottom;
  transition: transform .35s ease;
}

.pe-page .pe-card:hover {
  transform: translateY(-4px);
  border-color: #c3d8eb;
  box-shadow: 0 14px 33px rgba(20,48,82,.1);
}

.pe-page .pe-card:hover::after {
  transform: scaleY(1);
}

.pe-page .pe-current .pe-card {
  border-color: #c9dfef;
  background: linear-gradient(
    120deg,
    #fff,
    #f8fbff
  );
}

/* CARD DETAILS */

.pe-page .pe-role {
  margin: 0 0 9px;
  color: var(--pe-navy);
  font-size: 1.2rem;
  font-weight: 800;
  line-height: 1.4;
}

.pe-page .pe-organization {
  display: flex;
  align-items: flex-start;
  gap: 9px;
  margin-bottom: 13px;
  color: var(--pe-primary);
  font-size: .95rem;
  font-weight: 650;
  line-height: 1.6;
}

.pe-page .pe-organization i {
  flex-shrink: 0;
  margin-top: 3px;
  color: var(--pe-accent);
}

.pe-page .pe-affiliation {
  margin: -4px 0 13px 24px;
  color: var(--pe-muted);
  font-size: .84rem;
  font-style: italic;
  line-height: 1.6;
}

.pe-page .pe-bottom {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 13px;
}

.pe-page .pe-period {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 8px 12px;
  border-radius: 8px;
  background: #edf4fb;
  color: #365b7f;
  font-size: .82rem;
  font-weight: 650;
}

.pe-page .pe-period i {
  font-size: .93rem;
}

.pe-page .pe-badge {
  display: inline-flex;
  align-items: center;
  gap: 7px;
  padding: 7px 11px;
  border-radius: 50px;
  background: #e8f6f2;
  color: #167967;
  font-size: .72rem;
  font-weight: 750;
}

.pe-page .pe-badge::before {
  content: "";
  width: 7px;
  height: 7px;
  background: #21987d;
  border-radius: 50%;
}

/* END NOTE */

.pe-page .pe-note {
  display: flex;
  align-items: flex-start;
  gap: 14px;
  margin-top: 32px;
  padding: 22px 24px;
  border: 1px solid var(--pe-border);
  border-radius: 13px;
  background: var(--pe-soft);
}

.pe-page .pe-note > i {
  margin-top: 2px;
  color: var(--pe-accent);
  font-size: 1.25rem;
}

.pe-page .pe-note p {
  margin: 0;
  color: #526980;
  font-size: .9rem;
  line-height: 1.8;
}

/* ENTRANCE ANIMATION */

.pe-page .pe-fade {
  animation: pe-rise .7s ease both;
}

.pe-page .pe-delay-1 { animation-delay: .08s; }
.pe-page .pe-delay-2 { animation-delay: .16s; }
.pe-page .pe-delay-3 { animation-delay: .24s; }
.pe-page .pe-delay-4 { animation-delay: .32s; }
.pe-page .pe-delay-5 { animation-delay: .40s; }
.pe-page .pe-delay-6 { animation-delay: .48s; }

@keyframes pe-rise {
  from {
    opacity: 0;
    transform: translateY(18px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* RESPONSIVE DESIGN */

@media (max-width: 767px) {

  .pe-page .pe-hero {
    padding: 35px 23px;
    border-radius: 15px;
  }

  .pe-page .pe-hero h1 {
    font-size: 1.9rem;
  }

  .pe-page .pe-timeline {
    padding-left: 27px;
  }

  .pe-page .pe-timeline::before {
    left: 10px;
  }

  .pe-page .pe-entry::before {
    left: -23px;
  }

  .pe-page .pe-card {
    padding: 21px 19px;
  }

  .pe-page .pe-role {
    font-size: 1.07rem;
  }

  .pe-page .pe-organization {
    font-size: .88rem;
  }

  .pe-page .pe-note {
    padding: 20px;
  }
}

@media (prefers-reduced-motion: reduce) {
  .pe-page *,
  .pe-page *::before,
  .pe-page *::after {
    animation: none !important;
    transition: none !important;
  }
}
</style>

<main class="pe-page">

  <!-- HERO -->

  <header class="pe-hero pe-fade">

    <div class="pe-eyebrow">
      <i class="bi bi-briefcase"
         aria-hidden="true"></i>
      Academic &amp; Professional Career
    </div>

    <h1>Professional Experience</h1>

    <p>
      A professional journey encompassing university
      teaching, environmental engineering consultancy,
      industrial practice, and academic research.
    </p>

  </header>

  <!-- CAREER SUMMARY -->

  <section class="pe-summary pe-fade pe-delay-1"
           aria-label="Career overview">

    <div class="container-fluid px-0">
      <div class="row g-3">

        <div class="col-12 col-sm-6">

          <div class="pe-summary-card">
            <div class="pe-summary-icon">
              <i class="bi bi-briefcase-fill"
                 aria-hidden="true"></i>
            </div>

            <div>
              <span class="pe-summary-value">6</span>
              <span class="pe-summary-label">
                Professional Positions
              </span>
            </div>
          </div>

        </div>

        <div class="col-12 col-sm-6">

          <div class="pe-summary-card">
            <div class="pe-summary-icon">
              <i class="bi bi-buildings"
                 aria-hidden="true"></i>
            </div>

            <div>
              <span class="pe-summary-value">5</span>
              <span class="pe-summary-label">
                Organizations
              </span>
            </div>
          </div>

        </div>

      </div>
    </div>

  </section>

  <!-- EXPERIENCE TIMELINE -->

  <section aria-labelledby="pe-career-heading">

    <div class="pe-section-heading">
      <i class="bi bi-clock-history"
         aria-hidden="true"></i>
      <h2 id="pe-career-heading">Career Timeline</h2>
    </div>

    <div class="pe-timeline">

      <!-- 1. LECTURER -->

      <article class="pe-entry pe-current pe-fade pe-delay-1">

        <div class="pe-card">

          <h3 class="pe-role">Lecturer</h3>

          <div class="pe-organization">
            <i class="bi bi-building"
               aria-hidden="true"></i>
            <span>
              World University of Bangladesh (WUB)
            </span>
          </div>

          <div class="pe-bottom">

            <span class="pe-period">
              <i class="bi bi-calendar3"
                 aria-hidden="true"></i>
              January 2025 – Present
            </span>

            <span class="pe-badge">
              Current Position
            </span>

          </div>

        </div>

      </article>

      <!-- 2. ENRAC -->

      <article class="pe-entry pe-fade pe-delay-2">

        <div class="pe-card">

          <h3 class="pe-role">Environmental Engineer</h3>

          <div class="pe-organization">
            <i class="bi bi-building"
               aria-hidden="true"></i>
            <span>
              Environment and Resource Analysis
              Center (ENRAC)
            </span>
          </div>

          <div class="pe-bottom">

            <span class="pe-period">
              <i class="bi bi-calendar3"
                 aria-hidden="true"></i>
              April 2024 – January 2025
            </span>

          </div>

        </div>

      </article>

      <!-- 3. ACE JUNIOR ENGINEER -->

      <article class="pe-entry pe-fade pe-delay-3">

        <div class="pe-card">

          <h3 class="pe-role">
            Junior Environmental Engineer
          </h3>

          <div class="pe-organization">
            <i class="bi bi-building"
               aria-hidden="true"></i>
            <span>ACE Consultants Limited</span>
          </div>

          <p class="pe-affiliation">
            Subsidiary of SMEC International Pty Ltd.
          </p>

          <div class="pe-bottom">

            <span class="pe-period">
              <i class="bi bi-calendar3"
                 aria-hidden="true"></i>
              October 2022 – March 2024
            </span>

          </div>

        </div>

      </article>

      <!-- 4. ACE GRADUATE ENGINEER -->

      <article class="pe-entry pe-fade pe-delay-4">

        <div class="pe-card">

          <h3 class="pe-role">Graduate Engineer</h3>

          <div class="pe-organization">
            <i class="bi bi-building"
               aria-hidden="true"></i>
            <span>ACE Consultants Limited</span>
          </div>

          <p class="pe-affiliation">
            Subsidiary of SMEC International Pty Ltd.
          </p>

          <div class="pe-bottom">

            <span class="pe-period">
              <i class="bi bi-calendar3"
                 aria-hidden="true"></i>
              April 2022 – September 2022
            </span>

          </div>

        </div>

      </article>

      <!-- 5. EAGLE FIBRE -->

      <article class="pe-entry pe-fade pe-delay-5">

        <div class="pe-card">

          <h3 class="pe-role">
            Assistant Environmental Engineer
          </h3>

          <div class="pe-organization">
            <i class="bi bi-building"
               aria-hidden="true"></i>
            <span>Eagle Fibre Industries Ltd.</span>
          </div>

          <div class="pe-bottom">

            <span class="pe-period">
              <i class="bi bi-calendar3"
                 aria-hidden="true"></i>
              July 2021 – March 2022
            </span>

          </div>

        </div>

      </article>

      <!-- 6. AUST -->

      <article class="pe-entry pe-fade pe-delay-6">

        <div class="pe-card">

          <h3 class="pe-role">Research Assistant</h3>

          <div class="pe-organization">
            <i class="bi bi-building"
               aria-hidden="true"></i>
            <span>
              Ahsanullah University of Science
              and Technology (AUST)
            </span>
          </div>

          <div class="pe-bottom">

            <span class="pe-period">
              <i class="bi bi-calendar3"
                 aria-hidden="true"></i>
              January 2020 – June 2021
            </span>

          </div>

        </div>

      </article>

    </div>

  </section>

  <!-- SUMMARY NOTE -->

  <footer class="pe-note pe-fade">

    <i class="bi bi-info-circle"
       aria-hidden="true"></i>

    <p>
      This professional experience spans academic
      teaching, environmental engineering consultancy,
      industrial engineering, and research activities
      across university and professional settings.
    </p>

  </footer>

</main>

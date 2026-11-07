---
layout: single
title: "Teaching"
permalink: /teaching/
author_profile: true
---

<!-- Bootstrap 5 Grid -->
<link rel="stylesheet"
href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap-grid.min.css">

<!-- Bootstrap Icons -->
<link rel="stylesheet"
href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">

<style>
/* ==========================================
   TEACHING PORTFOLIO
   Abdur Razzak Zubaer
========================================== */

.arz-teaching {
  --tp-navy: #102d50;
  --tp-primary: #173b68;
  --tp-blue: #2877c7;
  --tp-teal: #168b89;
  --tp-purple: #6e70b8;
  --tp-text: #293e53;
  --tp-muted: #61768a;
  --tp-border: #e0e8f1;
  --tp-light: #f6f9fd;

  width: 100%;
  color: var(--tp-text);
  font-family: inherit;
}

.arz-teaching *,
.arz-teaching *::before,
.arz-teaching *::after {
  box-sizing: border-box;
}

/* HERO */

.arz-teaching .tp-hero {
  position: relative;
  isolation: isolate;
  overflow: hidden;
  padding: 45px 35px;
  margin-bottom: 28px;
  border-radius: 18px;
  background: linear-gradient(
    130deg,
    #102d50 0%,
    #194777 62%,
    #286ea5 100%
  );
  color: #ffffff;
}

.arz-teaching .tp-hero::after {
  content: "";
  position: absolute;
  top: -100px;
  right: -90px;
  width: 240px;
  height: 240px;
  border: 1px solid rgba(255,255,255,.18);
  border-radius: 50%;
  box-shadow:
    0 0 0 40px rgba(255,255,255,.035),
    0 0 0 80px rgba(255,255,255,.025);
  z-index: -1;
}

.arz-teaching .tp-eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 9px;
  margin-bottom: 13px;
  color: #b9ddff;
  font-size: .76rem;
  font-weight: 700;
  letter-spacing: 1.2px;
  text-transform: uppercase;
}

.arz-teaching .tp-hero h1 {
  margin: 0 0 12px;
  padding: 0;
  border: none;
  color: #fff;
  font-size: clamp(1.8rem, 3.6vw, 2.5rem);
  font-weight: 800;
  line-height: 1.2;
}

.arz-teaching .tp-hero p {
  max-width: 650px;
  margin: 0;
  color: #e2edf9;
  font-size: .96rem;
  line-height: 1.8;
}

/* SUMMARY CARDS */

.arz-teaching .tp-summary {
  margin-bottom: 35px;
}

.arz-teaching .tp-stat {
  display: flex;
  align-items: center;
  gap: 13px;
  height: 100%;
  padding: 17px;
  background: var(--tp-light);
  border: 1px solid var(--tp-border);
  border-radius: 12px;
}

.arz-teaching .tp-stat-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  width: 45px;
  height: 45px;
  border-radius: 11px;
  background: #e9f3ff;
  color: var(--tp-blue);
  font-size: 1.35rem;
}

.arz-teaching .tp-stat strong {
  display: block;
  margin-bottom: 4px;
  color: var(--tp-navy);
  font-size: 1.2rem;
  font-weight: 800;
}

.arz-teaching .tp-stat span {
  display: block;
  color: var(--tp-muted);
  font-size: .8rem;
  line-height: 1.4;
}

/* SECTION HEADERS */

.arz-teaching .tp-section {
  margin-bottom: 35px;
}

.arz-teaching .tp-section-head {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-bottom: 20px;
}

.arz-teaching .tp-section-head-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 43px;
  height: 43px;
  flex-shrink: 0;
  border-radius: 11px;
  background: #eaf3ff;
  color: var(--tp-blue);
  font-size: 1.25rem;
}

.arz-teaching .tp-section-head h2 {
  margin: 0;
  padding: 0;
  border: 0;
  color: var(--tp-navy);
  font-size: 1.37rem;
  font-weight: 750;
}

/* COURSE CARD */

.arz-teaching .tp-card {
  position: relative;
  display: flex;
  flex-direction: column;
  height: 100%;
  min-width: 0;
  overflow: hidden;
  padding: 24px;
  border: 1px solid var(--tp-border);
  border-radius: 15px;
  background: #fff;
  box-shadow: 0 4px 17px rgba(20,48,82,.045);

  transition:
    transform .3s cubic-bezier(.2,.8,.2,1),
    border-color .3s ease,
    box-shadow .3s ease;
}

.arz-teaching .tp-card::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 3px;
  background: var(--card-accent);
}

.arz-teaching .tp-card:hover {
  transform: translateY(-5px);
  border-color: #c1d6eb;
  box-shadow: 0 15px 32px rgba(20,48,82,.1);
}

.arz-teaching .tp-theory {
  --card-accent: #2877c7;
  --card-icon-bg: #eaf3ff;
}

.arz-teaching .tp-lab {
  --card-accent: #168b89;
  --card-icon-bg: #e5f6f3;
}

.arz-teaching .tp-sessional {
  --card-accent: #6e70b8;
  --card-icon-bg: #eeeeff;
}

/* COURSE CONTENT */

.arz-teaching .tp-card-top {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  margin-bottom: 18px;
}

.arz-teaching .tp-course-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 52px;
  height: 52px;
  border-radius: 13px;
  background: var(--card-icon-bg);
  color: var(--card-accent);
  font-size: 1.55rem;
}

.arz-teaching .tp-course-type {
  display: inline-flex;
  padding: 6px 11px;
  border-radius: 50px;
  color: var(--card-accent);
  background: var(--card-icon-bg);
  font-size: .75rem;
  font-weight: 700;
}

.arz-teaching .tp-course-code {
  display: inline-flex;
  align-self: flex-start;
  margin-bottom: 12px;
  padding: 7px 11px;
  border-radius: 8px;
  background: var(--tp-light);
  color: #3f6385;
  font-size: .83rem;
  font-weight: 750;
  letter-spacing: .2px;
}

.arz-teaching .tp-card h3 {
  margin: 0;
  color: var(--tp-navy);
  font-size: 1.13rem;
  font-weight: 750;
  line-height: 1.55;
}

/* FOOTER NOTE */

.arz-teaching .tp-note {
  display: flex;
  align-items: flex-start;
  gap: 14px;
  margin-top: 12px;
  padding: 23px;
  border: 1px solid var(--tp-border);
  border-radius: 13px;
  background: var(--tp-light);
}

.arz-teaching .tp-note > i {
  margin-top: 2px;
  color: var(--tp-blue);
  font-size: 1.3rem;
}

.arz-teaching .tp-note p {
  margin: 0;
  color: var(--tp-muted);
  font-size: .9rem;
  line-height: 1.8;
}

/* ANIMATION */

.arz-teaching .tp-fade {
  animation: tpFadeUp .65s ease both;
}

.arz-teaching .tp-delay-1 {
  animation-delay: .08s;
}

.arz-teaching .tp-delay-2 {
  animation-delay: .16s;
}

.arz-teaching .tp-delay-3 {
  animation-delay: .24s;
}

@keyframes tpFadeUp {
  from {
    opacity: 0;
    transform: translateY(17px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* MOBILE */

@media (max-width: 767px) {
  .arz-teaching .tp-hero {
    padding: 33px 22px;
    border-radius: 14px;
  }

  .arz-teaching .tp-card {
    padding: 21px;
  }

  .arz-teaching .tp-card h3 {
    font-size: 1.06rem;
  }

  .arz-teaching .tp-section-head h2 {
    font-size: 1.22rem;
  }
}

/* ACCESSIBILITY */

@media (prefers-reduced-motion: reduce) {
  .arz-teaching *,
  .arz-teaching *::before,
  .arz-teaching *::after {
    animation: none !important;
    transition: none !important;
  }
}
</style>

<div class="arz-teaching">

  <!-- HERO -->

  <header class="tp-hero tp-fade">
    <div class="tp-eyebrow">
      <i class="bi bi-mortarboard"
         aria-hidden="true"></i>
      Academic Teaching Portfolio
    </div>

    <h1>Courses Taught</h1>

    <p>
      An overview of my teaching experience in
      civil and environmental engineering,
      covering theoretical instruction,
      laboratory practice, and sessional courses.
    </p>
  </header>

  <!-- SUMMARY -->

  <section class="tp-summary"
           aria-label="Teaching overview">

    <div class="container-fluid px-0">
      <div class="row g-3">

        <div class="col-12 col-sm-4">
          <div class="tp-stat tp-fade tp-delay-1">
            <div class="tp-stat-icon">
              <i class="bi bi-book"
                 aria-hidden="true"></i>
            </div>
            <div>
              <strong>4</strong>
              <span>Theory Courses</span>
            </div>
          </div>
        </div>

        <div class="col-12 col-sm-4">
          <div class="tp-stat tp-fade tp-delay-2">
            <div class="tp-stat-icon">
              <i class="bi bi-flask"
                 aria-hidden="true"></i>
            </div>
            <div>
              <strong>1</strong>
              <span>Lab Course</span>
            </div>
          </div>
        </div>

        <div class="col-12 col-sm-4">
          <div class="tp-stat tp-fade tp-delay-3">
            <div class="tp-stat-icon">
              <i class="bi bi-pencil-square"
                 aria-hidden="true"></i>
            </div>
            <div>
              <strong>3</strong>
              <span>Sessional Courses</span>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- THEORY COURSES -->

  <section class="tp-section"
           aria-labelledby="tp-theory-heading">

    <div class="tp-section-head">
      <div class="tp-section-head-icon">
        <i class="bi bi-journal-bookmark-fill"
           aria-hidden="true"></i>
      </div>
      <h2 id="tp-theory-heading">Theory Courses</h2>
    </div>

    <div class="container-fluid px-0">
      <div class="row g-3">

        <div class="col-12 col-md-6">
          <article class="tp-card tp-theory tp-fade tp-delay-1">
            <div class="tp-card-top">
              <div class="tp-course-icon">
                <i class="bi bi-recycle"
                   aria-hidden="true"></i>
              </div>
              <span class="tp-course-type">Theory</span>
            </div>
            <span class="tp-course-code">CE07324213</span>
            <h3>Solid Waste Management</h3>
          </article>
        </div>

        <div class="col-12 col-md-6">
          <article class="tp-card tp-theory tp-fade tp-delay-2">
            <div class="tp-card-top">
              <div class="tp-course-icon">
                <i class="bi bi-water"
                   aria-hidden="true"></i>
              </div>
              <span class="tp-course-type">Theory</span>
            </div>
            <span class="tp-course-code">CE07323211</span>
            <h3>Hydrology</h3>
          </article>
        </div>

        <div class="col-12 col-md-6">
          <article class="tp-card tp-theory tp-fade tp-delay-1">
            <div class="tp-card-top">
              <div class="tp-course-icon">
                <i class="bi bi-compass"
                   aria-hidden="true"></i>
              </div>
              <span class="tp-course-type">Theory</span>
            </div>
            <span class="tp-course-code">CE07321311</span>
            <h3>Advanced Surveying</h3>
          </article>
        </div>

        <div class="col-12 col-md-6">
          <article class="tp-card tp-theory tp-fade tp-delay-2">
            <div class="tp-card-top">
              <div class="tp-course-icon">
                <i class="bi bi-train-front"
                   aria-hidden="true"></i>
              </div>
              <span class="tp-course-type">Theory</span>
            </div>
            <span class="tp-course-code">CE07324107</span>
            <h3>Railway Engineering</h3>
          </article>
        </div>

      </div>
    </div>
  </section>

  <!-- LAB COURSES -->

  <section class="tp-section"
           aria-labelledby="tp-lab-heading">

    <div class="tp-section-head">
      <div class="tp-section-head-icon">
        <i class="bi bi-droplet-half"
           aria-hidden="true"></i>
      </div>
      <h2 id="tp-lab-heading">Lab Courses</h2>
    </div>

    <div class="container-fluid px-0">
      <div class="row g-3">

        <div class="col-12">
          <article class="tp-card tp-lab tp-fade tp-delay-1">
            <div class="tp-card-top">
              <div class="tp-course-icon">
                <i class="bi bi-water"
                   aria-hidden="true"></i>
              </div>
              <span class="tp-course-type">Laboratory</span>
            </div>
            <span class="tp-course-code">CE07322212</span>
            <h3>Fluid Mechanics Lab</h3>
          </article>
        </div>

      </div>
    </div>
  </section>

  <!-- SESSIONAL COURSES -->

  <section class="tp-section"
           aria-labelledby="tp-sessional-heading">

    <div class="tp-section-head">
      <div class="tp-section-head-icon">
        <i class="bi bi-pencil-square"
           aria-hidden="true"></i>
      </div>
      <h2 id="tp-sessional-heading">Sessional Courses</h2>
    </div>

    <div class="container-fluid px-0">
      <div class="row g-3">

        <div class="col-12 col-md-6">
          <article class="tp-card tp-sessional tp-fade tp-delay-1">
            <div class="tp-card-top">
              <div class="tp-course-icon">
                <i class="bi bi-tree"
                   aria-hidden="true"></i>
              </div>
              <span class="tp-course-type">Sessional</span>
            </div>
            <span class="tp-course-code">CE07324214</span>
            <h3>Environmental Engineering Sessional</h3>
          </article>
        </div>

        <div class="col-12 col-md-6">
          <article class="tp-card tp-sessional tp-fade tp-delay-2">
            <div class="tp-card-top">
              <div class="tp-course-icon">
                <i class="bi bi-droplet"
                   aria-hidden="true"></i>
              </div>
              <span class="tp-course-type">Sessional</span>
            </div>
            <span class="tp-course-code">CE07324310</span>
            <h3>Water Resource Engineering Sessional</h3>
          </article>
        </div>

        <div class="col-12">
          <article class="tp-card tp-sessional tp-fade tp-delay-3">
            <div class="tp-card-top">
              <div class="tp-course-icon">
                <i class="bi bi-building"
                   aria-hidden="true"></i>
              </div>
              <span class="tp-course-type">Sessional</span>
            </div>
            <span class="tp-course-code">CE07323120</span>
            <h3>Steel Structure Sessional</h3>
          </article>
        </div>

      </div>
    </div>
  </section>

  <!-- FOOTER -->

  <footer class="tp-note tp-fade tp-delay-3">
    <i class="bi bi-info-circle"
       aria-hidden="true"></i>
    <p>
      The courses listed above represent teaching
      activities in civil and environmental engineering,
      spanning theoretical learning, laboratory exercises,
      and sessional instruction.
    </p>
  </footer>

</div>

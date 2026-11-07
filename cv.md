---
layout: single
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
---

<!-- Bootstrap Responsive Grid -->
<link
  href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap-grid.min.css"
  rel="stylesheet"
>

<!-- Bootstrap Icons -->
<link
  href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css"
  rel="stylesheet"
>

<style>
/* ======================================
   Curriculum Vitae | Academic Portfolio
====================================== */

.cv-page {
  --cv-primary: #173b68;
  --cv-primary-dark: #102d50;
  --cv-accent: #2877c7;
  --cv-text: #24354a;
  --cv-muted: #62758a;
  --cv-border: #e1e8f0;
  --cv-bg: #ffffff;

  width: 100%;
  margin: 0 auto;
  font-family: inherit;
  color: var(--cv-text);
}

.cv-page *,
.cv-page *::before,
.cv-page *::after {
  box-sizing: border-box;
}

/* =====================
   Hero Section
===================== */

.cv-hero {
  position: relative;
  overflow: hidden;
  padding: 46px 32px;
  margin-bottom: 32px;
  border-radius: 18px;
  background: linear-gradient(
    135deg,
    #102d50 0%,
    #1b4c80 65%,
    #2877b7 100%
  );
  color: #ffffff;
  animation: cv-fade-up .7s ease both;
}

.cv-hero::after {
  content: "";
  position: absolute;
  top: -90px;
  right: -75px;
  width: 220px;
  height: 220px;
  border-radius: 50%;
  border: 1px solid rgba(255,255,255,.17);
  box-shadow:
    0 0 0 35px rgba(255,255,255,.035),
    0 0 0 75px rgba(255,255,255,.025);
  pointer-events: none;
}

.cv-eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 9px;
  margin-bottom: 13px;
  color: #b9ddff;
  font-size: .76rem;
  font-weight: 700;
  letter-spacing: 1.4px;
  text-transform: uppercase;
}

.cv-hero h2 {
  margin: 0 0 13px;
  padding: 0;
  border: none;
  color: #ffffff;
  font-size: clamp(1.75rem, 3.5vw, 2.4rem);
  font-weight: 750;
  line-height: 1.2;
}

.cv-hero p {
  max-width: 590px;
  margin: 0;
  color: #e0ebf7;
  font-size: .97rem;
  line-height: 1.8;
}

/* =====================
   Section Heading
===================== */

.cv-section {
  margin-bottom: 24px;
}

.cv-section h3 {
  margin: 0 0 9px;
  padding: 0;
  border: none;
  color: var(--cv-primary);
  font-size: 1.3rem;
  font-weight: 750;
}

.cv-section p {
  margin: 0;
  color: var(--cv-muted);
  font-size: .94rem;
  line-height: 1.7;
}

/* =====================
   Document Cards
===================== */

.cv-card {
  position: relative;
  display: flex;
  flex-direction: column;
  height: 100%;
  min-width: 0;
  padding: 28px;
  overflow: hidden;
  background: var(--cv-bg);
  border: 1px solid var(--cv-border);
  border-radius: 16px;
  box-shadow: 0 4px 18px rgba(18,48,82,.04);

  transition:
    transform .32s cubic-bezier(.2,.8,.2,1),
    box-shadow .32s ease,
    border-color .32s ease;
}

.cv-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  height: 3px;
  width: 100%;
  background: var(--cv-card-accent);
  transform: scaleX(0);
  transform-origin: left;
  transition: transform .35s ease;
}

.cv-card:hover,
.cv-card:focus-within {
  transform: translateY(-6px);
  border-color: #c2d5e9;
  box-shadow: 0 15px 36px rgba(22,53,85,.12);
}

.cv-card:hover::before,
.cv-card:focus-within::before {
  transform: scaleX(1);
}

.cv-academic {
  --cv-card-accent: #2877c7;
  --cv-icon-bg: #eaf3ff;
}

.cv-detailed {
  --cv-card-accent: #397b83;
  --cv-icon-bg: #e8f5f4;
}

/* =====================
   Card Icons
===================== */

.cv-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 60px;
  height: 60px;
  margin-bottom: 22px;
  border-radius: 14px;
  color: var(--cv-card-accent);
  background: var(--cv-icon-bg);
  font-size: 1.75rem;
  transition: transform .3s ease;
}

.cv-card:hover .cv-icon {
  transform: scale(1.07);
}

/* =====================
   Card Content
===================== */

.cv-card h4 {
  margin: 0 0 11px;
  color: var(--cv-primary);
  font-size: 1.25rem;
  font-weight: 750;
}

.cv-description {
  margin: 0 0 21px;
  color: var(--cv-muted);
  font-size: .92rem;
  line-height: 1.8;
}

.cv-features {
  display: flex;
  flex-direction: column;
  gap: 11px;
  margin: 0 0 26px;
  padding: 0;
  list-style: none;
}

.cv-features li {
  display: flex;
  align-items: flex-start;
  gap: 10px;
  color: #536880;
  font-size: .89rem;
  line-height: 1.5;
}

.cv-features i {
  flex-shrink: 0;
  margin-top: 2px;
  color: var(--cv-card-accent);
  font-size: .95rem;
}

.cv-card-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: auto;
}

/* =====================
   Action Buttons
===================== */

.cv-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 9px;
  min-height: 43px;
  padding: 11px 16px;
  border: 1px solid transparent;
  border-radius: 9px;
  font-family: inherit;
  font-size: .86rem;
  font-weight: 700;
  line-height: 1.3;
  text-decoration: none !important;
  cursor: pointer;

  transition:
    background .25s ease,
    color .25s ease,
    border-color .25s ease,
    transform .25s ease;
}

.cv-btn-primary {
  flex: 1 1 155px;
  background: var(--cv-primary);
  color: #ffffff !important;
}

.cv-btn-primary:hover {
  background: #235b94;
  color: #ffffff !important;
  transform: translateY(-2px);
}

.cv-btn-outline {
  flex: 1 1 110px;
  background: #f7faff;
  color: var(--cv-primary) !important;
  border-color: #dce7f2;
}

.cv-btn-outline:hover {
  background: #e8f2fc;
  border-color: #bdd5eb;
  color: var(--cv-primary) !important;
  transform: translateY(-2px);
}

.cv-btn:focus-visible {
  outline: 3px solid #73b6ff;
  outline-offset: 3px;
}

/* =====================
   Information Footer
===================== */

.cv-info {
  display: flex;
  align-items: flex-start;
  gap: 16px;
  margin-top: 34px;
  padding: 23px 25px;
  border: 1px solid #dfe8f1;
  border-radius: 13px;
  background: #f7fafd;
}

.cv-info-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  width: 42px;
  height: 42px;
  border-radius: 11px;
  background: #eaf3ff;
  color: var(--cv-accent);
  font-size: 1.2rem;
}

.cv-info h4 {
  margin: 0 0 5px;
  color: var(--cv-primary);
  font-size: .96rem;
  font-weight: 750;
}

.cv-info p {
  margin: 0;
  color: #62758a;
  font-size: .87rem;
  line-height: 1.7;
}

/* =====================
   Animations
===================== */

.cv-animate {
  animation: cv-fade-up .7s ease both;
}

.cv-delay-1 {
  animation-delay: .1s;
}

.cv-delay-2 {
  animation-delay: .2s;
}

.cv-delay-3 {
  animation-delay: .3s;
}

@keyframes cv-fade-up {
  from {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* =====================
   Mobile Optimization
===================== */

@media (max-width: 767px) {

  .cv-hero {
    padding: 34px 23px;
    border-radius: 14px;
  }

  .cv-card {
    padding: 23px;
  }

  .cv-card-actions {
    flex-direction: column;
  }

  .cv-btn {
    flex: none;
    width: 100%;
  }

  .cv-info {
    padding: 20px;
  }
}

/* Accessibility */

@media (prefers-reduced-motion: reduce) {
  .cv-page *,
  .cv-page *::before,
  .cv-page *::after {
    animation: none !important;
    transition: none !important;
    scroll-behavior: auto !important;
  }
}
</style>

<section class="cv-page" aria-label="Curriculum Vitae">

  <!-- Hero Section -->

  <header class="cv-hero">

    <div class="cv-eyebrow">
      <i class="bi bi-person-badge" aria-hidden="true"></i>
      Academic Portfolio
    </div>

    <h2>Curriculum Vitae</h2>

    <p>
      Explore my academic qualifications, research activities,
      professional experience, technical expertise, and
      scholarly contributions through the CV documents below.
    </p>

  </header>

  <!-- Section Heading -->

  <div class="cv-section">
    <h3>Explore My CV</h3>

    <p>
      Choose the document that best suits your requirements.
      Both versions are available in PDF format for viewing
      and downloading.
    </p>
  </div>

  <!-- Bootstrap Cards -->

  <div class="container-fluid px-0">
    <div class="row g-4">

      <!-- Academic CV -->

      <div class="col-12 col-md-6">

        <article class="cv-card cv-academic cv-animate cv-delay-1">

          <div class="cv-icon">
            <i class="bi bi-mortarboard-fill"
               aria-hidden="true"></i>
          </div>

          <h4>Academic CV</h4>

          <p class="cv-description">
            A focused overview of my educational background,
            research interests, publications, teaching
            experience, and academic contributions.
          </p>

          <ul class="cv-features">

            <li>
              <i class="bi bi-check-circle-fill"
                 aria-hidden="true"></i>
              Academic Qualifications
            </li>

            <li>
              <i class="bi bi-check-circle-fill"
                 aria-hidden="true"></i>
              Research Interests &amp; Publications
            </li>

            <li>
              <i class="bi bi-check-circle-fill"
                 aria-hidden="true"></i>
              Teaching &amp; Academic Activities
            </li>

            <li>
              <i class="bi bi-check-circle-fill"
                 aria-hidden="true"></i>
              Scholarly Contributions
            </li>

          </ul>

          <div class="cv-card-actions">

            <a
              class="cv-btn cv-btn-outline"
              href="/Abdur-Razzak-Zubaer.github.io/files/CV_Academic_Abdur%20Razzak%20Zubaer.pdf"
              target="_blank"
              rel="noopener noreferrer"
              aria-label="Preview Academic CV PDF in a new tab"
            >
              <i class="bi bi-eye" aria-hidden="true"></i>
              Preview
            </a>

            <a
              class="cv-btn cv-btn-primary"
              href="/Abdur-Razzak-Zubaer.github.io/files/CV_Academic_Abdur%20Razzak%20Zubaer.pdf"
              download="CV_Academic_Abdur_Razzak_Zubaer.pdf"
              aria-label="Download Academic CV as PDF"
            >
              <i class="bi bi-download" aria-hidden="true"></i>
              Download PDF
            </a>

          </div>

        </article>

      </div>

      <!-- Detailed CV -->

      <div class="col-12 col-md-6">

        <article class="cv-card cv-detailed cv-animate cv-delay-2">

          <div class="cv-icon">
            <i class="bi bi-file-earmark-person-fill"
               aria-hidden="true"></i>
          </div>

          <h4>Detailed CV</h4>

          <p class="cv-description">
            A comprehensive record of my professional
            background, technical competencies, project
            experience, academic activities, and achievements.
          </p>

          <ul class="cv-features">

            <li>
              <i class="bi bi-check-circle-fill"
                 aria-hidden="true"></i>
              Professional Experience
            </li>

            <li>
              <i class="bi bi-check-circle-fill"
                 aria-hidden="true"></i>
              Technical Skills &amp; Expertise
            </li>

            <li>
              <i class="bi bi-check-circle-fill"
                 aria-hidden="true"></i>
              Projects &amp; Responsibilities
            </li>

            <li>
              <i class="bi bi-check-circle-fill"
                 aria-hidden="true"></i>
              Professional Achievements
            </li>

          </ul>

          <div class="cv-card-actions">

            <a
              class="cv-btn cv-btn-outline"
              href="/Abdur-Razzak-Zubaer.github.io/files/CV%20Abdur%20Razzak%20Zubaer_Detailed.pdf"
              target="_blank"
              rel="noopener noreferrer"
              aria-label="Preview Detailed CV PDF in a new tab"
            >
              <i class="bi bi-eye" aria-hidden="true"></i>
              Preview
            </a>

            <a
              class="cv-btn cv-btn-primary"
              href="/Abdur-Razzak-Zubaer.github.io/files/CV%20Abdur%20Razzak%20Zubaer_Detailed.pdf"
              download="CV_Abdur_Razzak_Zubaer_Detailed.pdf"
              aria-label="Download Detailed CV as PDF"
            >
              <i class="bi bi-download" aria-hidden="true"></i>
              Download PDF
            </a>

          </div>

        </article>

      </div>

    </div>
  </div>

  <!-- Information Footer -->

  <footer class="cv-info cv-animate cv-delay-3">

    <div class="cv-info-icon">
      <i class="bi bi-info-circle"
         aria-hidden="true"></i>
    </div>

    <div>
      <h4>Document Information</h4>

      <p>
        Both curriculum vitae documents are provided
        in PDF format for convenient viewing and downloading.
        The Academic CV emphasizes research and academic
        experience, while the Detailed CV provides a
        broader professional overview.
      </p>
    </div>

  </footer>

</section>

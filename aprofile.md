---
layout: single
title: "Academic Profile"
permalink: /aprofile/
author_profile: true
---

<!-- Bootstrap 5 Grid -->
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
/* ==================================
   Academic Profile | Design System
================================== */

.academic-profile {
  --ap-primary: #173b68;
  --ap-accent: #2877c7;
  --ap-text: #24354a;
  --ap-muted: #62758a;
  --ap-border: #e1e8f0;
  --ap-surface: #ffffff;

  width: 100%;
  margin: 0 auto;
  color: var(--ap-text);
  font-family: inherit;
}

.academic-profile *,
.academic-profile *::before,
.academic-profile *::after {
  box-sizing: border-box;
}

/* Hero Section */

.ap-hero {
  position: relative;
  overflow: hidden;
  padding: 48px 30px;
  margin-bottom: 34px;
  border-radius: 18px;
  background: linear-gradient(
    135deg,
    #102d50 0%,
    #1c4f82 65%,
    #2877b7 100%
  );
  color: #ffffff;
  animation: ap-fade-up .7s ease both;
}

.ap-hero::after {
  content: "";
  position: absolute;
  width: 220px;
  height: 220px;
  right: -85px;
  top: -95px;
  border: 1px solid rgba(255,255,255,.18);
  border-radius: 50%;
  box-shadow:
    0 0 0 35px rgba(255,255,255,.035),
    0 0 0 75px rgba(255,255,255,.025);
  pointer-events: none;
}

.ap-eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 9px;
  font-size: .76rem;
  font-weight: 700;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: #b9ddff;
  margin-bottom: 13px;
}

.ap-hero h2 {
  font-size: clamp(1.7rem, 3.5vw, 2.4rem);
  font-weight: 750;
  line-height: 1.2;
  color: #ffffff;
  margin: 0 0 13px;
  border: 0;
}

.ap-hero p {
  max-width: 570px;
  margin: 0;
  font-size: .98rem;
  line-height: 1.8;
  color: #dfebf8;
}

/* Section Heading */

.ap-section {
  margin-bottom: 23px;
}

.ap-section h3 {
  font-size: 1.28rem;
  font-weight: 750;
  color: var(--ap-primary);
  margin: 0 0 8px;
  border: none;
}

.ap-section p {
  font-size: .94rem;
  line-height: 1.7;
  color: var(--ap-muted);
  margin: 0;
}

/* Profile Cards */

.ap-card {
  position: relative;
  display: flex;
  flex-direction: column;
  height: 100%;
  padding: 26px;
  overflow: hidden;
  background: var(--ap-surface);
  border: 1px solid var(--ap-border);
  border-radius: 16px;
  box-shadow: 0 4px 18px rgba(18,48,82,.035);
  transition:
    transform .32s cubic-bezier(.2,.8,.2,1),
    box-shadow .32s ease,
    border-color .32s ease;
}

.ap-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 3px;
  background: var(--card-accent);
  transform: scaleX(0);
  transform-origin: left;
  transition: transform .3s ease;
}

.ap-card:hover,
.ap-card:focus-within {
  transform: translateY(-6px);
  border-color: #c2d5e9;
  box-shadow: 0 15px 36px rgba(22,53,85,.12);
}

.ap-card:hover::before,
.ap-card:focus-within::before {
  transform: scaleX(1);
}

.ap-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 54px;
  height: 54px;
  margin-bottom: 21px;
  border-radius: 13px;
  font-size: 1.6rem;
  color: var(--card-accent);
  background: var(--card-bg);
  transition: transform .3s ease;
}

.ap-card:hover .ap-icon {
  transform: scale(1.07);
}

.ap-card h4 {
  margin: 0 0 9px;
  font-size: 1.18rem;
  font-weight: 750;
  color: var(--ap-primary);
}

.ap-card p {
  margin: 0 0 24px;
  flex-grow: 1;
  font-size: .91rem;
  line-height: 1.75;
  color: var(--ap-muted);
}

.ap-link {
  display: inline-flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  width: 100%;
  padding: 11px 15px;
  border: 1px solid #dce7f2;
  border-radius: 9px;
  color: var(--ap-primary) !important;
  background: #f7faff;
  text-decoration: none !important;
  font-size: .87rem;
  font-weight: 700;
  transition:
    background .25s ease,
    border-color .25s ease,
    color .25s ease;
}

.ap-link:hover {
  color: #ffffff !important;
  background: var(--ap-primary);
  border-color: var(--ap-primary);
}

.ap-link i {
  transition: transform .25s ease;
}

.ap-link:hover i {
  transform: translate(3px,-3px);
}

.ap-link:focus-visible {
  outline: 3px solid #73b6ff;
  outline-offset: 3px;
}

/* Platform Colors */

.ap-github {
  --card-accent: #303b4c;
  --card-bg: #edf0f3;
}

.ap-scholar {
  --card-accent: #4285f4;
  --card-bg: #edf4ff;
}

.ap-orcid {
  --card-accent: #83ad16;
  --card-bg: #f2f8e7;
}

.ap-linkedin {
  --card-accent: #0a66c2;
  --card-bg: #eaf4ff;
}

/* Footer */

.ap-footer {
  margin-top: 35px;
  padding: 22px 25px;
  display: flex;
  align-items: center;
  gap: 15px;
  border-radius: 12px;
  border: 1px solid #dfe8f1;
  background: #f7fafd;
}

.ap-footer-icon {
  flex-shrink: 0;
  font-size: 1.5rem;
  color: var(--ap-accent);
}

.ap-footer p {
  margin: 0;
  font-size: .87rem;
  line-height: 1.7;
  color: #536880;
}

/* Entrance Animations */

.ap-animate {
  animation: ap-fade-up .7s ease both;
}

.ap-delay-1 { animation-delay: .08s; }
.ap-delay-2 { animation-delay: .16s; }
.ap-delay-3 { animation-delay: .24s; }
.ap-delay-4 { animation-delay: .32s; }

@keyframes ap-fade-up {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Responsive Layout */

@media (max-width: 767px) {
  .ap-hero {
    padding: 34px 23px;
    border-radius: 14px;
  }

  .ap-card {
    padding: 22px;
  }

  .ap-footer {
    padding: 20px;
    align-items: flex-start;
  }
}

@media (prefers-reduced-motion: reduce) {
  .academic-profile *,
  .academic-profile *::before,
  .academic-profile *::after {
    animation: none !important;
    transition: none !important;
    scroll-behavior: auto !important;
  }
}
</style>

<section class="academic-profile" aria-label="Academic profiles">

  <!-- Hero -->

  <header class="ap-hero">
    <div class="ap-eyebrow">
      <i class="bi bi-mortarboard" aria-hidden="true"></i>
      Academic Network
    </div>

    <h2>Academic &amp; Professional Profiles</h2>

    <p>
      Explore my research presence, scholarly contributions,
      professional network, and open-source activities
      through the platforms below.
    </p>
  </header>

  <!-- Section Heading -->

  <div class="ap-section">
    <h3>Explore My Profiles</h3>
    <p>
      Connect with my academic research and professional work.
    </p>
  </div>

  <!-- Bootstrap Responsive Grid -->

  <div class="container-fluid px-0">
    <div class="row g-4">

      <!-- GitHub -->

      <div class="col-12 col-md-6">
        <article class="ap-card ap-github ap-animate ap-delay-1">

          <div class="ap-icon">
            <i class="bi bi-github" aria-hidden="true"></i>
          </div>

          <h4>GitHub</h4>

          <p>
            Explore research-related projects, repositories,
            technical implementations, and collaborative
            development activities.
          </p>

          <a
            class="ap-link"
            href="https://github.com/Abdurrazzakzubaer"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="Visit my GitHub profile (opens in a new tab)"
          >
            <span>View GitHub Profile</span>
            <i class="bi bi-arrow-up-right" aria-hidden="true"></i>
          </a>

        </article>
      </div>

      <!-- Google Scholar -->

      <div class="col-12 col-md-6">
        <article class="ap-card ap-scholar ap-animate ap-delay-2">

          <div class="ap-icon">
            <i class="bi bi-mortarboard-fill" aria-hidden="true"></i>
          </div>

          <h4>Google Scholar</h4>

          <p>
            Discover my academic publications, research
            contributions, citation information, and
            scholarly activities.
          </p>

          <a
            class="ap-link"
            href="https://scholar.google.com/citations?user=k_MgNaEAAAAJ&amp;hl=en"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="Visit my Google Scholar profile (opens in a new tab)"
          >
            <span>View Scholar Profile</span>
            <i class="bi bi-arrow-up-right" aria-hidden="true"></i>
          </a>

        </article>
      </div>

      <!-- ORCID -->

      <div class="col-12 col-md-6">
        <article class="ap-card ap-orcid ap-animate ap-delay-3">

          <div class="ap-icon">
            <i class="bi bi-person-vcard" aria-hidden="true"></i>
          </div>

          <h4>ORCID</h4>

          <p>
            Access my unique researcher identifier,
            academic affiliations, research outputs,
            and professional scholarly record.
          </p>

          <a
            class="ap-link"
            href="https://orcid.org/0009-0003-7472-3922"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="Visit my ORCID record (opens in a new tab)"
          >
            <span>View ORCID Record</span>
            <i class="bi bi-arrow-up-right" aria-hidden="true"></i>
          </a>

        </article>
      </div>

      <!-- LinkedIn -->

      <div class="col-12 col-md-6">
        <article class="ap-card ap-linkedin ap-animate ap-delay-4">

          <div class="ap-icon">
            <i class="bi bi-linkedin" aria-hidden="true"></i>
          </div>

          <h4>LinkedIn</h4>

          <p>
            Connect professionally and explore my
            academic background, teaching experience,
            research interests, and career activities.
          </p>

          <a
            class="ap-link"
            href="www.linkedin.com/in/abdur-razzak-zubaer-680a821a4"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="Open LinkedIn (opens in a new tab)"
          >
            <span>Connect on LinkedIn</span>
            <i class="bi bi-arrow-up-right" aria-hidden="true"></i>
          </a>

        </article>
      </div>

    </div>
  </div>

  <!-- Footer -->

  <footer class="ap-footer ap-animate ap-delay-4">

    <i
      class="bi bi-globe2 ap-footer-icon"
      aria-hidden="true"
    ></i>

    <p>
      These platforms provide access to my research,
      scholarly identity, academic collaborations,
      and professional activities.
    </p>

  </footer>

</section>

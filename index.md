---
layout: single
title: "Home"
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
/* ==========================================
   ABDUR RAZZAK ZUBAER
   Professional Academic Homepage
========================================== */

.arz-home {
  --primary: #173b68;
  --primary-dark: #102d50;
  --accent: #2877c7;
  --teal: #178c89;
  --text: #273a50;
  --muted: #62758a;
  --border: #e1e9f2;
  --soft: #f6f9fd;
  --white: #ffffff;

  width: 100%;
  color: var(--text);
  font-family: inherit;
}

.arz-home *,
.arz-home *::before,
.arz-home *::after {
  box-sizing: border-box;
}

/* HERO */

.arz-home .arz-hero {
  position: relative;
  overflow: hidden;
  padding: 48px 36px;
  margin-bottom: 34px;
  border-radius: 20px;

  background: linear-gradient(
    130deg,
    #102d50 0%,
    #194777 58%,
    #256b9e 100%
  );

  color: #fff;
  isolation: isolate;
}

.arz-home .arz-hero::before {
  content: "";
  position: absolute;
  width: 300px;
  height: 300px;
  right: -105px;
  top: -115px;
  border: 1px solid rgba(255,255,255,.18);
  border-radius: 50%;
  box-shadow:
    0 0 0 42px rgba(255,255,255,.04),
    0 0 0 85px rgba(255,255,255,.025);
  z-index: -1;
}

.arz-home .arz-eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  margin-bottom: 15px;
  color: #b9ddff;
  font-size: .76rem;
  font-weight: 700;
  letter-spacing: 1.35px;
  text-transform: uppercase;
}

.arz-home .arz-hero h2 {
  margin: 0 0 13px;
  padding: 0;
  border: 0;
  color: #fff;
  font-size: clamp(1.8rem, 3.5vw, 2.65rem);
  font-weight: 800;
  line-height: 1.2;
  letter-spacing: -.035em;
}

.arz-home .arz-hero-subtitle {
  max-width: 610px;
  margin: 0 0 18px;
  color: #e2effb;
  font-size: 1rem;
  font-weight: 500;
  line-height: 1.75;
}

.arz-home .arz-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin: 0 0 28px;
}

.arz-home .arz-tag {
  padding: 7px 12px;
  border: 1px solid rgba(255,255,255,.19);
  border-radius: 100px;
  background: rgba(255,255,255,.09);
  color: #e7f1fc;
  font-size: .74rem;
  font-weight: 600;
}

.arz-home .arz-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 11px;
}

.arz-home .arz-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 9px;
  min-height: 44px;
  padding: 11px 18px;
  border: 1px solid transparent;
  border-radius: 9px;
  font-size: .85rem;
  font-weight: 700;
  text-decoration: none !important;
  line-height: 1.3;
  transition:
    transform .28s ease,
    background-color .28s ease,
    border-color .28s ease,
    box-shadow .28s ease;
}

.arz-home .arz-btn-light {
  background: #fff;
  color: #173b68 !important;
}

.arz-home .arz-btn-light:hover {
  background: #e6f1fc;
  transform: translateY(-2px);
}

.arz-home .arz-btn-glass {
  border-color: rgba(255,255,255,.35);
  background: rgba(255,255,255,.09);
  color: #fff !important;
}

.arz-home .arz-btn-glass:hover {
  background: rgba(255,255,255,.18);
  transform: translateY(-2px);
}

/* SECTION TITLES */

.arz-home .arz-section {
  margin: 0 0 36px;
  scroll-margin-top: 85px;
}

.arz-home .arz-section-heading {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-bottom: 18px;
}

.arz-home .arz-section-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  width: 43px;
  height: 43px;
  border-radius: 11px;
  background: #eaf3ff;
  color: var(--accent);
  font-size: 1.2rem;
}

.arz-home .arz-section-heading h2 {
  margin: 0;
  padding: 0;
  border: 0;
  color: var(--primary-dark);
  font-size: 1.38rem;
  font-weight: 750;
}

/* SHARED CARDS */

.arz-home .arz-card {
  display: flex;
  flex-direction: column;
  height: 100%;
  min-width: 0;
  padding: 25px;
  border: 1px solid var(--border);
  border-radius: 15px;
  background: var(--white);
  box-shadow: 0 4px 18px rgba(20,48,82,.045);

  transition:
    transform .32s cubic-bezier(.2,.8,.2,1),
    box-shadow .32s ease,
    border-color .32s ease;
}

.arz-home .arz-card:hover {
  transform: translateY(-5px);
  border-color: #c7daec;
  box-shadow: 0 15px 30px rgba(20,48,82,.1);
}

.arz-home .arz-card h3 {
  margin: 0 0 10px;
  color: var(--primary);
  font-size: 1.06rem;
  font-weight: 750;
  line-height: 1.4;
}

.arz-home .arz-card p {
  margin: 0;
  color: var(--muted);
  font-size: .9rem;
  line-height: 1.8;
}

/* ABOUT */

.arz-home .arz-about {
  padding: 27px 30px;
  border: 1px solid var(--border);
  border-radius: 15px;
  background: var(--soft);
}

.arz-home .arz-about p {
  margin: 0;
  color: #455d76;
  font-size: .96rem;
  line-height: 1.95;
}

/* ACADEMIC QUALIFICATIONS */

.arz-home .arz-degree-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 48px;
  height: 48px;
  margin-bottom: 18px;
  border-radius: 12px;
  background: #eaf3ff;
  color: var(--accent);
  font-size: 1.4rem;
}

.arz-home .arz-degree-level {
  margin-bottom: 8px;
  color: var(--teal);
  font-size: .73rem;
  font-weight: 750;
  text-transform: uppercase;
  letter-spacing: .8px;
}

.arz-home .arz-status {
  align-self: flex-start;
  margin-top: 17px;
  padding: 5px 10px;
  border-radius: 30px;
  background: #e8f6f2;
  color: #197a67;
  font-size: .72rem;
  font-weight: 700;
}

/* EXPERIENCE */

.arz-home .arz-role {
  position: relative;
  padding-left: 17px;
  border-left: 3px solid #d9e8f7;
}

.arz-home .arz-role::before {
  content: "";
  position: absolute;
  top: 2px;
  left: -6px;
  width: 9px;
  height: 9px;
  border-radius: 50%;
  background: var(--accent);
}

.arz-home .arz-role h3 {
  margin: 0 0 6px;
  color: var(--primary-dark);
  font-size: .98rem;
  font-weight: 750;
}

.arz-home .arz-role p {
  margin: 0;
  color: var(--muted);
  font-size: .86rem;
  line-height: 1.6;
}

/* SKILLS */

.arz-home .arz-skill {
  display: flex;
  align-items: flex-start;
  gap: 12px;
  height: 100%;
  padding: 18px;
  border: 1px solid var(--border);
  border-radius: 12px;
  background: #fff;

  transition:
    transform .28s ease,
    border-color .28s ease,
    background-color .28s ease;
}

.arz-home .arz-skill:hover {
  transform: translateY(-3px);
  border-color: #bdd5ed;
  background: #f8fbff;
}

.arz-home .arz-skill i {
  flex-shrink: 0;
  margin-top: 2px;
  color: var(--accent);
  font-size: 1.25rem;
}

.arz-home .arz-skill strong {
  display: block;
  margin-bottom: 5px;
  color: var(--primary-dark);
  font-size: .88rem;
}

.arz-home .arz-skill span {
  display: block;
  color: var(--muted);
  font-size: .81rem;
  line-height: 1.6;
}

/* CONTACT */

.arz-home .arz-contact {
  padding: 29px;
  border: 1px solid var(--border);
  border-radius: 16px;
  background: linear-gradient(135deg, #f4f8fd, #fff);
}

.arz-home .arz-contact p {
  margin: 0 0 20px;
  color: var(--muted);
  font-size: .9rem;
  line-height: 1.7;
}

.arz-home .arz-email {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 13px 15px;
  margin-bottom: 10px;
  border: 1px solid #e2ebf5;
  border-radius: 10px;
  background: #fff;

  color: var(--primary) !important;
  text-decoration: none !important;
  font-size: .85rem;
  overflow-wrap: anywhere;

  transition:
    transform .28s ease,
    background-color .28s ease,
    border-color .28s ease;
}

.arz-home .arz-email:last-child {
  margin-bottom: 0;
}

.arz-home .arz-email:hover {
  transform: translateX(4px);
  background: #f3f8ff;
  border-color: #bfd7ee;
}

.arz-home .arz-email i {
  flex-shrink: 0;
  color: var(--accent);
  font-size: 1.15rem;
}

/* ANIMATIONS */

.arz-home .arz-fade {
  animation: arz-fade-up .7s ease both;
}

.arz-home .arz-delay-1 {
  animation-delay: .1s;
}

.arz-home .arz-delay-2 {
  animation-delay: .2s;
}

.arz-home .arz-delay-3 {
  animation-delay: .3s;
}

.arz-home .arz-delay-4 {
  animation-delay: .4s;
}

@keyframes arz-fade-up {
  from {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* ACCESSIBILITY */

.arz-home a:focus-visible {
  outline: 3px solid #7bb9fa;
  outline-offset: 3px;
}

/* MOBILE */

@media (max-width: 767px) {
  .arz-home .arz-hero {
    padding: 35px 23px;
    border-radius: 15px;
  }

  .arz-home .arz-card {
    padding: 21px;
  }

  .arz-home .arz-about,
  .arz-home .arz-contact {
    padding: 22px;
  }

  .arz-home .arz-actions {
    flex-direction: column;
  }

  .arz-home .arz-btn {
    width: 100%;
  }

  .arz-home .arz-section-heading h2 {
    font-size: 1.22rem;
  }

  .arz-home .arz-email {
    font-size: .78rem;
  }
}

@media (prefers-reduced-motion: reduce) {
  .arz-home *,
  .arz-home *::before,
  .arz-home *::after {
    animation: none !important;
    transition: none !important;
  }
}
</style>

<div class="arz-home">

  <!-- =========================
       HERO
  ========================== -->

  <header class="arz-hero arz-fade">

    <div class="arz-eyebrow">
      <i class="bi bi-mortarboard"
         aria-hidden="true"></i>
      Academic &amp; Professional Portfolio
    </div>

    <h2>Abdur Razzak Zubaer</h2>

    <p class="arz-hero-subtitle">
      Lecturer in Civil &amp; Environmental Engineering
      <br>
      Academic Researcher | Individual Consultant
    </p>

    <div class="arz-tags">
      <span class="arz-tag">Environmental Engineering</span>
      <span class="arz-tag">Academic Research</span>
      <span class="arz-tag">Statistical Modeling</span>
      <span class="arz-tag">GIS</span>
    </div>

    <div class="arz-actions">

      <a href="{{ '/cv/' | relative_url }}"
         class="arz-btn arz-btn-light">
        <i class="bi bi-file-earmark-person"
           aria-hidden="true"></i>
        View Curriculum Vitae
      </a>

      <a href="#contact"
         class="arz-btn arz-btn-glass">
        <i class="bi bi-envelope"
           aria-hidden="true"></i>
        Contact Me
      </a>

    </div>

  </header>

  <!-- =========================
       ABOUT
  ========================== -->

  <section id="about"
           class="arz-section arz-fade arz-delay-1">

    <div class="arz-section-heading">
      <div class="arz-section-icon">
        <i class="bi bi-person-lines-fill"
           aria-hidden="true"></i>
      </div>
      <h2>About Me</h2>
    </div>

    <div class="arz-about">

      <p>
        My academic background combines civil engineering,
        environmental science and management, and ongoing
        postgraduate study in environmental engineering.
        My professional experience includes university teaching,
        environmental engineering consultancy, and research
        activities.
      </p>

    </div>

  </section>

  <!-- =========================
       ACADEMIC QUALIFICATIONS
  ========================== -->

  <section id="education"
           class="arz-section arz-fade arz-delay-2">

    <div class="arz-section-heading">
      <div class="arz-section-icon">
        <i class="bi bi-mortarboard-fill"
           aria-hidden="true"></i>
      </div>
      <h2>Academic Qualifications</h2>
    </div>

    <div class="container-fluid px-0">
      <div class="row g-3">

        <!-- BUET -->

        <div class="col-12 col-md-6">
          <article class="arz-card">

            <div class="arz-degree-icon">
              <i class="bi bi-book"
                 aria-hidden="true"></i>
            </div>

            <div class="arz-degree-level">
              Postgraduate Studies
            </div>

            <h3>MSc in Environmental Engineering</h3>

            <p>
              Bangladesh University of Engineering
              and Technology (BUET)
            </p>

            <span class="arz-status">Ongoing</span>

          </article>
        </div>

        <!-- BUP -->

        <div class="col-12 col-md-6">
          <article class="arz-card">

            <div class="arz-degree-icon">
              <i class="bi bi-mortarboard"
                 aria-hidden="true"></i>
            </div>

            <div class="arz-degree-level">
              Master's Degree
            </div>

            <h3>MSc in Environmental Science and Management</h3>

            <p>
              Bangladesh University of Professionals (BUP)
            </p>

          </article>
        </div>

        <!-- AUST -->

        <div class="col-12">
          <article class="arz-card">

            <div class="arz-degree-icon">
              <i class="bi bi-buildings"
                 aria-hidden="true"></i>
            </div>

            <div class="arz-degree-level">
              Undergraduate Degree
            </div>

            <h3>BSc in Civil Engineering</h3>

            <p>
              Ahsanullah University of Science and
              Technology (AUST)
            </p>

          </article>
        </div>

      </div>
    </div>

  </section>

  <!-- =========================
       PROFESSIONAL EXPERIENCE
  ========================== -->

  <section id="experience"
           class="arz-section arz-fade arz-delay-2">

    <div class="arz-section-heading">
      <div class="arz-section-icon">
        <i class="bi bi-briefcase-fill"
           aria-hidden="true"></i>
      </div>
      <h2>Professional Experience</h2>
    </div>

    <div class="container-fluid px-0">
      <div class="row g-3">

        <div class="col-12 col-md-6">
          <div class="arz-card">
            <div class="arz-role">
              <h3>Lecturer</h3>
              <p>World University of Bangladesh</p>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6">
          <div class="arz-card">
            <div class="arz-role">
              <h3>Environmental Engineer</h3>
              <p>
                Environment and Resource Analysis
                Center (ENRAC)
              </p>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6">
          <div class="arz-card">
            <div class="arz-role">
              <h3>
                Junior Environmental Engineer
                and Graduate Engineer
              </h3>
              <p>ACE Consultants Limited</p>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6">
          <div class="arz-card">
            <div class="arz-role">
              <h3>Assistant Environmental Engineer</h3>
              <p>Eagle Fibre Industries Ltd.</p>
            </div>
          </div>
        </div>

        <div class="col-12">
          <div class="arz-card">
            <div class="arz-role">
              <h3>Research Assistant</h3>
              <p>
                Ahsanullah University of Science
                and Technology
              </p>
            </div>
          </div>
        </div>

      </div>
    </div>

  </section>

  <!-- =========================
       TECHNICAL SKILLS
  ========================== -->

  <section id="skills"
           class="arz-section arz-fade arz-delay-3">

    <div class="arz-section-heading">
      <div class="arz-section-icon">
        <i class="bi bi-tools"
           aria-hidden="true"></i>
      </div>
      <h2>Technical Skills</h2>
    </div>

    <div class="container-fluid px-0">
      <div class="row g-3">

        <div class="col-12 col-md-6">
          <div class="arz-skill">
            <i class="bi bi-globe-asia-australia"
               aria-hidden="true"></i>
            <div>
              <strong>Geographic Information Systems</strong>
              <span>ArcGIS, QGIS</span>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6">
          <div class="arz-skill">
            <i class="bi bi-graph-up-arrow"
               aria-hidden="true"></i>
            <div>
              <strong>Modeling</strong>
              <span>
                Statistical Modeling (Prediction Model)
              </span>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6">
          <div class="arz-skill">
            <i class="bi bi-rulers"
               aria-hidden="true"></i>
            <div>
              <strong>Drafting</strong>
              <span>AutoCAD</span>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6">
          <div class="arz-skill">
            <i class="bi bi-bar-chart-line"
               aria-hidden="true"></i>
            <div>
              <strong>Design &amp; Analysis</strong>
              <span>ETABS, JASP, SPSS</span>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6">
          <div class="arz-skill">
            <i class="bi bi-code-slash"
               aria-hidden="true"></i>
            <div>
              <strong>Programming</strong>
              <span>Python, C</span>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6">
          <div class="arz-skill">
            <i class="bi bi-laptop"
               aria-hidden="true"></i>
            <div>
              <strong>Productivity</strong>
              <span>Microsoft 365</span>
            </div>
          </div>
        </div>

      </div>
    </div>

  </section>

  <!-- =========================
       CONTACT
  ========================== -->

  <section id="contact"
           class="arz-section arz-fade arz-delay-4">

    <div class="arz-section-heading">
      <div class="arz-section-icon">
        <i class="bi bi-envelope-fill"
           aria-hidden="true"></i>
      </div>
      <h2>Contact</h2>
    </div>

    <div class="arz-contact">

      <p>
        For academic correspondence, research discussions,
        or professional inquiries, please use one of the
        email addresses below.
      </p>

      <a class="arz-email"
         href="mailto:abdur.razzak@civil.wub.edu.bd">
        <i class="bi bi-envelope"
           aria-hidden="true"></i>
        <span>abdur.razzak@civil.wub.edu.bd</span>
      </a>

      <a class="arz-email"
         href="mailto:zubaer.bup@gmail.com">
        <i class="bi bi-envelope"
           aria-hidden="true"></i>
        <span>zubaer.bup@gmail.com</span>
      </a>

      <a class="arz-email"
         href="mailto:0426042502@Ce.buet.ac.bd">
        <i class="bi bi-envelope"
           aria-hidden="true"></i>
        <span>0426042502@Ce.buet.ac.bd</span>
      </a>

    </div>

  </section>

</div>

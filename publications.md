---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
---
<!-- Bootstrap grid and Bootstrap Icons; remove if already loaded globally -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap-grid.min.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
<style>
/* Scoped to this page. Content always remains visible. */
.arz-pubs{--navy:#102d50;--blue:#2877c7;--teal:#168b89;--muted:#596d81;--line:#dfe8f1;--soft:#f6f9fd;color:#263b52;width:100%}
.arz-pubs *, .arz-pubs *::before, .arz-pubs *::after{box-sizing:border-box}
.arz-pubs .pub-hero{padding:clamp(26px,5vw,44px);border-radius:18px;background:linear-gradient(125deg,#102d50,#1a487b 70%,#2877a8);color:#fff;margin:0 0 24px}
.arz-pubs .pub-kicker{font-size:.75rem;letter-spacing:.09em;font-weight:700;text-transform:uppercase;color:#b9ddff;margin:0 0 12px}
.arz-pubs .pub-hero h1{margin:0 0 12px;padding:0;border:0;color:#fff;font-size:clamp(1.7rem,4vw,2.55rem);line-height:1.2}
.arz-pubs .pub-hero p{margin:0;max-width:680px;color:#e5effa;line-height:1.75;font-size:.95rem}
.arz-pubs .pub-stats{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:12px;margin:0 0 34px}
.arz-pubs .pub-stat{padding:16px;background:var(--soft);border:1px solid var(--line);border-radius:12px}
.arz-pubs .pub-stat strong{display:block;font-size:1.5rem;color:var(--navy);line-height:1.2}
.arz-pubs .pub-stat span{font-size:.79rem;color:var(--muted)}
.arz-pubs .pub-section{margin:0 0 34px}
.arz-pubs .pub-section-heading{display:flex;align-items:center;gap:12px;margin:0 0 18px}
.arz-pubs .pub-section-heading i{display:grid;place-items:center;flex:none;width:43px;height:43px;border-radius:11px;background:#eaf3ff;color:var(--blue);font-size:1.2rem}
.arz-pubs .pub-section-heading h2{font-size:1.35rem;color:var(--navy);border:0;padding:0;margin:0}
/* Native grid fallback works even when Bootstrap CDN is unavailable */
.arz-pubs .pub-grid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:18px;margin:0}
.arz-pubs .pub-grid>[class*="col-"]{padding:0;width:auto;max-width:none;flex:none}
.arz-pubs .pub-card{height:100%;display:flex;flex-direction:column;min-width:0;background:#fff;border:1px solid var(--line);border-top:3px solid var(--blue);border-radius:14px;padding:23px;box-shadow:0 4px 17px rgba(17,48,81,.045);animation:pub-enter .55s ease-out both;transition:transform .25s ease,box-shadow .25s ease,border-color .25s ease}
.arz-pubs .pub-card:hover{transform:translateY(-4px);box-shadow:0 13px 30px rgba(17,48,81,.10);border-color:#bad3e8}
.arz-pubs .pub-conference .pub-card{border-top-color:var(--teal)}
.arz-pubs .pub-card-top{display:flex;justify-content:space-between;gap:12px;align-items:center;margin-bottom:15px}
.arz-pubs .pub-num{display:inline-flex;align-items:center;justify-content:center;width:40px;height:36px;border-radius:9px;background:#eaf3ff;color:#173b68;font-weight:750;font-size:.86rem}
.arz-pubs .pub-conference .pub-num{background:#e8f6f2;color:#147e72}
.arz-pubs .pub-year{font-size:.8rem;color:var(--muted);font-weight:700}
.arz-pubs .pub-card h3{font-size:1.06rem;line-height:1.52;color:var(--navy);margin:0 0 14px;padding:0;border:0;overflow-wrap:anywhere}
.arz-pubs .pub-venue{font-size:.89rem;color:#536b82;line-height:1.65;margin:0 0 12px}
.arz-pubs .pub-location{font-size:.84rem;color:var(--muted);line-height:1.6;margin:0 0 14px}
.arz-pubs .pub-actions{margin-top:auto;padding-top:10px}
.arz-pubs .pub-link{display:inline-flex;align-items:center;gap:8px;font-size:.84rem;font-weight:700;color:#145b9b;text-decoration:none;border-bottom:1px solid transparent;overflow-wrap:anywhere}
.arz-pubs .pub-link:hover{color:#103d70;border-color:currentColor}
.arz-pubs .pub-link:focus-visible{outline:3px solid #80bcf2;outline-offset:4px}
.arz-pubs .pub-note{padding:18px 20px;background:var(--soft);border:1px solid var(--line);border-radius:12px;color:var(--muted);font-size:.85rem;line-height:1.75}
@keyframes pub-enter{from{transform:translateY(7px)}to{transform:translateY(0)}}
@media(max-width:800px){.arz-pubs .pub-grid{grid-template-columns:1fr}}
@media(max-width:480px){.arz-pubs .pub-stats{gap:8px}.arz-pubs .pub-stat{padding:12px 9px}.arz-pubs .pub-stat strong{font-size:1.3rem}.arz-pubs .pub-stat span{font-size:.7rem}.arz-pubs .pub-card{padding:19px}.arz-pubs .pub-hero{border-radius:13px}}
@media(prefers-reduced-motion:reduce){.arz-pubs .pub-card{animation:none;transition:none}}
<div class="arz-pubs">
  <header class="pub-hero">
    <p class="pub-kicker"><i class="bi bi-journal-richtext" aria-hidden="true"></i> Academic &amp; Research Portfolio</p>
    <h1>Publications</h1>
    <p>Journal articles, research outputs, and conference proceedings covering civil engineering, environmental engineering, water and sanitation, structural engineering, and transportation.</p>
  </header>
<div class="pub-stats" aria-label="Publication summary">
    <div class="pub-stat"><strong>16</strong><span>Total listed works</span></div>
    <div class="pub-stat"><strong>11</strong><span>Articles &amp; research outputs</span></div>
    <div class="pub-stat"><strong>5</strong><span>Conference proceedings</span></div>
  </div>
<section class="pub-section" aria-labelledby="journals-title">
    <div class="pub-section-heading"><i class="bi bi-journal-text" aria-hidden="true"></i><h2 id="journals-title">Journal Articles &amp; Research Outputs</h2></div>
    <div class="row g-4 pub-grid">
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">01</span><span class="pub-year">2021</span></div>
          <h3>A comparison between inclined shear reinforcement and loop shear reinforcement on RC beam: Finite Element Analysis</h3>
          <p class="pub-venue"><em>Malaysian Journal of Civil Engineering, 33(3)</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.11113/mjce.v33.17307" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 1"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">02</span><span class="pub-year">2022</span></div>
          <h3>Feasibility Study on Concrete Dust as A Substitute of Filling Sand for Road Construction</h3>
          <p class="pub-venue"><em>Journal of Advances in Geotechnical Engineering, 4(3)</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.5281/zenodo.5792993" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 2"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">03</span><span class="pub-year">2022</span></div>
          <h3>An Overview of the foot over-bridge at Dhaka City</h3>
          <p class="pub-venue"><em>Journal of Advances in Civil Engineering and Management, 5(1)</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.5281/zenodo.6087177" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 3"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">04</span><span class="pub-year">2022</span></div>
          <h3>Reliability Analysis of Rooftop Rainwater Harvesting Using Daily Water Balance for an Educational Institute</h3>
          <p class="pub-venue"><em>Journal of Engineering Analysis and Design, 4(1)</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.5281/zenodo.6086805" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 4"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">05</span><span class="pub-year">2023</span></div>
          <h3>Evaluation of Bangladesh&#x27;s SDG6 achievement: A review</h3>
          <p class="pub-venue"><em>Journal of Environmental Engineering and its Scope, 6(1)</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.5281/zenodo.7627649" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 5"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">06</span><span class="pub-year">2023</span></div>
          <h3>An Analysis of the Quality of Dhaka&#x27;s Potable Water and Sanitation Services</h3>
          <p class="pub-venue"><em>Journal of Environmental Issues and Climate Change, 2(1)</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.59110/jeicc.v2i1.134" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 6"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">07</span><span class="pub-year">2023</span></div>
          <h3>A Comparison of Long-Term Meteorological Data of Khulna and Dhaka to Comprehend Climate Change Impacts</h3>
          <p class="pub-venue"><em>Journal of Environmental Engineering and its Scope, 6(2)</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.5281/zenodo.8131076" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 7"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">08</span><span class="pub-year">2024</span></div>
          <h3>Structural behavior of CFRP wrapped circular hollow bridge piers under cyclic loading considering local buckling limit state</h3>
          <p class="pub-venue"><em>Asian Journal of Civil Engineering</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.1007/s42107-024-00993-2" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 8"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">09</span><span class="pub-year">2024</span></div>
          <h3>Impact of Code Changes on The Design of RC Frame Structure</h3>
          <p class="pub-venue"><em>Research output (venue not specified)</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.21203/rs.3.rs-4404310/v1" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 9"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">10</span><span class="pub-year">2024</span></div>
          <h3>Performance Analysis of Coir Fibered Soft Clay</h3>
          <p class="pub-venue"><em>Journal of Earthquake Science and Soil Dynamics Engineering, 7(3)</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.5281/zenodo.13883657" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 10"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">11</span><span class="pub-year">2024</span></div>
          <h3>Performance Analysis of Soft Clay with Rice Husk Ash &amp; Polypropylene Fibered</h3>
          <p class="pub-venue"><em>Journal of Earthquake Science and Soil Dynamics Engineering, 7(3)</em></p>
          <div class="pub-actions"><a class="pub-link" href="https://doi.org/10.5281/zenodo.13883638" target="_blank" rel="noopener noreferrer" aria-label="Open DOI for publication 11"><i class="bi bi-box-arrow-up-right" aria-hidden="true"></i> View publication / DOI</a></div>
        </article>
      </div>
    </div>
  </section>
<section class="pub-section pub-conference" aria-labelledby="conference-title">
    <div class="pub-section-heading"><i class="bi bi-people" aria-hidden="true"></i><h2 id="conference-title">Conference Proceedings</h2></div>
    <div class="row g-4 pub-grid">
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">01</span><span class="pub-year">2023</span></div>
          <h3>Short-term and Long-term Aging Performance of Styrene Butadiene Styrene (SBS) Modified Asphalt Binder</h3>
          <p class="pub-venue"><em>Proceedings of the Second International Conference on Advances in Civil Infrastructure and Construction Materials</em></p>
          <p class="pub-location"><i class="bi bi-geo-alt" aria-hidden="true"></i> Dhaka, Bangladesh</p>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">02</span><span class="pub-year">2023</span></div>
          <h3>Life Cycle Assessment of Rigid and Flexible Pavements: A Review in Bangladesh Perspective</h3>
          <p class="pub-venue"><em>Proceedings of the Second International Conference on Advances in Civil Infrastructure and Construction Materials</em></p>
          <p class="pub-location"><i class="bi bi-geo-alt" aria-hidden="true"></i> Dhaka, Bangladesh</p>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">03</span><span class="pub-year">2024</span></div>
          <h3>A Critical Analysis and Investigative Assessment of The Influence of Ride-Sharing Services on The Transportation System in Dhaka</h3>
          <p class="pub-venue"><em>Proceedings of the 7th International Conference on Civil Engineering for Sustainable Development (ICCESD 2024)</em></p>
          <p class="pub-location"><i class="bi bi-geo-alt" aria-hidden="true"></i> 7–9 February 2024 · KUET, Khulna, Bangladesh</p>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">04</span><span class="pub-year">2024</span></div>
          <h3>A Case Study on Land Use and Land Cover Changes in Specific Areas in Chattogram City Corporation</h3>
          <p class="pub-venue"><em>Proceedings of the 7th International Conference on Civil Engineering for Sustainable Development (ICCESD 2024)</em></p>
          <p class="pub-location"><i class="bi bi-geo-alt" aria-hidden="true"></i> 7–9 February 2024 · KUET, Khulna, Bangladesh</p>
        </article>
      </div>
      <div class="col-12 col-lg-6">
        <article class="pub-card">
          <div class="pub-card-top"><span class="pub-num">05</span><span class="pub-year">2024</span></div>
          <h3>A Systematic Review on High and Low-Temperature Performance of Nanomodified Asphalt Binder Considering Short and Long-Term Aging</h3>
          <p class="pub-venue"><em>Proceedings of the 7th International Conference on Civil Engineering for Sustainable Development (ICCESD 2024)</em></p>
          <p class="pub-location"><i class="bi bi-geo-alt" aria-hidden="true"></i> 7–9 February 2024 · KUET, Khulna, Bangladesh</p>
        </article>
      </div>
    </div>
  </section>
  <footer class="pub-note">Publication titles and bibliographic details are reproduced from the supplied CV list. The entry “Impact of Code Changes on The Design of RC Frame Structure” is described as a research output because a journal venue was not supplied.</footer>
</div>

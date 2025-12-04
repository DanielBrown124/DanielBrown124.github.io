---
layout: none
title: Quantum–Kinetic Dark Energy (QKDE)
---

<!-- MathJax -->
<script>
  window.MathJax = { tex: { inlineMath: [['$','$'], ['\\(','\\)']] } };
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<style>
  [id] {
  scroll-margin-top: 90px;
}
 /* ===========================
   CALCULATOR LAYOUT
   =========================== */

.calc-section {
  margin-top: 8px;
}

.calc-intro {
  font-size: 0.93rem;
  opacity: 0.9;
  margin-bottom: 16px;
}

.calc-header-row {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 8px 14px;
  justify-content: space-between;
  margin-bottom: 6px;
}

.calc-header-row h3 {
  margin: 0;
  font-size: 1rem;
  color: #d6f7ff;
  letter-spacing: 0.03em;
  text-transform: uppercase;
}

/* Small pills for presets / mode indicators */
.calc-pill-row {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
}

.calc-pill {
  font-size: 0.72rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  padding: 3px 9px;
  border-radius: 999px;
  border: 1px solid rgba(160, 220, 255, 0.5);
  background: rgba(6, 12, 20, 0.95);
  color: #c8efff;
  cursor: pointer;
  transition: background 0.18s ease, color 0.18s ease, box-shadow 0.18s ease;
  white-space: nowrap;
}

.calc-pill:hover {
  background: rgba(65, 190, 220, 0.2);
  box-shadow: 0 0 8px rgba(102,252,241,0.35);
}

.calc-pill.is-active {
  background: linear-gradient(135deg, #66fcf1, #45b9d9);
  color: #031016;
  box-shadow: 0 0 10px rgba(102,252,241,0.7);
  border-color: rgba(200,240,255,0.9);
}

/* ===========================
   CALCULATOR GRID & CARDS
   =========================== */

.calc-grid {
  margin-top: 14px;
  display: flex;
  flex-wrap: wrap;
  gap: 22px;
  justify-content: center;
}

.calc-card {
  flex: 1 1 320px;
  max-width: 430px;
  background: radial-gradient(circle at 0% 0%, rgba(102,252,241,0.12) 0, transparent 55%),
              radial-gradient(circle at 120% 120%, rgba(102,252,241,0.10) 0, transparent 55%),
              rgba(12, 18, 28, 0.82);
  padding: 20px 22px 22px;
  border-radius: 16px;
  border: 1px solid rgba(102,252,241,0.14);
  box-shadow:
    0 0 22px rgba(102,252,241,0.12),
    inset 0 0 18px rgba(102,252,241,0.06);
  backdrop-filter: blur(7px);
  position: relative;
  overflow: hidden;
  transition: transform 0.22s ease, box-shadow 0.22s ease, border-color 0.22s ease;
}

/* subtle top accent line */
.calc-card::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 3px;
  width: 100%;
  background: linear-gradient(
    to right,
    rgba(102,252,241,0.85),
    rgba(69,160,201,0.55),
    rgba(102,252,241,0.85)
  );
  opacity: 0.9;
  pointer-events: none;
}

.calc-card:hover {
  transform: translateY(-3px);
  border-color: rgba(102,252,241,0.26);
  box-shadow:
    0 0 26px rgba(102,252,241,0.24),
    inset 0 0 22px rgba(102,252,241,0.10);
}

/* ===========================
   CARD BODY
   =========================== */

.calc-card h4 {
  margin: 4px 0 4px;
  font-size: 1.08rem;
  color: #c9f6ff;
  font-weight: 400;
}

.calc-note {
  font-size: 0.83rem;
  opacity: 0.85;
  margin-top: 2px;
  margin-bottom: 10px;
  color: #e3f6ff;
  line-height: 1.5;
}

.calc-label {
  display: block;
  font-size: 0.82rem;
  margin-top: 9px;
  margin-bottom: 3px;
  color: #d6faff;
  letter-spacing: 0.04em;
  text-transform: uppercase;
}

.calc-input-row {
  display: grid;
  grid-template-columns: 1.15fr 0.85fr;
  gap: 8px 10px;
}

@media (max-width: 540px) {
  .calc-input-row {
    grid-template-columns: 1fr;
  }
}

/* ===========================
   INPUTS & BUTTONS
   =========================== */

.calc-input {
  width: 100%;
  padding: 7px 10px;
  border-radius: 7px;
  border: 1px solid rgba(120,160,190,0.7);
  background: rgba(5, 10, 18, 0.9);
  color: #f0f7ff;
  font-size: 0.9rem;
  box-sizing: border-box;
  transition: border-color 0.22s ease, box-shadow 0.22s ease, background 0.22s ease;
}

.calc-input::placeholder {
  color: rgba(200,225,250,0.4);
}

.calc-input:hover {
  border-color: rgba(102,252,241,0.45);
}

.calc-input:focus {
  outline: none;
  border-color: rgba(102,252,241,0.9);
  background: rgba(8, 14, 22, 0.98);
  box-shadow: 0 0 12px rgba(102,252,241,0.65);
}

.calc-action-row {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 14px;
}

.calc-btn {
  padding: 8px 16px;
  border-radius: 999px;
  border: 1px solid rgba(200,240,255,0.8);
  background: linear-gradient(135deg, #d2f2ff, #bfe6f7);
  color: #031016;
  font-size: 0.86rem;
  font-weight: 500;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  cursor: pointer;
  transition: transform 0.16s ease, box-shadow 0.16s ease, background 0.16s ease;
}

.calc-btn:hover {
  transform: translateY(-1px);
  background: linear-gradient(135deg, #e6f6ff, #d7f0ff);
  box-shadow: 0 0 12px rgba(210,240,255,0.75);
}

.calc-btn.secondary {
  background: transparent;
  color: #c8f3ff;
  border-color: rgba(140,200,255,0.7);
}

.calc-btn.secondary:hover {
  background: rgba(10,20,32,0.9);
  box-shadow: 0 0 10px rgba(102,252,241,0.45);
}

/* ===========================
   OUTPUT & ERROR STATES
   =========================== */

.calc-output {
  margin-top: 14px;
  font-family: "JetBrains Mono","Menlo","Consolas",monospace;
  font-size: 0.8rem;
  line-height: 1.45;
  background: rgba(0, 0, 0, 0.55);
  border-radius: 10px;
  padding: 11px 13px;
  border: 1px solid rgba(120,160,190,0.36);
  max-height: 210px;
  overflow-y: auto;
  overflow-x: hidden;
  white-space: pre-wrap;
  color: #e9faff;
  opacity: 0.96;
  transition: box-shadow 0.22s ease;
}

.calc-output:hover {
  box-shadow: 0 0 14px rgba(102,252,241,0.25);
}

.calc-output.error {
  border-color: rgba(255,140,140,0.75);
  background: rgba(60, 5, 10, 0.75);
  color: #ffe6e6;
}

/* ===========================
   FORMULA BOX
   =========================== */

.calc-formula-box {
  margin-top: 12px;
  padding: 10px 12px;
  border-radius: 9px;
  background: rgba(5, 10, 18, 0.9);
  border: 1px solid rgba(120,160,190,0.5);
  font-size: 0.86rem;
  color: #e0f4ff;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.3s ease, padding-top 0.3s ease, padding-bottom 0.3s ease;
}

/* when visible, we add a helper class in JS */
.calc-formula-box.is-open {
  max-height: 260px;
  padding-top: 10px;
  padding-bottom: 10px;
}

/* Let long equations scroll horizontally if needed */
.calc-formula-inner {
  overflow-x: auto;
  padding-bottom: 4px;
}

.calc-formula-inner p {
  margin: 4px 0;
}

/* ===========================
   FOOTNOTE
   =========================== */

.calc-footnote {
  margin-top: 18px;
  font-size: 0.9rem;
  opacity: 0.9;
}

/* ===========================
   RESPONSIVENESS
   =========================== */

@media (max-width: 780px) {
  .calc-grid {
    gap: 18px;
  }
  .calc-card {
    padding: 18px 18px 20px;
  }
}
  html {
  scroll-behavior: smooth;
}
.nav-header {
  position: sticky;
  top: 0;
  z-index: 1000;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  justify-content: center;
  padding: 12px 18px;
  margin: -30px -30px 25px;
  background: linear-gradient(
    to right,
    rgba(5, 10, 20, 0.94),
    rgba(8, 15, 28, 0.94)
  );
  border-bottom: 1px solid rgba(102,252,241,0.18);
  box-shadow: 0 4px 18px rgba(0,0,0,0.55);
  backdrop-filter: blur(10px);
  border-top-left-radius: 14px;
  border-top-right-radius: 14px;
}

.nav-header a {
  font-size: 0.9rem;
  letter-spacing: 0.03em;
  text-transform: uppercase;
  text-decoration: none;
  color: #c8eaff;
  padding: 6px 10px;
  border-radius: 999px;
  border: 1px solid transparent;
  transition: 0.18s ease;
}

.nav-header a:hover {
  border-color: rgba(102,252,241,0.6);
  background: rgba(102,252,241,0.09);
  color: #ffffff;
  text-shadow: 0 0 6px rgba(102,252,241,0.9);
}
.nav-header .nav-button {
  padding: 6px 14px;
  margin-left: 10px;
  background: linear-gradient(135deg, #66fcf1, #45c9c9);
  color: #0a0f12;
  font-weight: 600;
  font-size: 0.83rem;
  border-radius: 14px;
  text-decoration: none;
  border: 1px solid rgba(255,255,255,0.15);
  box-shadow: 0 0 6px rgba(102,252,241,0.35);
  transition: all 0.25s ease;
  display: inline-block;
  white-space: nowrap;
}

.nav-header .nav-button:hover {
  background: linear-gradient(135deg, #8afef4, #5edbd8);
  transform: translateY(-1px);
  box-shadow: 0 0 10px rgba(102,252,241,0.5);
  color: #000;
}
.alt-button {
  background: #fff0b3;
  color: #0b0c10;
}

.alt-button:hover {
  background: #ffe680;
  box-shadow: 0 0 14px rgba(255, 230, 128, 0.8);
}
  .cite-box {
  margin-top: 40px;
  background: rgba(15, 22, 32, 0.55);
  border: 1px solid rgba(102, 252, 241, 0.12);
  border-radius: 12px;
  padding: 20px 25px;
  box-shadow: 0 0 20px rgba(102,252,241,0.12);
}

.cite-box h3 {
  color: #b9ecff;
  font-family: "Merriweather", serif;
  font-weight: 300;
  margin-top: 0;
}

.cite-text {
  font-family: "Menlo", "Consolas", monospace;
  font-size: 0.85rem;
  color: #e8e9ef;
  background: rgba(0, 0, 0, 0.35);
  padding: 12px 14px;
  border-radius: 8px;
  overflow-x: auto;
}
  .cite-label {
  display: block;
  margin-bottom: 6px;
  font-size: 0.95rem;
  color: #c5f2ff;
  font-family: "Merriweather", serif;
}

.cite-select {
  background: rgba(20, 30, 45, 0.7);
  color: #e8e9ef;
  padding: 6px 10px;
  border-radius: 6px;
  border: 1px solid rgba(102,252,241,0.20);
  margin-bottom: 14px;
  font-size: 0.95rem;
}
/* ===== Enhanced Cite Box Styling ===== */

.enhanced-cite {
  margin-top: 55px;
  padding: 28px 28px 32px;
  background: linear-gradient(
      to bottom right,
      rgba(15, 22, 32, 0.7),
      rgba(12, 18, 28, 0.55)
    );
  border-radius: 14px;
  border: 1px solid rgba(102,252,241,0.18);
  box-shadow: 0 0 25px rgba(102,252,241,0.15);
  position: relative;
}

.enhanced-cite::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 3px;
  width: 100%;
  background: linear-gradient(to right, #66fcf1, #45a0c9, #66fcf1);
  border-top-left-radius: 14px;
  border-top-right-radius: 14px;
  opacity: 0.8;
}

.cite-header h3 {
  margin-bottom: 4px;
  font-size: 1.45rem;
}

.cite-subtext {
  color: #c9e6f8;
  font-size: 0.9rem;
  opacity: 0.8;
  margin-top: 0;
}

/* Citation Text Block */
.cite-text {
  font-family: "JetBrains Mono", "Menlo", "Consolas", monospace;
  background: rgba(0, 0, 0, 0.45);
  border: 1px solid rgba(120,160,200,0.25);
  padding: 14px 16px;
  border-radius: 8px;
  color: #e8e9ef;
  font-size: 0.88rem;
  max-height: 220px;
  overflow-y: auto;
  transition: max-height 0.3s ease;
}

/* Buttons container */
.cite-buttons {
  margin-top: 14px;
  display: flex;
  gap: 14px;
}

/* Second button style */
.alt-cite-btn {
  background: #c8f5ff;
}

.alt-cite-btn:hover {
  background: #aee8f7;
}

/* Toast Notification */
.toast {
  position: fixed;
  bottom: 28px;
  right: 28px;
  background: rgba(20, 160, 200, 0.9);
  padding: 12px 18px;
  color: white;
  border-radius: 8px;
  font-size: 0.9rem;
  opacity: 0;
  transform: translateY(20px);
  transition: all 0.35s ease;
  z-index: 9999;
}

.toast.show {
  opacity: 1;
  transform: translateY(0);
}
.cite-select:hover {
  border-color: rgba(102,252,241,0.40);
  cursor: pointer;
}
  .site-footer {
  margin-top: 55px;
  text-align: center;
  font-size: 0.85rem;
  color: #a8c3d9;
  opacity: 0.8;
  padding-top: 20px;
  border-top: 1px solid rgba(102,252,241,0.10);
}
/* Global resets */
body {
  margin: 0;
  padding: 0;
  font-family: "Inter", -apple-system, BlinkMacSystemFont, system-ui, sans-serif;
  color: #e8e9ef;
  line-height: 1.75;
  background: #000;
  overflow-x: hidden;
}

/* Starfield background (static image) */
body {
  margin: 0;
  padding: 0;
  font-family: "Inter", sans-serif;
  color: #e8e9ef;
  line-height: 1.75;
  background: url("cosmos.jpeg") no-repeat center center fixed;
  background-size: cover;
  overflow-x: hidden;
}
/* Page container */
.page {
  max-width: 900px;
  margin: 90px auto;
  background: rgba(10, 13, 20, 0.72);
  padding: 50px;
  border-radius: 18px;
  border: 1px solid rgba(102,252,241,0.12);
  box-shadow: 0 0 35px rgba(102,252,241,0.18);
  backdrop-filter: blur(12px);
}

/* Headings */
h1, h2, h3 {
  font-family: "Merriweather", serif;
  font-weight: 300;
  color: #9be7ff;
  margin-top: 0;
}

h1 {
  text-align: center;
  font-size: 2.4rem;
  letter-spacing: 0.5px;
}

h2 {
  font-size: 1.8rem;
  margin-top: 40px;
}

h3 {
  color: #b9ecff;
  margin-bottom: 12px;
}

/* Dividers */
hr {
  border: none;
  height: 1px;
  background: linear-gradient(to right, transparent, #568ea6, transparent);
  margin: 45px 0;
}

/* Author box */
.author-box {
  display: flex;
  gap: 25px;
  align-items: center;
  background: rgba(15, 22, 32, 0.55);
  padding: 25px;
  border-radius: 14px;
  border: 1px solid rgba(102,252,241,0.12);
  box-shadow: inset 0 0 15px rgba(102,252,241,0.09);
}

.author-photo {
  width: 130px;
  height: 130px;
  border-radius: 8px;
  object-fit: cover;
  border: 2px solid rgba(102,252,241,0.22);
  box-shadow: 0 0 12px rgba(102,252,241,0.26);
}

/* Social box */
.social-box {
  background: rgba(15, 22, 32, 0.45);
  padding: 18px 25px;
  border-radius: 12px;
  border: 1px solid rgba(102,252,241,0.10);
  margin-top: 25px;
}

/* Social links with logos */
.social-link {
  display: flex;
  align-items: center;
  gap: 10px;
  color: #aeeaff;
  text-decoration: none;
  margin-bottom: 8px;
  transition: 0.2s ease;
  font-size: 0.98rem;
}

.social-link:hover {
  color: #66fcf1;
  text-shadow: 0 0 8px rgba(102,252,241,0.8);
}

.social-icon {
  width: 20px;
  height: 20px;
  flex-shrink: 0;
}

.social-icon svg {
  width: 100%;
  height: 100%;
  fill: #aeeaff;
}
.social-icon img {
  width: 22px;
  height: 22px;
  vertical-align: middle;
  margin-right: 8px;
}
/* Paper box */
.paper-box {
  background: rgba(15, 22, 32, 0.45);
  padding: 30px;
  border-radius: 14px;
  border: 1px solid rgba(102,252,241,0.10);
  box-shadow: 0 0 20px rgba(102,252,241,0.12);
}

/* Button */
.paper-button {
  display: inline-block;
  padding: 12px 28px;
  background: #d2f2ff;
  color: #0b0c10;
  font-size: 1.05rem;
  border-radius: 7px;
  text-decoration: none;
  transition: 0.2s;
}

.paper-button:hover {
  background: #bfe6f7;
  box-shadow: 0 0 16px rgba(174,234,255,0.8);
}

.center { text-align: center; }

/* Details (collapsible sections) */
details {
  margin-top: 30px;
  background: rgba(15, 22, 32, 0.45);
  border-radius: 12px;
  border: 1px solid rgba(102,252,241,0.14);
  padding: 16px 20px;
}

details + details {
  margin-top: 22px;
}

details summary {
  cursor: pointer;
  list-style: none;
  font-family: "Merriweather", serif;
  font-weight: 300;
  font-size: 1.1rem;
  color: #c5f2ff;
}

details summary::-webkit-details-marker {
  display: none;
}

.summary-label {
  display: inline-block;
  position: relative;
  padding-left: 18px;
}

.summary-label::before {
  content: "▸";
  position: absolute;
  left: 0;
  top: 0;
  font-size: 0.9rem;
  transition: transform 0.15s ease;
}

details[open] .summary-label::before {
  transform: rotate(90deg);
}

.details-body {
  margin-top: 14px;
  font-size: 0.95rem;
}

/* Symbol table */
.symbol-table {
  width: 100%;
  border-collapse: collapse;
  font-size: 0.9rem;
}

.symbol-table th,
.symbol-table td {
  border: 1px solid rgba(120,160,190,0.6);
  padding: 6px 8px;
  vertical-align: top;
}

.symbol-table th {
  background: rgba(40,60,85,0.7);
  font-weight: 400;
}

.symbol-table tr:nth-child(even) td {
  background: rgba(15, 22, 32, 0.65);
}

/* Reference list */
.ref-list {
  margin: 0;
  padding-left: 22px;
  font-size: 0.92rem;
  color: #ffffff; /* text inside the list is white */
}

/* Each list item */
.ref-list li {
  margin-bottom: 6px;
  color: #ffffff; /* ensure all li are white */
}

/* Reference links inside list */
.ref-list a {
  color: #ffffff;             /* default = white */
  text-decoration: none;
  transition: color 0.25s ease, text-shadow 0.25s ease;
}

/* Hover effect */
.ref-list a:hover {
  color: #9bd8ff; /* soft light blue */
  text-shadow: 0 0 6px rgba(140,200,255,0.8);
}

</style>

<!-- Stars -->
<div class="star-layer"></div>
<div class="star-layer"></div>
<div class="star-layer"></div>
<a id="top"></a>
<nav class="nav-header">
  <a href="#reviewer-guide">Guide</a>
  <a href="#what-this-work-proposes">This work</a>
  <a href="#symbol-index">Symbols</a>
  <a href="#derivations">Derivations</a>
  <a href="#calculator">Calculator</a>
  <a href="#comparison-qkde">Comparisons</a>
  <a href="#references-qkde">References</a>
  <a href="#cite-qkde">Cite</a>
  <a class="nav-button" href="QKDE_v.3F.pdf">
    View PDF
  </a>
  
  
</nav>
<div class="page">
<h1>Quantum–Kinetic Dark Energy (QKDE)</h1>
<p style="text-align:center; margin-top:-10px; font-style: italic;">
An effective dark energy framework with the Einstein–Hilbert metric sector intact and a time-dependent scalar kinetic normalization
</p>

<div class="author-box">
  <img src="photoDaniel.jpg" alt="Author photo" class="author-photo">

  <div>
  <h2>Daniel Brown</h2>
  <p>Independent researcher exploring dark energy, scalar-field physics, and cosmic expansion through effective field theory and first-principles modeling.</p>
  <p>Graduate of the University of Utah and resident of Salt Lake City, Utah.</p>
  <p>Author of the monograph <em>Quantum–Kinetic Dark Energy</em>, a revision and expansion of the earlier Scalar-Cost Dark Energy framework.</p>
  <p>My work aims to clarify minimal, GR-consistent explanations of late-time acceleration while developing reproducible numerical tools and observational tests.</p>
</div>
</div>

<div class="social-box">

  <a href="https://orcid.org/0009-0001-8082-9702" class="social-link" target="_blank">
  <span class="social-icon">
    <img src="ORCID_iD.svg.png" alt="ORCID logo" />
  </span>
  <span>ORCiD</span>
</a>

  <a href="https://github.com/DanielBrown124/QKDE" class="social-link" target="_blank">
    <span class="social-icon">
      <!-- GitHub mark (simplified) -->
      <svg viewBox="0 0 24 24" aria-hidden="true">
        <path d="M12 1.5A10.5 10.5 0 0 0 1.5 12c0 4.63 3 8.56 7.17 9.95.53.1.73-.23.73-.5v-1.75c-2.92.64-3.54-1.4-3.54-1.4-.48-1.2-1.17-1.52-1.17-1.52-.96-.65.07-.63.07-.63 1.06.08 1.62 1.1 1.62 1.1.95 1.63 2.5 1.16 3.11.89.1-.7.37-1.16.68-1.43-2.33-.27-4.78-1.18-4.78-5.25 0-1.16.42-2.1 1.1-2.84-.11-.27-.48-1.36.1-2.83 0 0 .9-.29 2.95 1.08a10.1 10.1 0 0 1 5.38 0c2.05-1.37 2.95-1.08 2.95-1.08.58 1.47.21 2.56.1 2.83.68.74 1.1 1.68 1.1 2.84 0 4.08-2.45 4.98-4.79 5.25.38.33.73.97.73 1.96v2.9c0 .27.2.6.73.5A10.52 10.52 0 0 0 22.5 12 10.5 10.5 0 0 0 12 1.5Z" />
      </svg>
    </span>
    <span>GITHUB REPOSITORY</span>
  </a>

  <a href="https://doi.org/10.5281/zenodo.17757109" class="social-link" target="_blank">
    <span class="social-icon">
    <img src="zenodo.ico" alt="ZENODO logo" />
  </span>
  <span>ZENODO</span>
</a>

  <a href="https://independent.academia.edu/DanielBrown462" class="social-link" target="_blank">
    <span class="social-icon">
    <img src="academia.png" alt="ACADEMIA logo" />
  </span>
    <span>ACADEMIA</span>
  </a>
  <a href="https://www.researchgate.net/profile/Daniel-Brown-133?ev=hdr_xprf" class="social-link" target="_blank">
    <span class="social-icon">
    <img src="ResearchGate.png" alt="RESEARCHGATE LOGO"/>
  </span>
    <span>RESEARCHGATE</span>
  </a>
</div>

<hr>
<div class="center" style="margin-top: 35px;">
  <a class="paper-button" href="QKDE_v.3F.pdf">
    QKDE Paper (PDF)
  </a>
</div>
<details id="reviewer-guide">
  <summary><span class="summary-label">Reviewer Quick-Guide</span></summary>
  <div class="details-body">

    <p>
      This section is designed to assist journal referees, editors, and technically oriented
      readers in quickly understanding the theoretical status, assumptions, and testability 
      of the Quantum–Kinetic Dark Energy (QKDE) framework.  
      It highlights what the model claims, what it does <em>not</em> claim, how it differs 
      from nearby theories, and how all results can be reproduced.
    </p>

    <!-- ========================================================= -->
    <!-- 1. What QKDE Actually Claims                              -->
    <!-- ========================================================= -->
    <h3>1. What QKDE Claims</h3>

    <ul>
      <li><strong>QKDE is a single-scalar, GR-preserving dark-energy framework</strong> with no 
          modification to the Einstein–Hilbert metric sector.</li>

      <li><strong>Cosmic acceleration arises entirely from a scalar sector</strong> of the form  
          \(P(X,\phi,t) = K(t)X - V(\phi)\), where the <em>kinetic normalization</em> 
          \(K(t) > 0\) drifts slowly in time.</li>

      <li><strong>All EFT–DE gravitational functions vanish</strong> except  
          \(\alpha_K = K\dot{\phi}^2/(H^2 M_{\rm pl}^2) > 0\):  
          <br><code>α_B = α_M = α_T = α_H = 0</code>.</li>

      <li><strong>Gravitational waves are luminal</strong> (\(c_T^2 = 1\)),  
          the <strong>Planck mass is constant</strong>,  
          and <strong>metric potentials satisfy</strong> \(\Phi = \Psi\).</li>

      <li><strong>The linear growth equation is exactly GR</strong>: all deviations enter only 
          through the background expansion history \(H(a)\).</li>

      <li><strong>The model is falsifiable</strong>:  
          \(\mu(a,k)=\Sigma(a,k)=1,\;\eta(a,k)=0\) on linear scales.  
          Any statistically significant deviation excludes QKDE.</li>
    </ul>

    <!-- ========================================================= -->
    <!-- 2. What QKDE Does NOT Claim                               -->
    <!-- ========================================================= -->
    <h3>2. What QKDE Does <em>Not</em> Claim</h3>

    <ul>
      <li>It does <strong>not</strong> modify gravity, introduce an evolving Planck mass, or alter 
          light deflection.</li>

      <li>It does <strong>not</strong> introduce scale-dependent growth, screening mechanisms, 
          sound speeds \(c_s^2 \neq 1\), or higher-derivative operators.</li>

      <li>It does <strong>not</strong> attempt to solve the cosmological constant problem.</li>

      <li>It does <strong>not</strong> rely on phenomenological templates;  
          all equations come from the covariant action and the EFT mapping.</li>

      <li>It does <strong>not</strong> introduce extra degrees of freedom beyond the single scalar.</li>
    </ul>

    <!-- ========================================================= -->
    <!-- 3. Why QKDE ≠ Quintessence                                -->
    <!-- ========================================================= -->
    <h3>3. Why QKDE Is Not Quintessence</h3>

    <ul>
      <li>Quintessence uses <strong>fixed canonical normalization</strong>:  
          \(P(X,\phi)=X-V(\phi)\).</li>

      <li>QKDE uses <strong>time-dependent kinetic normalization</strong>  
          \(K(t)X\), motivated by curvature-suppressed operators and integrating 
          out heavy fields in QFT in curved spacetime.</li>

      <li>Quintessence variations affect \(V(\phi)\);  
          QKDE variations occur in \(K(t)\).</li>

      <li>Quintessence has <strong>no operator-level EFT derivation for a running kinetic term</strong>;  
          QKDE explicitly builds this in from the UV-motivated operator \(R X\).</li>
    </ul>

    <!-- ========================================================= -->
    <!-- 4. Why QKDE ≠ k-essence                                   -->
    <!-- ========================================================= -->
    <h3>4. Why QKDE Is Not k-Essence</h3>

    <ul>
      <li>k-essence allows broad functional freedom: \(P(X,\phi)\).</li>

      <li>QKDE is a <strong>highly constrained subset</strong>:
          <br><code>P = K(t)X - V(φ)</code>  
          with no higher powers of \(X\) and no noncanonical speeds.</li>

      <li>Generic k-essence yields <strong>non-unit sound speeds</strong>;  
          QKDE enforces \(c_s^2 = 1\) exactly.</li>

      <li>k-essence can generate <strong>scale-dependent growth</strong>;  
          QKDE predicts GR-like, scale-independent growth.</li>

      <li>QKDE’s drift \(K(t)\) is <strong>time-only</strong>, unlike general 
          k-essence dependence on both \(X\) and \(\phi\).</li>
    </ul>

    <!-- ========================================================= -->
    <!-- 5. Mathematical Structure                                 -->
    <!-- ========================================================= -->
    <h3>5. Mathematical Structure</h3>

    <ul>
      <li><strong>Variables:</strong> \( (H, \phi, s=\phi') \).</li>

      <li>Closed background system (no iteration):  
        \[
          \phi' = s, \qquad
          s' = -(3+E)s - (K'/K)s - \frac{V_{,\phi}}{H^2 K}, \qquad
          E = \frac{H'}{H}.
        \]
      </li>

      <li><strong>Curvature-based model:</strong>  
        \[
        K = 1 + \frac{\alpha R}{M^2}, \qquad
        \frac{K'}{K} = 
        \frac{\alpha R}{M^2 + \alpha R}
        \left( 2E + \frac{E'}{2+E} \right).
        \]
      </li>

      <li><strong>Running model:</strong>  
        \[
        K(N)=1+K_0 e^{-pN},\qquad
        \frac{K'}{K} = \frac{-p K_0 e^{-pN}}{1 + K_0 e^{-pN}}.
        \]
      </li>

      <li><strong>Perturbations:</strong>  
        \[
        \Phi=\Psi,\quad c_s^2=1,\quad \mu=1,\quad \Sigma=1,\quad \eta=0.
        \]
      </li>
    </ul>

    <!-- ========================================================= -->
    <!-- 6. Testability                                            -->
    <!-- ========================================================= -->
    <h3>6. Testable Predictions</h3>

    <ul>
      <li><strong>Null tests:</strong>  
        \[
        \mu(a,k)=1, \qquad \Sigma(a,k)=1, \qquad \eta(a,k)=0.
        \]
      </li>
      <li><strong>No scale dependence</strong> in linear growth.</li>
      <li><strong>No deviations in GW propagation</strong> (\(c_T^2=1\)).</li>
      <li><strong>All departures from ΛCDM appear only in:</strong>  
        <ul>
          <li>expansion history \(H(a)\),</li>
          <li>effective equation of state \(w_{\rm eff}(a)\),</li>
          <li>growth factor \(D(a)\).</li>
        </ul>
      </li>
    </ul>

    <!-- ========================================================= -->
    <!-- 7. Reproducibility                                        -->
    <!-- ========================================================= -->
    <h3>7. How to Reproduce All Results</h3>

    <p>Everything needed to reproduce the paper’s results is provided:</p>

    <ul>
      <li>Full background system in closed algebraic form.</li>
      <li>Consistent definitions of \(E, R, K'/K\), and all residual checks.</li>
      <li>Fisher setup using exact <em>sensitivity equations</em> (not numerical derivatives).</li>
      <li>Parameters and priors listed explicitly.</li>
      <li>Figures and tables regenerated from the same pipeline.</li>
      <li>Notebook + code provided in the GitHub repository.</li>
    </ul>

  </div>
</details>
<h2 id="what-this-work-proposes">What This Work Proposes</h2>

<div class="paper-box">

<h3>1. A minimal and GR-respecting dark energy model</h3>

<p>
Quantum–Kinetic Dark Energy (QKDE) introduces a time-dependent kinetic normalization for a scalar field while leaving the Einstein–Hilbert metric sector intact. The scalar sector is
</p>

\[
P(X,\phi,t) = K(t)\,X - V(\phi), \qquad K(t) > 0,
\]

\[
X = -\tfrac12 g^{\mu\nu}\partial_\mu\phi\,\partial_\nu\phi.
\]

<p>
This structure is motivated by curvature-suppressed operators in quantum field theory in curved spacetime, which naturally generate such running kinetic prefactors in an effective description.
</p>

<hr>

<h3>2. Gravity remains exactly Einsteinian</h3>

<p>
The Einstein–Hilbert metric sector is unmodified. In effective-field-theory language, the Planck mass is constant, gravitational waves are luminal, and there is no braiding or beyond-Horndeski structure. At the level of metric perturbations:
</p>

\[
\Phi = \Psi,\qquad c_T^2 = 1.
\]

<p>
QKDE therefore lives in the GR-preserving corner of the dark-energy theory space: it is not a modified-gravity model, but a controlled deformation of the scalar sector only.
</p>

<hr>

<h3>3. Observable effects originate only from background evolution</h3>

<p>
All deviations from ΛCDM in QKDE arise through the background expansion history and the induced linear growth:
</p>

\[
H(a), \qquad D(a),
\]

<p>
rather than through modified Poisson equations, slip, or new forces. Linear growth satisfies the GR growth equation with an altered history of \(H(a)\), leading to clean, falsifiable null tests.
</p>

<hr>

<h3>4. EFT of Dark Energy characterization</h3>

<p>
In the Effective Field Theory of Dark Energy (EFT–DE) language, QKDE is characterized by a single active background function:
</p>

\[
\alpha_K > 0,
\]

<p>
while
</p>

\[
\alpha_B = \alpha_M = \alpha_T = \alpha_H = 0.
\]

<p>
This enforces luminal tensors, a constant Planck mass, no braiding, and no beyond-Horndeski structure, keeping the gravitational sector strictly Einsteinian at the linear level.
</p>

<hr>

<h3>5. Concrete realizations of \(K(t)\)</h3>

<p>
The paper analyzes two illustrative realizations of the kinetic normalization:
</p>

<p>Curvature-motivated form</p>

\[
K = 1 + \frac{\alpha R}{M^2},
\]

<p>
with a fully algebraic, iteration-free identity for \(K'/K\) that closes the background system.
</p>

<p>Phenomenological running</p>

\[
K = 1 + K_0 (1+z)^{p},
\]

<p>
which parameterizes late-time drift with a small number of physically interpretable parameters.
</p>

<hr>

<h3>6. Background system, stability, and forecasts</h3>

<p>
From the unitary-gauge action
</p>

\[
S=\int d^{4}x\,\sqrt{-g}\,\left[\tfrac12 M_{\rm pl}^{2}R+K(t)X-V(\phi)\right],
\]

<p>
the work derives a closed first-order background system in e-fold time \(N = \ln a\), together with a scalar sector that propagates with sound speed
</p>

\[
c_s^2 = 1
\]

<p>
and no gravitational slip. Stability and admissibility reduce to the positivity of \(K(t)\) and the nonvanishing of a specific algebraic denominator in the curvature-based model.
</p>

<p>
A reproducible numerical pipeline is detailed, including the state vector, tolerances, and identity checks, together with a Fisher forecast setup based on exact sensitivity equations for distances, \(H(z)\), and \(f\sigma_8(z)\).
</p>

<hr>

<h3>7. Null tests and falsifiability</h3>

<p>
At linear scales and in the quasi-static regime, QKDE predicts:
</p>

\[
\mu(a,k) = 1,\qquad \Sigma(a,k) = 1,\qquad \eta(a,k) = 0,\qquad c_T^2 = 1,
\]

<p>
where \(\mu\) is the effective Newton constant, \(\Sigma\) the effective lensing strength, \(\eta\) the gravitational slip, and \(c_T\) the tensor speed. Any robust observational deviation from these null tests would rule out the QKDE baseline, providing a clear path to falsifiability.
</p>

<div class="center" style="margin-top: 35px;">
  <a class="paper-button" href="QKDE_v.3F.pdf">
    QKDE Paper (PDF)
  </a>
</div>

</div> <!-- end paper-box -->

<hr>

<details id="symbol-index">
  <summary><span class="summary-label">Symbol index</span></summary>
  <div class="details-body">

    <p>
    Key symbols and definitions used throughout the work. Units are in natural conventions \(c = \hbar = 1\); mass dimensions are indicated where relevant.
    </p>

    <table class="symbol-table">
      <thead>
        <tr>
          <th>Symbol</th>
          <th>Units</th>
          <th>Definition / Role</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>\(a(t)\)</td>
          <td>1</td>
          <td>Scale factor; \(N \equiv \ln a\) is the e-fold time.</td>
        </tr>
        <tr>
          <td>\(z\)</td>
          <td>1</td>
          <td>Redshift; \(z(N) = e^{-N} - 1\).</td>
        </tr>
        <tr>
          <td>\(H, H_0\)</td>
          <td>M</td>
          <td>Hubble rate and its value today.</td>
        </tr>
        <tr>
          <td>\(E\)</td>
          <td>1</td>
          <td>Hubble e-fold derivative: \(E \equiv H'/H\).</td>
        </tr>
        <tr>
          <td>\(R\)</td>
          <td>M\(^2\)</td>
          <td>FRW Ricci scalar: \(R = 6(2H^2 + \dot H) = 6H^2(2 + E)\).</td>
        </tr>
        <tr>
          <td>\(M_{\rm pl}\)</td>
          <td>M</td>
          <td>Reduced Planck mass, \(M_{\rm pl} = (8\pi G)^{-1/2}\).</td>
        </tr>
        <tr>
          <td>\(\rho_i, p_i\)</td>
          <td>M\(^4\)</td>
          <td>Energy density and pressure for \(i \in \{m,r,\phi\}\).</td>
        </tr>
        <tr>
          <td>\(\Omega_i\)</td>
          <td>1</td>
          <td>\(\Omega_i \equiv \rho_i/(3M_{\rm pl}^2 H^2)\).</td>
        </tr>
        <tr>
          <td>\(w_{\rm eff}, q\)</td>
          <td>1</td>
          <td>\(w_{\rm eff} = -1 - \tfrac{2}{3} E\), \(q = -1 - E\).</td>
        </tr>
        <tr>
          <td>\(\chi\)</td>
          <td>M\(^{-1}\)</td>
          <td>Comoving distance: \(\chi(z) = \int_0^z \mathrm{d}z'/H(z')\).</td>
        </tr>
        <tr>
          <td>\(D_A, D_L\)</td>
          <td>M\(^{-1}\)</td>
          <td>Angular-diameter and luminosity distances: \(D_A = \chi/(1+z)\), \(D_L = (1+z)\chi\).</td>
        </tr>
        <tr>
          <td>\(D_V\)</td>
          <td>M\(^{-1}\)</td>
          <td>Volume-averaged BAO distance: \(D_V = [(1+z)^2 D_A^2 z/H]^{1/3}\).</td>
        </tr>
        <tr>
          <td>\(F_{\rm AP}\)</td>
          <td>1</td>
          <td>Alcock–Paczyński combination: \(F_{\rm AP} = (1+z) D_A H^{-1}\).</td>
        </tr>
        <tr>
          <td>\(r_d\)</td>
          <td>M\(^{-1}\)</td>
          <td>Sound horizon at drag epoch: \(r_d = \int_{z_d}^{\infty} c_s/H \,\mathrm{d}z\).</td>
        </tr>
        <tr>
          <td>\(\eta\) (conformal time)</td>
          <td>M\(^{-1}\)</td>
          <td>Conformal time, defined by \(\mathrm{d}t = a\,\mathrm{d}\eta\).</td>
        </tr>
        <tr>
          <td>\(\phi\)</td>
          <td>M</td>
          <td>Homogeneous scalar field.</td>
        </tr>
        <tr>
          <td>\(X\)</td>
          <td>M\(^4\)</td>
          <td>Kinetic invariant: \(X \equiv -\tfrac12 g^{\mu\nu} \partial_\mu\phi \partial_\nu\phi\); FRW: \(X = \tfrac12 \dot\phi^2\).</td>
        </tr>
        <tr>
          <td>\(V(\phi)\)</td>
          <td>M\(^4\)</td>
          <td>Scalar potential.</td>
        </tr>
        <tr>
          <td>\(K(t)\)</td>
          <td>1</td>
          <td>Background kinetic normalization; \(K>0\) for ghost freedom.</td>
        </tr>
        <tr>
          <td>\(\alpha, M\)</td>
          <td>1, M</td>
          <td>Curvature model parameters in \(K = 1 + \alpha R/M^2\).</td>
        </tr>
        <tr>
          <td>\(K_0, p, N_p\)</td>
          <td>1, 1, 1</td>
          <td>Running form parameters: \(K(N) = 1 + K_0 e^{-pN} = 1 + K_p e^{-p(N-N_p)}\).</td>
        </tr>
        <tr>
          <td>\(K'/K\)</td>
          <td>1</td>
          <td>E-fold derivative of \(K\); closed algebraic expression in the curvature model.</td>
        </tr>
        <tr>
          <td>\(\rho_\phi, p_\phi\)</td>
          <td>M\(^4\)</td>
          <td>\(\rho_\phi = KX + V\), \(p_\phi = KX - V\).</td>
        </tr>
        <tr>
          <td>\(w_\phi\)</td>
          <td>1</td>
          <td>Scalar equation of state: \(w_\phi = (KX - V)/(KX + V)\).</td>
        </tr>
        <tr>
          <td>\(\Phi, \Psi\)</td>
          <td>1</td>
          <td>Bardeen potentials (Newtonian gauge); here \(\Phi = \Psi\).</td>
        </tr>
        <tr>
          <td>\(v, z\)</td>
          <td>M, M</td>
          <td>Gauge-invariant variables: \(v = a(\delta\phi + \dot\phi\,\Phi/H)\); \(z^2 = a^2 K \dot\phi^2/H^2\).</td>
        </tr>
        <tr>
          <td>\(\mathcal{R}\)</td>
          <td>1</td>
          <td>Comoving curvature perturbation: \(\mathcal{R} = v/z\).</td>
        </tr>
        <tr>
          <td>\(c_s^2\)</td>
          <td>1</td>
          <td>Scalar sound speed; in QKDE, \(c_s^2 = 1\).</td>
        </tr>
        <tr>
          <td>\(c_T^2\)</td>
          <td>1</td>
          <td>Tensor propagation speed; in QKDE, \(c_T^2 = 1\).</td>
        </tr>
        <tr>
          <td>\(\alpha_K, \alpha_B, \alpha_M, \alpha_T, \alpha_H\)</td>
          <td>1</td>
          <td>EFT–DE functions. In QKDE: \(\alpha_K = K \dot\phi^2/(H^2 M_{\rm pl}^2) \ge 0\); all others vanish.</td>
        </tr>
        <tr>
          <td>\(\mu(a,k)\)</td>
          <td>1</td>
          <td>Linear effective Newton constant in modified Poisson equation; here \(\mu = 1\).</td>
        </tr>
        <tr>
          <td>\(\Sigma(a,k)\)</td>
          <td>1</td>
          <td>Effective lensing modifier; here \(\Sigma = 1\).</td>
        </tr>
        <tr>
          <td>\(\eta(a,k)\)</td>
          <td>1</td>
          <td>Gravitational slip: \(\eta \equiv \Phi/\Psi - 1\); here \(\eta = 0\).</td>
        </tr>
        <tr>
          <td>\(k, \ell\)</td>
          <td>M, 1</td>
          <td>Comoving wavenumber and multipole index.</td>
        </tr>
        <tr>
          <td>\(P(k,z)\)</td>
          <td>M\(^{-3}\)</td>
          <td>Linear matter power spectrum; scales as \(P(k,z) = D^2(z) P(k,0)\).</td>
        </tr>
        <tr>
          <td>\(D(a)\)</td>
          <td>1</td>
          <td>Linear growth factor, satisfying the GR growth equation with modified \(H(a)\).</td>
        </tr>
        <tr>
          <td>\(f\)</td>
          <td>1</td>
          <td>Growth rate: \(f \equiv \mathrm{d}\ln D / \mathrm{d}\ln a\).</td>
        </tr>
        <tr>
          <td>\(\sigma_{8,0}\)</td>
          <td>1</td>
          <td>RMS matter fluctuation in \(8\,h^{-1}\,\mathrm{Mpc}\) at \(z=0\).</td>
        </tr>
        <tr>
          <td>\(f\sigma_8(z)\)</td>
          <td>1</td>
          <td>RSD observable: \(f(z)\,\sigma_{8,0}\,D(z)/D(0)\).</td>
        </tr>
        <tr>
          <td>\(s\)</td>
          <td>1</td>
          <td>Background scalar velocity in e-fold time: \(s \equiv \phi'\).</td>
        </tr>
        <tr>
          <td>\(y_H\)</td>
          <td>1</td>
          <td>Log-Hubble variable: \(y_H \equiv \ln H\).</td>
        </tr>
        <tr>
          <td>\(C_F\)</td>
          <td>1</td>
          <td>Friedmann-closure residual: \(C_F = 1 - \Omega_m - \Omega_r - \Omega_\phi\).</td>
        </tr>
        <tr>
          <td>\(C_R\)</td>
          <td>1</td>
          <td>Raychaudhuri residual in e-fold form (used as a consistency check).</td>
        </tr>
        <tr>
          <td>\(C_\phi\)</td>
          <td>1</td>
          <td>Background Klein–Gordon residual (consistency of scalar equation).</td>
        </tr>
        <tr>
          <td>\(C_{R/H^2}\)</td>
          <td>1</td>
          <td>Residual for the identity \(R/H^2 = 6(2 + H'/H)\).</td>
        </tr>
        <tr>
          <td>\(C_{\nabla\cdot T_\phi}\)</td>
          <td>1</td>
          <td>Residual measuring non-conservation due to \(K'(N)\) in the scalar energy–momentum tensor.</td>
        </tr>
        <tr>
          <td>\(\mu_{\rm SN}(z)\)</td>
          <td>1</td>
          <td>Distance modulus: \(\mu_{\rm SN}(z) = 5\log_{10}(D_L/\mathrm{Mpc}) + 25\).</td>
        </tr>
        <tr>
          <td>\(Q_\mu\)</td>
          <td>M\(^3\)</td>
          <td>Source term for an interaction four-vector \(Q_\mu\) when present (used for bookkeeping of energy exchange).</td>
        </tr>
      </tbody>
    </table>

  </div>
  </details>
<details id="derivations">
  <summary><span class="summary-label">Derivations</span></summary>
  <div class="details-body">

    <p>
      This section collects <strong>all principal analytic derivations</strong> used in the
      QKDE framework, organized into nested dropdowns for clarity. Everything matches
      the equations and notation in the monograph: no heuristic shortcuts, no omitted
      steps, and no approximations beyond those explicitly stated in the paper.
    </p>

    <!-- ===================================================== -->
    <!-- 0. Covariant Action and Variational Foundations      -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">0. Covariant action → field equations</span></summary>
      <div class="details-body">

        <p><strong>Starting point:</strong></p>

        \[
        S = \int d^4x\,\sqrt{-g}\,\left[\frac12 M_{\rm pl}^2 R + K(t)X - V(\phi)\right],
        \qquad
        X = -\frac12 g^{\mu\nu}\partial_\mu\phi\partial_\nu\phi .
        \]

        <h4>(a) Energy–momentum tensor</h4>

        Varying w.r.t. the metric:

        \[
        T_{\mu\nu} = K\,\partial_\mu\phi\partial_\nu\phi 
        - g_{\mu\nu}\left(KX - V\right).
        \]

        In FRW:

        \[
        \rho_\phi = KX + V, \qquad p_\phi = KX - V.
        \]

        <h4>(b) Scalar equation of motion</h4>

        Variation w.r.t. \(\phi\) gives:

        \[
        \nabla_\mu(K \nabla^\mu \phi) + V_{,\phi} = 0 .
        \]

        Because \(K = K(t)\):

        \[
        \nabla_\mu(K \nabla^\mu\phi)
        = K \Box\phi + K_{,\mu}\nabla^\mu\phi .
        \]

        In FRW:

        \[
        K(\ddot\phi + 3H\dot\phi) + \dot{K}\,\dot\phi + V_{,\phi}=0 .
        \]

        This is the starting point for the e-fold reformulation.

        <h4>(c) Einstein equations</h4>

        Friedmann:

        \[
        3M_{\rm pl}^2 H^2 = \rho_m + \rho_r + \rho_\phi .
        \]

        Raychaudhuri:

        \[
        M_{\rm pl}^2 (2\dot H + 3H^2) = -p_m - p_r - p_\phi .
        \]

        Nothing in QKDE modifies these except the new \(\rho_\phi, p_\phi\).
      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 1. E-fold background system                          -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">1. Closed background system (full derivation)</span></summary>
      <div class="details-body">

        <h4>(a) E-fold definitions</h4>

        \[
        N = \ln a, 
        \qquad f' \equiv \frac{df}{dN} = \frac{1}{H}\frac{df}{dt}.
        \]

        \[
        E \equiv \frac{H'}{H}.
        \]

        <h4>(b) Scalar velocity variable</h4>

        \[
        s \equiv \phi' = \frac{\dot\phi}{H}.
        \]

        Then:

        \[
        X = \frac12 \dot\phi^2 = \frac12 H^2 s^2.
        \]

        <h4>(c) Transforming the scalar EOM</h4>

        Starting from:

        \[
        K(\ddot\phi + 3H\dot\phi) + \dot K\,\dot\phi + V_{,\phi} = 0
        \]

        Convert derivatives:

        \[
        \ddot\phi = H^2 s' + H H's .
        \]

        Plug in:

        \[
        K\left(H^2 s' + H^2 E s + 3 H^2 s\right)
        + (H K' ) H s 
        + V_{,\phi} = 0.
        \]

        Divide by \(H^2 K\):

        \[
        s' + (3+E)s + \frac{K'}{K}s + \frac{1}{H^2 K} V_{,\phi} =0.
        \]

        So:

        \[
        s' = - (3+E)s - \frac{K'}{K}s - \frac{V_{,\phi}}{H^2 K}.
        \]

        <h4>(d) Full background system</h4>

        \[
        \phi' = s,
        \]

        \[
        s' = -(3+E)s - \frac{K'}{K}s - \frac{V_{,\phi}}{H^2K},
        \]

        \[
        E = \frac{H'}{H}.
        \]

        The system becomes deterministic once \(K'/K\) is known.

      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 2. Ricci identities and curvature relations          -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">2. Ricci scalar & e-fold identities</span></summary>
      <div class="details-body">
        <h4>(a) Ricci scalar in FRW</h4>

        \[
        R = 6(2H^2 + \dot H).
        \]

        Write \(\dot H = H^2 E\):

        \[
        R = 6H^2(2 + E).
        \]

        <h4>(b) Derivative of \(R\)</h4>

        \[
        \frac{R'}{R} = 2E + \frac{E'}{2+E}.
        \]
      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 3. K(t) derivations: curvature-based and running      -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">3. Kinetic normalization derivations</span></summary>
      <div class="details-body">

        <!-- Curvature Model -->
        <details>
          <summary><span class="summary-label">3a. Curvature-induced \(K(N)\)</span></summary>
          <div class="details-body">

            <p>Start with:</p>

            \[
            K = 1 + \frac{\alpha R}{M^2}.
            \]

            Then:

            \[
            \frac{K'}{K} =
            \frac{\alpha R'}{M^2 + \alpha R}.
            \]

            Using the Ricci identity:

            \[
            \frac{R'}{R} = 2E + \frac{E'}{2+E},
            \]

            gives:

            \[
            \frac{K'}{K}
            = \frac{\alpha R}{M^2 + \alpha R}
              \left(2E + \frac{E'}{2+E}\right).
            \]

            This closes the system exactly — no numerical differentiation needed.
          </div>
        </details>

        <!-- Running Model -->
        <details>
          <summary><span class="summary-label">3b. Running form \(K(N)\)</span></summary>
          <div class="details-body">

            <p>Parametrization:</p>

            \[
            K(N) = 1 + K_0 e^{-pN}.
            \]

            Then:

            \[
            \frac{K'}{K} =
            \frac{-p K_0 e^{-pN}}{1 + K_0 e^{-pN}}.
            \]

            Useful reparametrization:

            \[
            K(N) = 1 + K_p e^{-p(N-N_p)}.
            \]
          </div>
        </details>
      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 4. Energy-momentum tensor, rho, p, EOS               -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">4. Energy–momentum components & equation of state</span></summary>
      <div class="details-body">
        \[
        \rho_\phi = KX + V,
        \qquad
        p_\phi = KX - V.
        \]

        In FRW:

        \[
        X = \frac12 H^2 s^2.
        \]

        Scalar equation-of-state:

        \[
        w_\phi = \frac{KX - V}{KX + V}.
        \]
      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 5. Klein-Gordon equation (full derivation)           -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">5. Full Klein–Gordon derivation in e-fold time</span></summary>
      <div class="details-body">
        From the FRW scalar EOM:

        \[
        K(\ddot\phi + 3H\dot\phi) + \dot K\,\dot\phi + V_{,\phi}=0.
        \]

        Convert to e-fold variables step by step:

        - \(\dot\phi = H s\)  
        - \(\ddot\phi = H^2 s' + H^2 E s\)

        Insert:

        \[
        K\left(H^2 s' + H^2 E s + 3H^2 s\right)
        + HK' Hs + V_{,\phi} = 0.
        \]

        Divide by \(H^2 K\):

        \[
        s' = -(3+E)s - \frac{K'}{K}s - \frac{V_{,\phi}}{H^2K}.
        \]
      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 6. EFT-DE mapping                                    -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">6. EFT–DE mapping (exact)</span></summary>
      <div class="details-body">

        The unitary-gauge action:

        \[
        S = \int \! d^4x \sqrt{-g}\,
        \big[\tfrac12 M_{\rm pl}^2 R + K(t)X - V(\phi)\big]
        \]

        corresponds to:

        \[
        \alpha_K = \frac{K \dot\phi^2}{H^2 M_{\rm pl}^2} > 0,
        \]

        with:

        \[
        \alpha_B = 0,\qquad
        \alpha_M = 0,\qquad
        \alpha_T = 0,\qquad
        \alpha_H = 0.
        \]

        Thus QKDE lies in the GR-preserving corner of EFT–DE.
      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 7. Perturbations: action, variables, sound speed     -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">7. Perturbation theory & sound speed derivation</span></summary>
      <div class="details-body">

        <h4>(a) Second-order action</h4>

        In Newtonian gauge, expand:

        \[
        S^{(2)} = \int d^4x\, a^3
        \left[
          K \dot\phi^2 (\dot{\delta\phi})^2
          - K \frac{(\nabla\delta\phi)^2}{a^2}
          + \ldots
        \right].
        \]

        <h4>(b) Canonical variable</h4>

        Define:

        \[
        v = a(\delta\phi + \dot\phi\,\Phi/H),
        \qquad
        z^2 = a^2 K\dot\phi^2/H^2.
        \]

        Then the action becomes the Mukhanov–Sasaki form:

        \[
        S^{(2)} = \frac12 \int d\eta\, d^3k \left[v'^2 - c_s^2 k^2 v^2 + \frac{z''}{z} v^2\right].
        \]

        <h4>(c) Sound speed</h4>

        The coefficient of \((\nabla\delta\phi)^2\) is exactly \(K\); the kinetic
        coefficient is also \(K\) → therefore:

        \[
        c_s^2 = 1.
        \]

        <h4>(d) Metric potentials</h4>

        The Einstein equations yield:

        \[
        \Phi = \Psi.
        \]

        And:

        \[
        \mu = 1,\quad \Sigma=1,\quad \eta=0.
        \]

        No modified gravity signatures appear.

      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 8. Growth equation                                   -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">8. Growth of structure derivation</span></summary>
      <div class="details-body">

        With \(\mu = 1\), linear matter perturbations satisfy:

        \[
        \ddot D + 2H \dot D - \frac{3}{2}H^2 \Omega_m D = 0.
        \]

        Convert to e-fold variables:

        \[
        D' = \frac{\dot D}{H},\qquad
        D'' = \frac{\ddot D}{H^2} - E D'.
        \]

        Insert:

        \[
        D'' + (2 + E)D' - \frac{3}{2}\Omega_m D = 0.
        \]

        All deviations from \(\Lambda\)CDM enter purely through \(H(N)\).

      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 9. Stability & admissibility                         -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">9. Stability conditions</span></summary>
      <div class="details-body">

        <h4>(a) Ghost freedom</h4>

        \[
        K(N) > 0.
        \]

        <h4>(b) Gradient stability</h4>

        \[
        c_s^2 = 1 > 0.
        \]

        <h4>(c) Curvature model viability</h4>

        \[
        M^2 + \alpha R \neq 0.
        \]

        These conditions ensure consistent propagation and exclude pathological coupling regimes.
      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 10. Numerical consistency checks                     -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">10. Numerical identity checks (pipeline)</span></summary>
      <div class="details-body">

        <p>The monograph includes exact consistency residuals:</p>

        <ul>
          <li>\(C_F = 1 - \Omega_m - \Omega_r - \Omega_\phi\)</li>
          <li>\(C_R = R/H^2 - 6(2+E)\)</li>
          <li>\(C_{\phi}\) from KG equation</li>
          <li>\(C_{\nabla\cdot T_\phi}\) for scalar conservation</li>
          <li>\(C_{R/H^2}\) verifying the Ricci identity</li>
        </ul>

        <p>
          These quantify reproducibility and ensure that all algebraic closures are satisfied
          at machine precision throughout the integration.
        </p>

      </div>
    </details>

  </div>
</details>
<details id="calculator">
  <summary><span class="summary-label">Interactive Calculator</span></summary>
  <div class="details-body">
    <section class="calc-section">
      <p class="calc-intro">
        Use these tools to explore a flat ΛCDM reference background and the running
        kinetic normalization in QKDE. They are lightweight, browser-side calculators
        intended for intuition and quick checks.
      </p>

      <div class="calc-grid">
        <!-- ================= ΛCDM CARD ================= -->
        <article class="calc-card" id="lcdm-card">
          <div class="calc-header-row">
            <h3>ΛCDM Background & Distances</h3>
            <div class="calc-pill-row" aria-label="ΛCDM presets">
              <button type="button" class="calc-pill is-active" data-preset="planck">
                Planck-like
              </button>
              <button type="button" class="calc-pill" data-preset="local">
                Local H₀
              </button>
            </div>
          </div>

          <h4>Flat ΛCDM reference model</h4>
          <p class="calc-note">
            Computes the dimensionless Hubble factor, H(z), comoving distance χ(z),
            angular-diameter distance D<sub>A</sub>(z), luminosity distance D<sub>L</sub>(z),
            and distance modulus μ.
          </p>

          <div class="calc-input-row">
            <div>
              <label class="calc-label">Redshift z</label>
              <input id="lcdm-z" class="calc-input" type="number" step="0.01" value="0.5">
            </div>
            <div>
              <label class="calc-label">H₀ [km/s/Mpc]</label>
              <input id="lcdm-h0" class="calc-input" type="number" step="0.1" value="70">
            </div>

            <div>
              <label class="calc-label">Ω<sub>m0</sub></label>
              <input id="lcdm-om" class="calc-input" type="number" step="0.001" value="0.3">
            </div>
            <div>
              <label class="calc-label">Ω<sub>r0</sub></label>
              <input id="lcdm-or" class="calc-input" type="number" step="1e-5" value="0.0">
            </div>

            <div>
              <label class="calc-label">Ω<sub>Λ0</sub></label>
              <input id="lcdm-ol" class="calc-input" type="number" step="0.001" value="0.7">
            </div>
            <div>
              <label class="calc-label">z-steps (integration)</label>
              <input id="lcdm-steps" class="calc-input" type="number" step="50" value="400">
            </div>
          </div>

          <div class="calc-action-row">
            <button type="button" class="calc-btn" id="lcdm-compute">
              Compute ΛCDM
            </button>
            <button type="button" class="calc-btn secondary" id="lcdm-formula-toggle">
              Show formulas
            </button>
          </div>

          <pre id="lcdm-output" class="calc-output" aria-live="polite"></pre>

          <div id="lcdm-formulas" class="calc-formula-box" aria-hidden="true">
            <div class="calc-formula-inner">
              <p>
                Flat ΛCDM with matter, radiation, and a cosmological constant:
              </p>
              <p>
                \( H(z) = H_0\,E(z), \qquad
                   E(z) = \sqrt{\Omega_{m0}(1+z)^3 + \Omega_{r0}(1+z)^4 + \Omega_{\Lambda0}} \).
              </p>
              <p>
                Comoving distance:
                \( \chi(z) = c \int_0^{z} \frac{dz'}{H_0\,E(z')} \).
              </p>
              <p>
                Angular-diameter and luminosity distances:
                \( D_A(z) = \chi(z)/(1+z),\quad D_L(z) = (1+z)\,\chi(z) \).
              </p>
              <p>
                Distance modulus:
                \( \mu = 5 \log_{10}\!\big[ D_L / \text{Mpc} \big] + 25 \).
              </p>
            </div>
          </div>
        </article>

        <!-- ================= QKDE CARD ================= -->
        <article class="calc-card" id="qkde-card">
          <div class="calc-header-row">
            <h3>QKDE Running–K Visualizer</h3>
            <div class="calc-pill-row" aria-label="QKDE presets">
              <button type="button" class="calc-pill is-active" data-qkde-preset="mild">
                Mild drift
              </button>
              <button type="button" class="calc-pill" data-qkde-preset="strong">
                Strong drift
              </button>
            </div>
          </div>

          <h4>Running kinetic normalization</h4>
          <p class="calc-note">
            Uses the parameterization \( K(N) = 1 + K_0 e^{-pN} \) with
            \( N = \ln a = -\ln(1+z) \). This does not solve the full background
            system; it isolates how the kinetic normalization drifts with redshift.
          </p>

          <div class="calc-input-row">
            <div>
              <label class="calc-label">Redshift z</label>
              <input id="qkde-z" class="calc-input" type="number" step="0.01" value="0.5">
            </div>
            <div>
              <label class="calc-label">K₀</label>
              <input id="qkde-k0" class="calc-input" type="number" step="0.05" value="0.5">
            </div>

            <div>
              <label class="calc-label">p</label>
              <input id="qkde-p" class="calc-input" type="number" step="0.1" value="1.0">
            </div>
            <div>
              <label class="calc-label">Reference K(z=0)</label>
              <input id="qkde-kref" class="calc-input" type="number" step="0.01" value="1.0">
            </div>
          </div>

          <div class="calc-action-row">
            <button type="button" class="calc-btn" id="qkde-compute">
              Compute K(z)
            </button>
            <button type="button" class="calc-btn secondary" id="qkde-formula-toggle">
              Show definitions
            </button>
          </div>

          <pre id="qkde-output" class="calc-output" aria-live="polite"></pre>

          <div id="qkde-formulas" class="calc-formula-box" aria-hidden="true">
            <div class="calc-formula-inner">
              <p>
                Parametrized running in e-fold time:
              </p>
              <p>
                \( N = \ln a = -\ln(1+z), \qquad K(N) = 1 + K_0 e^{-pN}. \)
              </p>
              <p>
                At a given redshift z:
                \( K(z) = 1 + K_0 (1+z)^p \).
              </p>
              <p>
                Logarithmic derivative with respect to N:
                \( K'(N)/K(N) = \frac{dK/dN}{K} = \frac{-p K_0 e^{-pN}}{1 + K_0 e^{-pN}}. \)
              </p>
              <p>
                The quantity \(K'(N)/K(N)\) enters directly in the closed background
                system and determines how quickly the kinetic normalization drifts
                as the universe expands.
              </p>
            </div>
          </div>
        </article>
      </div>

      <p class="calc-footnote">
        These calculators are designed for clarity and speed. They reproduce the
        basic background relations and the QKDE running–K parameterization, but
        do not replace a full numerical pipeline for precision forecasting.
      </p>
    </section>
  </div>
</details>
<details id="comparison-qkde">
  <summary><span class="summary-label">Comparing QKDE to Existing Models</span></summary>
  <div class="details-body">

    <p>
      This section places <strong>Quantum–Kinetic Dark Energy (QKDE)</strong> within the full
      dark-energy and modified-gravity theory landscape. Content is organized into nested
      dropdowns: overview, flowchart, comparison matrix, detailed comparisons, and 
      a non-equivalence summary.
    </p>

    <!-- ============================================================
         1. OVERVIEW
    ============================================================ -->
    <details>
      <summary><span class="summary-label">Overview & Theory-Space Position</span></summary>
      <div class="details-body">
        <p>
          QKDE is defined by:
        </p>
        <p style="text-align:center;">
          \( P(X,\phi,t) = K(t)\,X - V(\phi), \qquad K(t) > 0,\quad
          X = -\tfrac12 g^{\mu\nu}\partial_\mu\phi\partial_\nu\phi. \)
        </p>
        <p>
          With an <em>unmodified Einstein–Hilbert sector</em>. In EFT–DE terms:
        </p>
        <ul>
          <li>One scalar degree of freedom.</li>
          <li>\(\alpha_K > 0\) (time-dependent kinetic normalization).</li>
          <li>\(\alpha_B = \alpha_M = \alpha_T = \alpha_H = 0\).</li>
          <li>Canonical perturbations: \(c_s^2 = 1\).</li>
          <li>Metric potentials equal: \(\Phi = \Psi\).</li>
          <li>Luminal gravitational waves: \(c_T^2 = 1\).</li>
        </ul>
        <p>
          All observational effects come from \(H(a)\) and \(D(a)\). QKDE is <em>not</em> modified gravity.
        </p>
      </div>
    </details>

    <!-- ============================================================
         2. FLOWCHART
    ============================================================ -->
    <details>
      <summary><span class="summary-label">Flowchart: Where QKDE Sits in Theory Space</span></summary>
      <div class="details-body">
        <p>This flowchart maps how the late-time acceleration landscape branches:</p>

<pre style="
  background:rgba(0,0,0,0.55);
  padding:20px;
  border-radius:14px;
  overflow-x:auto;
  font-size:0.94rem;
  line-height:1.6;
  border:1px solid rgba(102,252,241,0.28);
  color:#e8faff;
  white-space:pre;
  font-family: Consolas, 'JetBrains Mono', monospace;
">

                         COSMOLOGICAL LATE–TIME ACCELERATION  
                                 (Theory–Space Guide)

                                         ▼
                                         |
        ┌──────────────────────────────────────────────────────────────┐
        │  1. Does the gravitational sector modify Einstein gravity?   │
        └──────────────────────────────────────────────────────────────┘
                           | YES                                  | NO
                           |                                      |
          ┌────────────────────────────────┐        ┌────────────────────────────────┐
          │        MODIFIED GRAVITY        │        │     SCALAR DARK ENERGY IN GR   │
          └────────────────────────────────┘        └────────────────────────────────┘
                           |                                       |
        ┌────────────────────────────────┐        ┌──────────────────────────────────────────┐
        │ f(R), Horndeski, DHOST,        │        │ 2. Is the scalar kinetic term canonical  │
        │ higher-curvature, screening    │        │    (i.e., linear in X with cs² = 1)?     │
        └────────────────────────────────┘        └──────────────────────────────────────────┘
                                                             | YES                | NO
                                                             |                    |
                                        ┌──────────────────────────┐   ┌────────────────────────────┐
                                        │       QUINTESSENCE       │   │          k-ESSENCE         │
                                        │   P = X – V(φ); cs² = 1  │   │  general P(X,φ); cs² ≠ 1   │
                                        └──────────────────────────┘   └────────────────────────────┘
                                                             |
        ┌────────────────────────────────────────────────────────────────────────────────┐
        │ 3. Does the theory introduce a *time-dependent kinetic normalization* K(t),    │
        │    while preserving:                                                           │
        │       • canonical perturbations (cs² = 1),                                     │
        │       • no modified gravity signatures (α_B = α_M = α_T = α_H = 0),            │
        │       • GR-like potentials (Φ = Ψ),                                            │
        │       • luminal tensor speed (c_T² = 1)?                                       │
        └────────────────────────────────────────────────────────────────────────────────┘
                                                             | YES
                                                             |
                                   ┌─────────────────────────────────────────────────┐
                                   │                      QKDE                       │
                                   │    Unique GR-preserving scalar-field sector     │
                                   │    α_K > 0; all other EFT–DE functions = 0      │
                                   │    Dynamics driven by drift of K(t)             │
                                   └─────────────────────────────────────────────────┘

</pre>

        <p>
          This demonstrates: QKDE cannot be reduced to quintessence or k-essence, and 
          cannot arise from modified gravity while retaining GR behavior.
        </p>
      </div>
    </details>

    <!-- ============================================================
         3. COMPARISON MATRIX
    ============================================================ -->
    <details>
      <summary><span class="summary-label">Quick Comparison Matrix</span></summary>
      <div class="details-body">
        <p>A compact structural comparison:</p>

        <table class="symbol-table">
          <thead>
            <tr>
              <th>Model</th>
              <th>Gravity Sector</th>
              <th>Kinetic Structure</th>
              <th>EFT-DE Pattern</th>
              <th>Perturbations</th>
              <th>Driver of Dynamics</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>\(\Lambda\)CDM</td>
              <td>GR</td>
              <td>None</td>
              <td>All \(\alpha_i=0\)</td>
              <td>GR</td>
              <td>\(\Lambda\)</td>
            </tr>
            <tr>
              <td>Quintessence</td>
              <td>GR</td>
              <td>Canonical</td>
              <td>\(\alpha_K\neq0\)</td>
              <td>\(c_s^2=1\)</td>
              <td>Potential</td>
            </tr>
            <tr>
              <td>k-essence</td>
              <td>GR</td>
              <td>General \(P(X,\phi)\)</td>
              <td>Model-dependent</td>
              <td>Often \(c_s^2\neq1\)</td>
              <td>Nonlinear kinetic term</td>
            </tr>
            <tr>
              <td>Horndeski/DHOST</td>
              <td>Modified Gravity</td>
              <td>Higher-derivative</td>
              <td>Multiple \(\alpha_i\)</td>
              <td>Slip + MG</td>
              <td>Curvature mixing</td>
            </tr>
            <tr>
              <td><strong>QKDE</strong></td>
              <td><strong>GR</strong></td>
              <td><strong>Canonical with \(K(t)\)</strong></td>
              <td><strong>\(\alpha_K>0\)</strong></td>
              <td><strong>\(c_s^2=1,\ \Phi=\Psi\)</strong></td>
              <td><strong>Kinetic drift</strong></td>
            </tr>
          </tbody>
        </table>
      </div>
    </details>

    <!-- ============================================================
         4. DETAILED COMPARISONS
    ============================================================ -->
    <details>
      <summary><span class="summary-label">ΛCDM</span></summary>
      <div class="details-body">
        <ul>
          <li>No scalar field.</li>
          <li>No kinetic normalization \(K(t)\).</li>
          <li>Recovered from QKDE when \(K=\mathrm{const}\), \(V=\mathrm{const}\).</li>
        </ul>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">Quintessence</span></summary>
      <div class="details-body">
        <ul>
          <li>Quintessence uses fixed normalization; QKDE uses physical \(K(t)\).</li>
          <li>No quintessence potential can mimic time-varying normalization.</li>
          <li>QKDE’s UV origin (curvature-suppressed \(R X\)) has no analogue.</li>
        </ul>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">k-essence</span></summary>
      <div class="details-body">
        <ul>
          <li>k-essence allows arbitrary \(P(X,\phi)\); QKDE forces linearity in \(X\).</li>
          <li>k-essence changes sound speed; QKDE <em>enforces</em> \(c_s^2 = 1\).</li>
          <li>QKDE’s kinetic drift is derived, not arbitrary.</li>
        </ul>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">Modified Gravity</span></summary>
      <div class="details-body">
        <ul>
          <li>MG changes the Einstein–Hilbert term; QKDE does not.</li>
          <li>MG predicts scale-dependent growth; QKDE does not.</li>
          <li>MG produces slip; QKDE enforces \(\Phi=\Psi\).</li>
        </ul>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">Interacting / Unified Dark Sector</span></summary>
      <div class="details-body">
        <ul>
          <li>No interactions in QKDE.</li>
          <li>No unified dark fluid behavior.</li>
        </ul>
      </div>
    </details>

    <!-- ============================================================
         5. NON-EQUIVALENCE
    ============================================================ -->
    <details>
      <summary><span class="summary-label">Non-Equivalence Summary</span></summary>
      <div class="details-body">
        <ul>
          <li>Not quintessence — \(K(t)\) cannot be absorbed into potential.</li>
          <li>Not k-essence — no nonlinear \(P(X)\), canonical sound speed.</li>
          <li>Not MG — GR remains intact.</li>
          <li>Not interacting DE — no couplings.</li>
          <li>Not unified dark fluid — separate sectors preserved.</li>
        </ul>
      </div>
    </details>

  </div>
</details>
<details id="references-qkde">
  <summary><span class="summary-label">References</span></summary>
  <div class="details-body">

 <ol class="ref-list">

<li><a href="https://doi.org/10.1103/PhysRevLett.119.161101" target="_blank">
B. P. Abbott et al. GW170817: Observation of gravitational waves…
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevLett.119.251303" target="_blank">
Jeremy Sakstein and Bhuvnesh Jain. Implications of the neutron star merger…
</a></li>

<li><a href="https://doi.org/10.1088/1475-7516/2013/02/032" target="_blank">
Giulia Gubitosi et al. The effective field theory of dark energy.
</a></li>

<li><a href="https://doi.org/10.1088/1475-7516/2013/08/010" target="_blank">
Bloomfield et al. Dark energy or modified gravity?
</a></li>

<li><a href="https://doi.org/10.1088/1475-7516/2014/07/050" target="_blank">
Bellini & Sawicki. Maximal freedom at minimum cost.
</a></li>

<li><a href="https://doi.org/10.1016/S0370-2693(99)00602-4" target="_blank">
Garriga & Mukhanov. Perturbations in k-inflation.
</a></li>

<li><a href="https://doi.org/10.1017/CBO9780511622632" target="_blank">
Birrell & Davies. Quantum Fields in Curved Space.
</a></li>

<li><a href="https://doi.org/10.1103/PhysRev.183.1057" target="_blank">
Parker. Particle creation in expanding universes.
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevD.9.341" target="_blank">
Parker & Fulling. Adiabatic regularization…
</a></li>

<li><a href="https://doi.org/10.1088/0305-4470/13/4/022" target="_blank">
Bunch. Renormalized stress tensor in de Sitter space.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/1992eaqg.book.....B" target="_blank">
Buchbinder, Odintsov & Shapiro. Effective Action in Quantum Gravity.
</a></li>

<li><a href="https://doi.org/10.1017/CBO9780511813924" target="_blank">
Parker & Toms. QFT in Curved Spacetime.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/1985PhR...119....1B" target="_blank">
Barvinsky & Vilkovisky. Generalized Schwinger–DeWitt technique.
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevD.50.3874" target="_blank">
Donoghue. GR as an effective field theory.
</a></li>

<li><a href="https://doi.org/10.1086/185100" target="_blank">
Ratra & Peebles. Rolling homogeneous scalar field.
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevLett.80.1582" target="_blank">
Caldwell, Dave & Steinhardt. Cosmological imprint…
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevD.63.103510" target="_blank">
Armendariz-Picon, Mukhanov & Steinhardt. Essentials of k-essence.
</a></li>

<li><a href="https://doi.org/10.1086/176550" target="_blank">
Ma & Bertschinger. Cosmological perturbation theory.
</a></li>

<li><a href="https://doi.org/10.1051/0004-6361/201833910" target="_blank">
Planck Collaboration. Cosmological parameters (2018).
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevD.72.043529" target="_blank">
Linder. Cosmic growth history.
</a></li>

<li><a href="https://doi.org/10.1086/466512" target="_blank">
Eisenstein et al. Detection of the BAO peak.
</a></li>

<li><a href="https://doi.org/10.1088/1126-6708/2008/03/014" target="_blank">
Cheung et al. EFT of Inflation.
</a></li>

<li><a href="https://doi.org/10.1017/CBO9780511790553" target="_blank">
Mukhanov. Physical Foundations of Cosmology.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/2003mc..book.....D" target="_blank">
Dodelson. Modern Cosmology.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/1955tode.book.....C" target="_blank">
Coddington & Levinson. ODE Theory.
</a></li>

<li><a href="https://doi.org/10.12942/lrr-2004-5" target="_blank">
Burgess. Quantum gravity in everyday life.
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevD.92.123516" target="_blank">
Aubourg et al. BAO cosmological implications.
</a></li>

<li><a href="https://doi.org/10.1017/CBO9781139644167" target="_blank">
Weinberg. Quantum Theory of Fields II.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/1995itqf.book.....P" target="_blank">
Peskin & Schroeder. QFT textbook.
</a></li>

<li><a href="https://doi.org/10.1142/S0218271801000822" target="_blank">
Chevallier & Polarski. Scaling dark matter universes.
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevLett.90.091301" target="_blank">
Linder. Expansion history of the universe.
</a></li>

<li><a href="https://doi.org/10.12942/lrr-2010-3" target="_blank">
De Felice & Tsujikawa. f(R) theories.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/2008cosm.book.....W" target="_blank">
Weinberg. Cosmology.
</a></li>

<li><a href="https://doi.org/10.1016/j.physrep.2014.12.002" target="_blank">
Joyce et al. Beyond the standard model.
</a></li>

<li><a href="https://doi.org/10.1088/1361-6633/ab2429" target="_blank">
Kobayashi. Horndeski theory and beyond.
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevLett.114.211101" target="_blank">
Gleyzes et al. Healthy theories beyond Horndeski.
</a></li>

<li><a href="https://doi.org/10.1103/RevModPhys.82.451" target="_blank">
Sotiriou & Faraoni. f(R) theories.
</a></li>

<li><a href="https://doi.org/10.1016/j.physrep.2012.01.001" target="_blank">
Clifton et al. Modified gravity and cosmology.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/1999astro.ph..5116H" target="_blank">
Hogg. Distance measures in cosmology.
</a></li>

<li><a href="https://doi.org/10.1038/281358a0" target="_blank">
Alcock & Paczyński. Evolution-free test…
</a></li>

<li><a href="https://doi.org/10.1086/177989" target="_blank">
Hu & Sugiyama. Small-scale perturbations.
</a></li>

<li><a href="https://doi.org/10.1086/305424" target="_blank">
Eisenstein & Hu. Baryonic features in transfer function.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/1980lssu.book.....P" target="_blank">
Peebles. Large-Scale Structure of the Universe.
</a></li>

<li><a href="https://doi.org/10.1088/1475-7516/2009/10/004" target="_blank">
Song & Percival. Redshift-space distortion parameter.
</a></li>

<li><a href="https://doi.org/10.1086/145870" target="_blank">
Limber. Counts of extragalactic nebulae.
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevD.78.123506" target="_blank">
LoVerde & Afshordi. Extended Limber approximation.
</a></li>

<li><a href="https://doi.org/10.1016/S0370-1573(00)00082-X" target="_blank">
Bartelmann & Schneider. Weak lensing review.
</a></li>

<li><a href="https://doi.org/10.1086/148982" target="_blank">
Sachs & Wolfe. Angular variations of the CMB.
</a></li>

<li><a href="https://doi.org/10.1016/0771-050X(80)90013-3" target="_blank">
Dormand & Prince. Runge–Kutta formulae.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/1993sode.book.....H" target="_blank">
Hairer et al. ODEs I: Nonstiff Problems.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/1983qspa.book.....P" target="_blank">
Piessens et al. QUADPACK.
</a></li>

<li><a href="https://doi.org/10.1086/303939" target="_blank">
Tegmark, Taylor & Heavens. KL eigenmode analysis.
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevLett.79.3806" target="_blank">
Tegmark. Measuring cosmological parameters.
</a></li>

<li><a href="https://doi.org/10.1046/j.1365-8711.2003.06503.x" target="_blank">
Smith et al. Nonlinear matter power spectra.
</a></li>

<li><a href="https://doi.org/10.1088/0004-637X/761/2/152" target="_blank">
Takahashi et al. Revised halofit model.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/1984ucp..book.....W" target="_blank">
Wald. General Relativity.
</a></li>

<li><a href="https://doi.org/10.1143/PTP.76.1036" target="_blank">
Sasaki. Large-scale quantum fluctuations.
</a></li>

<li><a href="https://ui.adsabs.harvard.edu/abs/1988JETP...67.1297M" target="_blank">
Mukhanov. Gauge-invariant perturbations.
</a></li>

<li><a href="https://doi.org/10.1143/PTPS.78.1" target="_blank">
Kodama & Sasaki. Cosmological perturbation theory.
</a></li>

<li><a href="https://doi.org/10.1103/PhysRevD.69.083503" target="_blank">
Bean & Doré. Dark energy speed of sound.
</a></li>

<li><a href="https://doi.org/10.1086/306274" target="_blank">
Hu. Structure formation with generalized dark matter.
</a></li>

<li><a href="https://doi.org/10.1017/CBO9780511750823" target="_blank">
Amendola & Tsujikawa. Dark Energy: Theory & Observations.
</a></li>

</ol>
</div>
</details>
<!-- BEGIN CITE BOX (must stay inside details-body) -->
<!-- ===================== CITE THIS WORK ===================== -->

<div class="cite-box enhanced-cite" id="cite-qkde">
  <div class="cite-header">
    <h3>Cite This Work</h3>
    <p class="cite-subtext">Choose a citation format and copy it directly for your paper, thesis, or project.</p>
  </div>

  <label for="cite-select" class="cite-label">Citation style:</label>
  <select id="cite-select" class="cite-select" onchange="updateCitation()">
    <option value="bibtex">BibTeX</option>
    <option value="apa">APA (7th Edition)</option>
    <option value="mla">MLA (9th Edition)</option>
    <option value="chicago">Chicago (17th Edition)</option>
    <option value="ieee">IEEE</option>
    <option value="harvard">Harvard</option>
  </select>

  <pre id="cite-output" class="cite-text"></pre>

  <div class="cite-buttons">
    <button onclick="copyCitation()" class="paper-button cite-btn">
      Copy to Clipboard
    </button>

   
  </div>
</div>

<script>
function updateCitation() {
  const style = document.getElementById("cite-select").value;
  const output = document.getElementById("cite-output");
  const downloadBib = document.getElementById("download-bib");

  const citations = {
    bibtex: `@misc{brown2025qkde,
  author = {Daniel Brown},
  title = {Quantum–Kinetic Dark Energy (QKDE)},
  year = {2025},
  publisher = {Zenodo},
  doi = {10.5281/zenodo.17774687},
  url = {(https://doi.org/10.5281/zenodo.17774687)}
}`,
    apa: `Brown, D. (2025). *Quantum–Kinetic Dark Energy (QKDE).* Zenodo. https://doi.org/10.5281/zenodo.17757109`,
    mla: `Brown, Daniel. *Quantum–Kinetic Dark Energy (QKDE).* Zenodo, 2025, doi:10.5281/zenodo.17757109.`,
    chicago: `Brown, Daniel. 2025. *Quantum–Kinetic Dark Energy (QKDE).* Zenodo. https://doi.org/10.5281/zenodo.17757109.`,
    ieee: `D. Brown, "Quantum–Kinetic Dark Energy (QKDE)," Zenodo, 2025. doi:10.5281/zenodo.17757109.`,
    harvard: `Brown, D. (2025) “Quantum–Kinetic Dark Energy (QKDE).” Zenodo. doi:10.5281/zenodo.17757109.`
  };

  output.textContent = citations[style];

  // Also update BibTeX downloadable file
  const blob = new Blob([citations.bibtex], { type: 'text/plain' });
  downloadBib.href = URL.createObjectURL(blob);
}

function copyCitation() {
  const citation = document.getElementById("cite-output").textContent;
  navigator.clipboard.writeText(citation);
  
  // Smooth, non-annoying copy notification
  const toast = document.createElement("div");
  toast.className = "toast";
  toast.textContent = "Citation copied!";
  document.body.appendChild(toast);
  setTimeout(() => toast.classList.add("show"), 10);
  setTimeout(() => toast.classList.remove("show"), 2000);
  setTimeout(() => toast.remove(), 2600);
}

document.addEventListener("DOMContentLoaded", updateCitation);
</script>
<script>
  // =============== BASIC NUMERIC HELPERS ===============

  function E_of_z(z, Om, Or, Ol) {
    return Math.sqrt(
      Om * Math.pow(1 + z, 3) +
      Or * Math.pow(1 + z, 4) +
      Ol
    );
  }

  function integrate_chi(H0, Om, Or, Ol, zmax, steps) {
    const c = 299792.458;  // km/s
    const dz = zmax / steps;
    let integral = 0.0;

    for (let i = 0; i <= steps; i++) {
      const z = i * dz;
      const weight = (i === 0 || i === steps) ? 1 : (i % 2 === 0 ? 2 : 4);
      const Ez = E_of_z(z, Om, Or, Ol);
      integral += weight * (1.0 / Ez);
    }

    integral *= dz / 3.0;
    return (c / H0) * integral;  // Mpc
  }

  function setOutput(element, lines, isError = false) {
    if (!element) return;
    element.textContent = lines.join("\n");
    element.classList.toggle("error", isError);
  }

  // =============== FORMULA BOX TOGGLE ===============

  function attachFormulaToggle(buttonId, boxId) {
    const btn = document.getElementById(buttonId);
    const box = document.getElementById(boxId);
    if (!btn || !box) return;

    btn.addEventListener("click", () => {
      const isOpen = box.classList.toggle("is-open");
      box.setAttribute("aria-hidden", isOpen ? "false" : "true");
      btn.textContent = isOpen ? "Hide formulas" : "Show formulas";
      if (buttonId === "qkde-formula-toggle") {
        btn.textContent = isOpen ? "Hide definitions" : "Show definitions";
      }
      if (window.MathJax && window.MathJax.typeset) {
        MathJax.typeset([box]);
      }
    });
  }

  // =============== ΛCDM PRESETS ===============

  function attachLCDMPresets() {
    const card = document.getElementById("lcdm-card");
    if (!card) return;

    const h0El  = document.getElementById("lcdm-h0");
    const omEl  = document.getElementById("lcdm-om");
    const orEl  = document.getElementById("lcdm-or");
    const olEl  = document.getElementById("lcdm-ol");

    const pillButtons = card.querySelectorAll(".calc-pill");

    pillButtons.forEach(btn => {
      btn.addEventListener("click", () => {
        pillButtons.forEach(b => b.classList.remove("is-active"));
        btn.classList.add("is-active");
        const preset = btn.getAttribute("data-preset");

        if (preset === "planck") {
          if (h0El) h0El.value = 67.4;
          if (omEl) omEl.value = 0.315;
          if (orEl) orEl.value = 5e-5;
          if (olEl) olEl.value = 1.0 - parseFloat(omEl.value) - parseFloat(orEl.value);
        } else if (preset === "local") {
          if (h0El) h0El.value = 73.0;
          if (omEl) omEl.value = 0.30;
          if (orEl) orEl.value = 0.0;
          if (olEl) olEl.value = 0.70;
        }
      });
    });
  }

  // =============== QKDE PRESETS ===============

  function attachQKDEPresets() {
    const card = document.getElementById("qkde-card");
    if (!card) return;

    const zEl   = document.getElementById("qkde-z");
    const k0El  = document.getElementById("qkde-k0");
    const pEl   = document.getElementById("qkde-p");
    const krefEl = document.getElementById("qkde-kref");

    const pillButtons = card.querySelectorAll(".calc-pill");

    pillButtons.forEach(btn => {
      btn.addEventListener("click", () => {
        pillButtons.forEach(b => b.classList.remove("is-active"));
        btn.classList.add("is-active");
        const preset = btn.getAttribute("data-qkde-preset");

        if (preset === "mild") {
          if (k0El)  k0El.value  = 0.3;
          if (pEl)   pEl.value   = 0.8;
          if (krefEl) krefEl.value = 1.0;
        } else if (preset === "strong") {
          if (k0El)  k0El.value  = 1.0;
          if (pEl)   pEl.value   = 1.5;
          if (krefEl) krefEl.value = 1.0;
        }
        if (zEl && parseFloat(zEl.value) < 0) zEl.value = 0.0;
      });
    });
  }

  // =============== ΛCDM COMPUTE ===============

  function attachLCDMCompute() {
    const btn = document.getElementById("lcdm-compute");
    const out = document.getElementById("lcdm-output");
    if (!btn || !out) return;

    btn.addEventListener("click", () => {
      const z   = parseFloat(document.getElementById("lcdm-z").value);
      const H0  = parseFloat(document.getElementById("lcdm-h0").value);
      const Om  = parseFloat(document.getElementById("lcdm-om").value);
      const Or  = parseFloat(document.getElementById("lcdm-or").value);
      const Ol  = parseFloat(document.getElementById("lcdm-ol").value);
      const steps = parseInt(document.getElementById("lcdm-steps").value, 10);

      const errors = [];
      if (!(z >= 0)) errors.push("• Redshift z must be ≥ 0.");
      if (!(H0 > 0)) errors.push("• H₀ must be positive.");
      if (!(steps >= 50)) errors.push("• Integration steps should be at least 50.");
      if (Math.abs(Om + Or + Ol - 1.0) > 0.05) {
        errors.push("• For a flat model, Ωm0 + Ωr0 + ΩΛ0 ≈ 1 (current values differ by more than 0.05).");
      }

      if (errors.length > 0) {
        setOutput(out, ["Input error(s):", ""].concat(errors), true);
        return;
      }

      const Ez = E_of_z(z, Om, Or, Ol);
      const Hz = H0 * Ez;

      const chi = integrate_chi(H0, Om, Or, Ol, z, steps);
      const DL = (1 + z) * chi;
      const DA = chi / (1 + z);
      const muSN = 5 * Math.log10(DL) + 25;

      const lines = [];
      lines.push("Input parameters:");
      lines.push(`  z    = ${z.toFixed(3)}`);
      lines.push(`  H₀   = ${H0.toFixed(2)} km/s/Mpc`);
      lines.push(`  Ωm0  = ${Om.toFixed(4)}`);
      lines.push(`  Ωr0  = ${Or.toExponential(2)}`);
      lines.push(`  ΩΛ0  = ${Ol.toFixed(4)}`);
      lines.push(`  steps = ${steps}`);
      lines.push("");
      lines.push("Background (flat ΛCDM):");
      lines.push(`  E(z)     = H(z)/H₀ = ${Ez.toFixed(5)}`);
      lines.push(`  H(z)     = ${Hz.toFixed(2)} km/s/Mpc`);
      lines.push("");
      lines.push("Distances:");
      lines.push(`  χ(z)     = ${chi.toFixed(2)} Mpc  (${(chi/1000).toFixed(3)} Gpc)`);
      lines.push(`  D_A(z)   = ${DA.toFixed(2)} Mpc`);
      lines.push(`  D_L(z)   = ${DL.toFixed(2)} Mpc  (${(DL/1000).toFixed(3)} Gpc)`);
      lines.push(`  μ (SN)   = ${muSN.toFixed(3)} mag`);
      lines.push("");
      lines.push("Notes:");
      lines.push("  • Distances assume a spatially flat geometry.");
      lines.push("  • Radiation can be set ≈0 at low redshift for late-time probes.");
      lines.push("  • Increase step count for higher accuracy at large z.");

      setOutput(out, lines, false);
    });
  }

  // =============== QKDE COMPUTE ===============

  function attachQKDECompute() {
    const btn = document.getElementById("qkde-compute");
    const out = document.getElementById("qkde-output");
    if (!btn || !out) return;

    btn.addEventListener("click", () => {
      const z   = parseFloat(document.getElementById("qkde-z").value);
      const K0  = parseFloat(document.getElementById("qkde-k0").value);
      const p   = parseFloat(document.getElementById("qkde-p").value);
      const Kref = parseFloat(document.getElementById("qkde-kref").value);

      const errors = [];
      if (!(z >= 0)) errors.push("• Redshift z must be ≥ 0.");
      if (isNaN(K0)) errors.push("• K₀ must be a number.");
      if (isNaN(p)) errors.push("• p must be a number.");
      if (isNaN(Kref) || Kref <= 0) errors.push("• Reference K(z=0) must be positive.");

      if (errors.length > 0) {
        setOutput(out, ["Input error(s):", ""].concat(errors), true);
        return;
      }

      const N = -Math.log(1 + z);
      const a = Math.exp(N);

      const K = 1 + K0 * Math.exp(-p * N); // in N
      const dK_dN = -p * K0 * Math.exp(-p * N);
      const Kprime_over_K = dK_dN / K;

      const K_today = 1 + K0;  // at N=0 (z=0)
      const K_ratio_today = K_today / Kref;
      const K_ratio_z = K / Kref;

      const lines = [];
      lines.push("Running-K parameterization:");
      lines.push("  K(N) = 1 + K₀ e^{-pN},   N = ln a = -ln(1+z)");
      lines.push("");
      lines.push("Input:");
      lines.push(`  z       = ${z.toFixed(3)}`);
      lines.push(`  K₀      = ${K0}`);
      lines.push(`  p       = ${p}`);
      lines.push(`  K_ref   = ${Kref}  (reference normalization, e.g. today)`);
      lines.push("");
      lines.push("Derived background quantities:");
      lines.push(`  N(z)    = ${N.toFixed(5)}`);
      lines.push(`  a(z)    = e^N = ${a.toFixed(5)}`);
      lines.push("");
      lines.push("Kinetic normalization:");
      lines.push(`  K(today, z=0)        = 1 + K₀ = ${K_today.toFixed(6)}`);
      lines.push(`  K(z)                 = ${K.toFixed(6)}`);
      lines.push(`  K'(N)/K(N)           = ${Kprime_over_K.toFixed(6)}`);
      lines.push("");
      lines.push("Relative to reference normalization K_ref:");
      lines.push(`  K(today)/K_ref       = ${K_ratio_today.toFixed(6)}`);
      lines.push(`  K(z)/K_ref           = ${K_ratio_z.toFixed(6)}`);
      lines.push("");
      lines.push("Interpretation hints:");
      lines.push("  • The sign and magnitude of K'(N)/K(N) control how quickly");
      lines.push("    the kinetic sector drifts as the universe expands.");
      lines.push("  • Ratios K(z)/K_ref are convenient when matching to");
      lines.push("    observationally normalized EFT parameters.");

      setOutput(out, lines, false);
    });
  }

  // =============== INIT ===============

  document.addEventListener("DOMContentLoaded", () => {
    attachFormulaToggle("lcdm-formula-toggle", "lcdm-formulas");
    attachFormulaToggle("qkde-formula-toggle", "qkde-formulas");

    attachLCDMPresets();
    attachQKDEPresets();

    attachLCDMCompute();
    attachQKDECompute();
  });
</script>
<footer class="site-footer">
  © 2025 Daniel Brown — Quantum–Kinetic Dark Energy (QKDE)
</footer>
</div> <!-- end page -->

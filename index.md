---
layout: none
title: Quantum–Kinetic Dark Energy (QKDE)
---

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Quantum–Kinetic Dark Energy (QKDE)</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />

  <!-- MathJax -->
  <script>
    window.MathJax = { tex: { inlineMath: [['$','$'], ['\\(','\\)']] } };
  </script>
  <script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

  <style>
    [id] {
      scroll-margin-top: 90px;
    }

    html {
      scroll-behavior: smooth;
    }

    /* Starfield layers (static) */
    .star-layer {
      position: fixed;
      inset: 0;
      pointer-events: none;
      background: radial-gradient(circle at 20% 20%, rgba(255,255,255,0.14) 0, transparent 55%),
                  radial-gradient(circle at 80% 60%, rgba(255,255,255,0.10) 0, transparent 55%);
      mix-blend-mode: screen;
      opacity: 0.35;
      z-index: -1;
    }

    /* ============= NAVBAR ============= */

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

    /* ============= PAGE + GLOBAL ============= */

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

    hr {
      border: none;
      height: 1px;
      background: linear-gradient(to right, transparent, #568ea6, transparent);
      margin: 45px 0;
    }

    .center {
      text-align: center;
    }

    /* ============= AUTHOR BOX ============= */

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

    /* ============= SOCIAL LINKS ============= */

    .social-box {
      background: rgba(15, 22, 32, 0.45);
      padding: 18px 25px;
      border-radius: 12px;
      border: 1px solid rgba(102,252,241,0.10);
      margin-top: 25px;
    }

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

    /* ============= PAPER BOX + BUTTONS ============= */

    .paper-box {
      background: rgba(15, 22, 32, 0.45);
      padding: 30px;
      border-radius: 14px;
      border: 1px solid rgba(102,252,241,0.10);
      box-shadow: 0 0 20px rgba(102,252,241,0.12);
    }

    .paper-button {
      display: inline-block;
      padding: 12px 28px;
      background: #d2f2ff;
      color: #0b0c10;
      font-size: 1.05rem;
      border-radius: 7px;
      text-decoration: none;
      transition: 0.2s;
      border: none;
      cursor: pointer;
    }

    .paper-button:hover {
      background: #bfe6f7;
      box-shadow: 0 0 16px rgba(174,234,255,0.8);
    }

    /* ============= DETAILS / DROPDOWNS ============= */

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

    /* ============= SYMBOL TABLE & COMPARISON TABLES ============= */

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

    /* ============= REFERENCES LIST ============= */

    .ref-list {
      margin: 0;
      padding-left: 22px;
      font-size: 0.92rem;
      color: #ffffff;
    }

    .ref-list li {
      margin-bottom: 6px;
      color: #ffffff;
    }

    .ref-list a {
      color: #ffffff;
      text-decoration: none;
      transition: color 0.25s ease, text-shadow 0.25s ease;
    }

    .ref-list a:hover {
      color: #9bd8ff;
      text-shadow: 0 0 6px rgba(140,200,255,0.8);
    }

    /* ============= CITE BOX ============= */

    .cite-box {
      margin-top: 40px;
      background: rgba(15, 22, 32, 0.55);
      border: 1px solid rgba(102, 252, 241, 0.12);
      border-radius: 12px;
      padding: 20px 25px;
      box-shadow: 0 0 20px rgba(102,252,241,0.12);
    }

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
      color: #b9ecff;
      font-family: "Merriweather", serif;
      font-weight: 300;
    }

    .cite-subtext {
      color: #c9e6f8;
      font-size: 0.9rem;
      opacity: 0.8;
      margin-top: 0;
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

    .cite-select:hover {
      border-color: rgba(102,252,241,0.40);
      cursor: pointer;
    }

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
      white-space: pre-wrap;
    }

    .cite-buttons {
      margin-top: 14px;
      display: flex;
      gap: 14px;
    }

    .alt-cite-btn {
      background: #c8f5ff;
    }

    .alt-cite-btn:hover {
      background: #aee8f7;
    }

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

    /* ============= CALCULATOR STYLES ============= */

    .calc-grid {
      margin-top: 18px;
      display: flex;
      flex-wrap: wrap;
      gap: 22px;
    }

    @media (max-width: 780px) {
      .calc-grid {
        flex-direction: column;
      }
    }

    .calc-card {
      flex: 1 1 260px;
      background: rgba(15, 22, 32, 0.68);
      border-radius: 14px;
      border: 1px solid rgba(102, 252, 241, 0.18);
      padding: 18px 20px 20px;
      box-shadow: 0 0 18px rgba(102, 252, 241, 0.12);
      position: relative;
      overflow: hidden;
      transition: transform 0.18s ease, box-shadow 0.18s ease, border-color 0.18s ease;
    }

    .calc-card::before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      height: 3px;
      width: 100%;
      background: linear-gradient(to right, rgba(102,252,241,0.7), rgba(69,160,201,0.5), rgba(102,252,241,0.7));
      opacity: 0.7;
    }

    .calc-card:hover {
      transform: translateY(-2px);
      box-shadow: 0 0 24px rgba(102, 252, 241, 0.25);
      border-color: rgba(102, 252, 241, 0.28);
    }

    .calc-card-header {
      display: flex;
      align-items: baseline;
      justify-content: space-between;
      gap: 10px;
      margin-bottom: 6px;
    }

    .calc-card-header h3 {
      margin: 0;
      font-size: 1.05rem;
    }

    .calc-tag {
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      padding: 2px 8px;
      border-radius: 999px;
      border: 1px solid rgba(160, 220, 255, 0.45);
      background: rgba(8, 18, 28, 0.9);
      color: #aeeaff;
      white-space: nowrap;
    }

    .calc-note {
      font-size: 0.83rem;
      opacity: 0.85;
      margin-top: 4px;
      margin-bottom: 10px;
    }

    .calc-label {
      display: block;
      font-size: 0.83rem;
      margin-top: 8px;
      margin-bottom: 2px;
      color: #c5f2ff;
    }

    .calc-input-row {
      display: grid;
      grid-template-columns: 1.1fr 1fr;
      gap: 8px 10px;
    }

    @media (max-width: 500px) {
      .calc-input-row {
        grid-template-columns: 1fr;
      }
    }

    .calc-input {
      width: 100%;
      padding: 6px 8px;
      border-radius: 6px;
      border: 1px solid rgba(120, 160, 190, 0.7);
      background: rgba(5, 10, 18, 0.8);
      color: #e8e9ef;
      font-size: 0.9rem;
      box-sizing: border-box;
    }

    .calc-input::placeholder {
      color: rgba(200, 215, 235, 0.55);
      font-size: 0.8rem;
    }

    .calc-input:focus {
      outline: none;
      border-color: rgba(102, 252, 241, 0.95);
      box-shadow: 0 0 8px rgba(102, 252, 241, 0.7);
    }

    .calc-output {
      margin-top: 12px;
      font-family: "JetBrains Mono", "Menlo", "Consolas", monospace;
      font-size: 0.8rem;
      background: rgba(0, 0, 0, 0.55);
      border-radius: 8px;
      padding: 10px 12px;
      border: 1px solid rgba(120, 160, 190, 0.4);
      max-height: 190px;
      overflow-y: auto;
      white-space: pre-wrap;
    }

    .calc-output.error {
      border-color: rgba(255, 120, 120, 0.7);
      color: #ffd9d9;
    }

    .calc-btn {
      margin-top: 14px;
      font-size: 0.9rem;
      padding: 9px 18px;
    }

    .calc-footnote {
      margin-top: 20px;
      font-size: 0.9rem;
      opacity: 0.9;
    }

    .calc-divider {
      margin: 10px 0;
      height: 1px;
      background: linear-gradient(to right, transparent, rgba(120,160,200,0.7), transparent);
      border: none;
    }

    /* ============= FOOTER ============= */

    .site-footer {
      margin-top: 55px;
      text-align: center;
      font-size: 0.85rem;
      color: #a8c3d9;
      opacity: 0.8;
      padding-top: 20px;
      border-top: 1px solid rgba(102,252,241,0.10);
    }
  </style>
</head>
<body>
  <!-- Star layers -->
  <div class="star-layer"></div>
  <div class="star-layer"></div>
  <div class="star-layer"></div>

  <a id="top"></a>

  <div class="page">
    <nav class="nav-header" aria-label="Main navigation">
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

    <h1>Quantum–Kinetic Dark Energy (QKDE)</h1>
    <p style="text-align:center; margin-top:-10px; font-style: italic;">
      An effective dark energy framework with the Einstein–Hilbert metric sector intact and a time-dependent scalar kinetic normalization
    </p>

    <div class="author-box">
      <img src="photoDaniel.jpg" alt="Author photo" class="author-photo" />
      <div>
        <h2>Daniel Brown</h2>
        <p>Independent researcher exploring dark energy, scalar-field physics, and cosmic expansion through effective field theory and first-principles modeling.</p>
        <p>Graduate of the University of Utah and resident of Salt Lake City, Utah.</p>
        <p>Author of the monograph <em>Quantum–Kinetic Dark Energy</em>, a revision and expansion of the earlier Scalar-Cost Dark Energy framework.</p>
        <p>My work aims to clarify minimal, GR-consistent explanations of late-time acceleration while developing reproducible numerical tools and observational tests.</p>
      </div>
    </div>

    <div class="social-box">
      <a href="https://orcid.org/0009-0001-8082-9702" class="social-link" target="_blank" rel="noopener noreferrer">
        <span class="social-icon">
          <img src="ORCID_iD.svg.png" alt="ORCID logo" />
        </span>
        <span>ORCiD</span>
      </a>

      <a href="https://github.com/DanielBrown124/QKDE" class="social-link" target="_blank" rel="noopener noreferrer">
        <span class="social-icon">
          <svg viewBox="0 0 24 24" aria-hidden="true">
            <path d="M12 1.5A10.5 10.5 0 0 0 1.5 12c0 4.63 3 8.56 7.17 9.95.53.1.73-.23.73-.5v-1.75c-2.92.64-3.54-1.4-3.54-1.4-.48-1.2-1.17-1.52-1.17-1.52-.96-.65.07-.63.07-.63 1.06.08 1.62 1.1 1.62 1.1.95 1.63 2.5 1.16 3.11.89.1-.7.37-1.16.68-1.43-2.33-.27-4.78-1.18-4.78-5.25 0-1.16.42-2.1 1.1-2.84-.11-.27-.48-1.36.1-2.83 0 0 .9-.29 2.95 1.08a10.1 10.1 0 0 1 5.38 0c2.05-1.37 2.95-1.08 2.95-1.08.58 1.47.21 2.56.1 2.83.68.74 1.1 1.68 1.1 2.84 0 4.08-2.45 4.98-4.79 5.25.38.33.73.97.73 1.96v2.9c0 .27.2.6.73.5A10.52 10.52 0 0 0 22.5 12 10.5 10.5 0 0 0 12 1.5Z" />
          </svg>
        </span>
        <span>GitHub Repository</span>
      </a>

      <a href="https://doi.org/10.5281/zenodo.17757109" class="social-link" target="_blank" rel="noopener noreferrer">
        <span class="social-icon">
          <img src="zenodo.ico" alt="Zenodo logo" />
        </span>
        <span>Zenodo</span>
      </a>

      <a href="https://independent.academia.edu/DanielBrown462" class="social-link" target="_blank" rel="noopener noreferrer">
        <span class="social-icon">
          <img src="academia.png" alt="Academia.edu logo" />
        </span>
        <span>Academia</span>
      </a>

      <a href="https://www.researchgate.net/profile/Daniel-Brown-133?ev=hdr_xprf" class="social-link" target="_blank" rel="noopener noreferrer">
        <span class="social-icon">
          <img src="ResearchGate.png" alt="ResearchGate logo" />
        </span>
        <span>ResearchGate</span>
      </a>
    </div>

    <hr />

    <div class="center" style="margin-top: 35px;">
      <a class="paper-button" href="QKDE_v.3F.pdf">
        QKDE Paper (PDF)
      </a>
    </div>

    <!-- REVIEWER GUIDE -->
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

        <h3>1. What QKDE Claims</h3>
        <ul>
          <li><strong>QKDE is a single-scalar, GR-preserving dark-energy framework</strong> with no modification to the Einstein–Hilbert metric sector.</li>
          <li><strong>Cosmic acceleration arises entirely from a scalar sector</strong> of the form \(P(X,\phi,t) = K(t)X - V(\phi)\), where the <em>kinetic normalization</em> \(K(t) > 0\) drifts slowly in time.</li>
          <li><strong>All EFT–DE gravitational functions vanish</strong> except \(\alpha_K = K\dot{\phi}^2/(H^2 M_{\rm pl}^2) > 0\):<br /><code>α_B = α_M = α_T = α_H = 0</code>.</li>
          <li><strong>Gravitational waves are luminal</strong> (\(c_T^2 = 1\)), the <strong>Planck mass is constant</strong>, and <strong>metric potentials satisfy</strong> \(\Phi = \Psi\).</li>
          <li><strong>The linear growth equation is exactly GR</strong>: all deviations enter only through the background expansion history \(H(a)\).</li>
          <li><strong>The model is falsifiable</strong>: \(\mu(a,k)=\Sigma(a,k)=1,\;\eta(a,k)=0\) on linear scales. Any statistically significant deviation excludes QKDE.</li>
        </ul>

        <h3>2. What QKDE Does <em>Not</em> Claim</h3>
        <ul>
          <li>It does <strong>not</strong> modify gravity, introduce an evolving Planck mass, or alter light deflection.</li>
          <li>It does <strong>not</strong> introduce scale-dependent growth, screening mechanisms, sound speeds \(c_s^2 \neq 1\), or higher-derivative operators.</li>
          <li>It does <strong>not</strong> attempt to solve the cosmological constant problem.</li>
          <li>It does <strong>not</strong> rely on phenomenological templates; all equations come from the covariant action and the EFT mapping.</li>
          <li>It does <strong>not</strong> introduce extra degrees of freedom beyond the single scalar.</li>
        </ul>

        <h3>3. Why QKDE Is Not Quintessence</h3>
        <ul>
          <li>Quintessence uses <strong>fixed canonical normalization</strong>: \(P(X,\phi)=X-V(\phi)\).</li>
          <li>QKDE uses <strong>time-dependent kinetic normalization</strong> \(K(t)X\), motivated by curvature-suppressed operators and integrating out heavy fields in QFT in curved spacetime.</li>
          <li>Quintessence variations affect \(V(\phi)\); QKDE variations occur in \(K(t)\).</li>
          <li>Quintessence has <strong>no operator-level EFT derivation for a running kinetic term</strong>; QKDE explicitly builds this in from the UV-motivated operator \(R X\).</li>
        </ul>

        <h3>4. Why QKDE Is Not k-Essence</h3>
        <ul>
          <li>k-essence allows broad functional freedom: \(P(X,\phi)\).</li>
          <li>QKDE is a <strong>highly constrained subset</strong>:<br /><code>P = K(t)X - V(φ)</code> with no higher powers of \(X\) and no noncanonical speeds.</li>
          <li>Generic k-essence yields <strong>non-unit sound speeds</strong>; QKDE enforces \(c_s^2 = 1\) exactly.</li>
          <li>k-essence can generate <strong>scale-dependent growth</strong>; QKDE predicts GR-like, scale-independent growth.</li>
          <li>QKDE’s drift \(K(t)\) is <strong>time-only</strong>, unlike general k-essence dependence on both \(X\) and \(\phi\).</li>
        </ul>

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

    <!-- WHAT THIS WORK PROPOSES -->
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

      <hr />

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

      <hr />

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

      <hr />

      <h3>4. EFT of Dark Energy characterization</h3>
      <p>
        In the Effective Field Theory of Dark Energy (EFT–DE) language, QKDE is characterized by a single active background function:
      </p>
      \[
        \alpha_K > 0,
      \]
      <p>while</p>
      \[
        \alpha_B = \alpha_M = \alpha_T = \alpha_H = 0.
      \]
      <p>
        This enforces luminal tensors, a constant Planck mass, no braiding, and no beyond-Horndeski structure, keeping the gravitational sector strictly Einsteinian at the linear level.
      </p>

      <hr />

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
        which corresponds to
        \(
          K(N) = 1 + K_0 e^{-pN}
        \)
        with \( N = \ln a = -\ln(1+z) \), giving a simple analytic form for
        \(K'/K\) and enabling rapid exploration of parameter space.  
        Both realizations plug directly into the closed background system without requiring numerical iteration.
      </p>
    </div>

    <!-- SYMBOL INDEX -->
    <h2 id="symbol-index">Symbol Index</h2>
    <details>
      <summary><span class="summary-label">View symbol table</span></summary>
      <div class="details-body">
        <table class="symbol-table">
          <thead>
            <tr>
              <th>Symbol</th>
              <th>Meaning</th>
              <th>Notes</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>\(a(t)\)</td>
              <td>Scale factor</td>
              <td>Normalized to 1 today</td>
            </tr>
            <tr>
              <td>\(N = \ln a\)</td>
              <td>E-fold time</td>
              <td>Derivatives: \( f' = df/dN \)</td>
            </tr>
            <tr>
              <td>\(H = \dot{a}/a\)</td>
              <td>Hubble rate</td>
              <td>Key dynamical variable</td>
            </tr>
            <tr>
              <td>\(E = H'/H\)</td>
              <td>Dimensionless Hubble derivative</td>
              <td>Relates to \(w_{\rm eff}\)</td>
            </tr>
            <tr>
              <td>\(R\)</td>
              <td>Ricci scalar</td>
              <td>\(R = 6H^2(2+E)\) (FRW)</td>
            </tr>
            <tr>
              <td>\(X\)</td>
              <td>Kinetic term</td>
              <td>\(X = \frac12 H^2 s^2\) in FRW</td>
            </tr>
            <tr>
              <td>\(K(t)\)</td>
              <td>Kinetic normalization</td>
              <td>Time-dependent in QKDE</td>
            </tr>
            <tr>
              <td>\(\alpha_K\)</td>
              <td>EFT kinetic function</td>
              <td>\(\alpha_K = K\dot{\phi}^2/(H^2 M_{\rm pl}^2)\)</td>
            </tr>
            <tr>
              <td>\(\Phi,\Psi\)</td>
              <td>Metric potentials</td>
              <td>\(\Phi=\Psi\) in QKDE</td>
            </tr>
          </tbody>
        </table>
      </div>
    </details>

    <!-- DERIVATIONS -->
    <details id="derivations">
      <summary><span class="summary-label">Derivations</span></summary>
      <div class="details-body">

        <p>
          Below is a streamlined, reader-friendly version of the full analytic derivations in the QKDE monograph:
          background system, curvature-based identities, kinetic normalization, perturbations, growth equations,
          and stability conditions. Each expression matches those in the PDF exactly.
        </p>

        <h3>1. Closed Background System</h3>
        <p>E-fold time: \( N = \ln a \), with \( f' = H^{-1}\dot{f} \).</p>

        \[
          \phi' = s,
        \]
        \[
          s' = -(3+E)s - \frac{K'}{K}s - \frac{V_{,\phi}}{H^2 K},
        \]
        \[
          E = \frac{H'}{H}.
        \]

        <h3>2. Ricci Scalar</h3>

        \[
          R = 6H^2(2+E)
        \]
        \[
          \frac{R'}{R} = 2E + \frac{E'}{2+E}.
        \]

        <h3>3. Curvature-Induced \(K'/K\)</h3>

        \[
          K = 1 + \frac{\alpha R}{M^2},
        \]

        \[
          \frac{K'}{K} = 
          \frac{\alpha R}{M^2 + \alpha R}
          \left(
            2E + \frac{E'}{2+E}
          \right).
        \]

        <h3>4. Scalar Energy & Pressure</h3>

        \[
          \rho_\phi = KX + V, \qquad p_\phi = KX - V.
        \]

        <h3>5. Perturbation Structure</h3>

        \[
          c_s^2 = 1,\qquad
          \Phi = \Psi,\qquad
          \mu = \Sigma = 1,\qquad
          \eta = 0.
        \]

        <h3>6. GR Growth Equation</h3>

        \[
          D'' + (2 + E) D' - \frac{3}{2}\Omega_m D = 0.
        \]

        <h3>7. Stability</h3>

        \[
          K(t) > 0,\qquad
          c_s^2 > 0,\qquad
          M^2 + \alpha R \neq 0.
        \]
      </div>
    </details>

    <!-- CALCULATOR -->
    <details id="calculator">
      <summary><span class="summary-label">Interactive Calculator</span></summary>
      <div class="details-body">

        <p>
          These browser-side calculators provide intuition for ΛCDM background quantities and the behavior of a running kinetic normalization in QKDE.
          They use correct formulas and stable numerical integration. For full-precision forecasts, see the Python scripts in the GitHub repository.
        </p>

        <div class="calc-grid">

          <!-- ΛCDM CALC CARD -->
          <div class="calc-card">
            <div class="calc-card-header">
              <h3>ΛCDM Background & Distances</h3>
              <span class="calc-tag">Reference</span>
            </div>
            <p class="calc-note">
              Uses exact Friedmann equation and Simpson integration.
            </p>

            <label class="calc-label">Redshift \(z\)</label>
            <input id="lcdm-z" class="calc-input" type="number" value="0.5" step="0.01">

            <label class="calc-label">\(H_0\) [km/s/Mpc]</label>
            <input id="lcdm-h0" class="calc-input" type="number" value="70">

            <label class="calc-label">\(\Omega_{m0}\)</label>
            <input id="lcdm-om" class="calc-input" type="number" value="0.3" step="0.01">

            <label class="calc-label">\(\Omega_{r0}\)</label>
            <input id="lcdm-or" class="calc-input" type="number" value="0.0" step="1e-5">

            <label class="calc-label">\(\Omega_{\Lambda0}\)</label>
            <input id="lcdm-ol" class="calc-input" type="number" value="0.7" step="0.01">

            <label class="calc-label">Integration steps</label>
            <input id="lcdm-steps" class="calc-input" type="number" value="400">

            <button id="lcdm-button" class="paper-button calc-btn">Compute ΛCDM</button>
            <pre id="lcdm-output" class="calc-output"></pre>
          </div>

          <!-- QKDE K(N) VISUALIZER -->
          <div class="calc-card">
            <div class="calc-card-header">
              <h3>QKDE Running–\(K(t)\) Visualizer</h3>
              <span class="calc-tag">Model</span>
            </div>
            <p class="calc-note">
              Shows the drift of the kinetic normalization for \(K(N) = 1 + K_0 e^{-pN}\).
            </p>

            <label class="calc-label">Redshift \(z\)</label>
            <input id="qkde-z" class="calc-input" type="number" value="0.5" step="0.01">

            <label class="calc-label">\(K_0\)</label>
            <input id="qkde-k0" class="calc-input" type="number" value="0.5">

            <label class="calc-label">\(p\)</label>
            <input id="qkde-p" class="calc-input" type="number" value="1.0">

            <button id="qkde-button" class="paper-button calc-btn">Compute K(z)</button>
            <pre id="qkde-output" class="calc-output"></pre>
          </div>

        </div> <!-- end calc-grid -->

        <p class="calc-footnote">
          These tools provide intuition only; the full QKDE pipeline (background ODEs, sensitivity equations, forecasts)
          is implemented in Python and available on GitHub.
        </p>
      </div>
    </details>
        <!-- COMPARISON SECTION -->
    <h2 id="comparison-qkde">Comparison to Existing Models</h2>

    <details>
      <summary><span class="summary-label">ΛCDM vs QKDE</span></summary>
      <div class="details-body">
        <p>
          ΛCDM is recovered in the limit of a constant kinetic normalization and
          a cosmological constant:
        </p>
        \[
          K(t) \to 1,\qquad V(\phi) \to \Lambda = \text{const.}
        \]
        <p>
          In this limit the scalar sector is equivalent to an effective cosmological constant with
          no additional dynamics. QKDE generalizes this by allowing \(K(t)\) to drift slowly in time,
          while keeping the Einstein–Hilbert sector <em>identical</em> to that of ΛCDM.
        </p>
        <ul>
          <li><strong>Same:</strong> Einstein–Hilbert action, luminal GWs, constant \(M_{\rm pl}\), GR growth equation.</li>
          <li><strong>Different:</strong> Effective dark-energy equation of state and background history \(H(a)\)
              driven by \(K(t)\) rather than by a fixed \(\Lambda\).</li>
        </ul>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">Quintessence vs QKDE</span></summary>
      <div class="details-body">
        <p>
          Quintessence is characterized by a canonical scalar:
        </p>
        \[
          P_{\rm quint}(X,\phi) = X - V(\phi).
        \]
        <p>
          QKDE replaces the fixed normalization of \(X\) with a controlled, mildly time-dependent
          prefactor \(K(t)\):
        </p>
        \[
          P_{\rm QKDE}(X,\phi,t) = K(t)X - V(\phi), \qquad K(t) > 0.
        \]
        <ul>
          <li>Quintessence variations live almost entirely in the potential \(V(\phi)\).</li>
          <li>QKDE variations live in \(K(t)\), motivated by curvature-suppressed operators and heavy-field integration.</li>
          <li>Both preserve GR, luminal GWs, and a single scalar degree of freedom.</li>
        </ul>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">k-Essence vs QKDE</span></summary>
      <div class="details-body">
        <p>
          k-essence admits a broad functional dependence:
        </p>
        \[
          P_{\rm k\text{-}ess}(X,\phi) = F(X,\phi),
        \]
        <p>
          often involving higher powers of \(X\), leading to nontrivial sound speeds and
          potentially scale-dependent growth.
        </p>
        <p>
          QKDE is a tightly constrained subset:
        </p>
        \[
          P_{\rm QKDE}(X,\phi,t) = K(t)X - V(\phi),
        \]
        <ul>
          <li>No higher powers of \(X\).</li>
          <li>Exact luminal scalar sound speed: \(c_s^2 = 1\).</li>
          <li>No additional EFT–DE functions beyond \(\alpha_K\).</li>
          <li>Linear perturbations remain strictly GR-like; only the background \(H(a)\) is deformed.</li>
        </ul>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">Modified Gravity / Horndeski vs QKDE</span></summary>
      <div class="details-body">
        <p>
          Many modified-gravity and Horndeski/beyond-Horndeski models are characterized by
          additional EFT–DE functions:
        </p>
        \[
          \alpha_M,\; \alpha_B,\; \alpha_T,\; \alpha_H \neq 0,
        \]
        <p>
          introducing evolving Planck mass, braiding, modified GW speed, or higher-derivative
          curvature couplings.
        </p>
        <p>
          QKDE sits in the GR-preserving corner:
        </p>
        \[
          \alpha_B = \alpha_M = \alpha_T = \alpha_H = 0,\qquad \alpha_K > 0.
        \]
        <ul>
          <li>Metric sector is exactly Einsteinian.</li>
          <li>No extra forces or screened regimes at linear order.</li>
          <li>Any observed departure from \(\mu=\Sigma=1\) or \(\eta=0\) would falsify QKDE.</li>
        </ul>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">Early Dark Energy & Interacting DE vs QKDE</span></summary>
      <div class="details-body">
        <p>
          Early dark energy (EDE) and interacting dark-energy models typically:
        </p>
        <ul>
          <li>Introduce non-negligible dark-energy fractions at recombination,</li>
          <li>or couple the dark-energy sector directly to dark matter or other fields.</li>
        </ul>
        <p>
          QKDE, as developed in the monograph, does not introduce explicit dark-sector couplings,
          and is designed primarily as a late-time, GR-respecting effective framework.
          The kinetic drift \(K(t)\) is constructed so that standard early-time physics
          (BBN, CMB decoupling) is preserved in the simplest realizations.
        </p>
      </div>
    </details>

    <!-- REFERENCES -->
    <h2 id="references-qkde">Selected References</h2>
    <ol class="ref-list">
      <li>
        Cheung, C., Creminelli, P., Fitzpatrick, A. L., Kaplan, J., &amp; Senatore, L.,
        “The Effective Field Theory of Inflation,”
        <em>JHEP</em> <strong>03</strong> (2008) 014.
      </li>
      <li>
        Gubitosi, G., Piazza, F., &amp; Vernizzi, F.,
        “The Effective Field Theory of Dark Energy,”
        <em>JCAP</em> <strong>02</strong> (2013) 032.
      </li>
      <li>
        Bloomfield, J., Flanagan, É. É., Park, M., &amp; Watson, S.,
        “Dark energy or modified gravity? An effective field theory approach,”
        <em>JCAP</em> <strong>08</strong> (2013) 010.
      </li>
      <li>
        Bellini, E., &amp; Sawicki, I.,
        “Maximal freedom at minimum cost: linear large-scale structure in general
        modifications of gravity,”
        <em>JCAP</em> <strong>07</strong> (2014) 050.
      </li>
      <li>
        Mukhanov, V.,
        <em>Physical Foundations of Cosmology</em>,
        Cambridge University Press (2005).
      </li>
      <li>
        Dodelson, S.,
        <em>Modern Cosmology</em>,
        Academic Press (2003).
      </li>
      <li>
        Barvinsky, A. O., &amp; Vilkovisky, G. A.,
        “The Generalized Schwinger–DeWitt Technique in Gauge Theories and Quantum Gravity,”
        <em>Phys. Rept.</em> <strong>119</strong> (1985) 1.
      </li>
      <!-- Your QKDE monograph reference -->
      <li>
        Brown, D.,
        “Quantum–Kinetic Dark Energy,”
        Zenodo (2025). DOI: <a href="https://doi.org/10.5281/zenodo.17757109" target="_blank" rel="noopener noreferrer">
        10.5281/zenodo.17757109</a>.
      </li>
    </ol>

    <!-- CITE BOX -->
    <h2 id="cite-qkde">How to Cite QKDE</h2>

    <div class="enhanced-cite">
      <div class="cite-header">
        <h3>Citation Helper</h3>
        <p class="cite-subtext">
          Select a format and copy the citation text. All formats refer to the same monograph.
        </p>
      </div>

      <label for="cite-format" class="cite-label">Citation format</label>
      <select id="cite-format" class="cite-select">
        <option value="bibtex">BibTeX</option>
        <option value="ads">ADS-style</option>
        <option value="plain">Plain text</option>
      </select>

      <pre id="cite-text" class="cite-text"></pre>

      <div class="cite-buttons">
        <button id="copy-cite" class="paper-button">Copy citation</button>
        <button id="copy-doi" class="paper-button alt-cite-btn">Copy DOI only</button>
      </div>
    </div>

    <footer class="site-footer">
      <p>
        &copy; <span id="year-span"></span> Daniel Brown. All rights reserved.
      </p>
      <p>
        Built for transparency, reproducibility, and constructive criticism.
        <a href="#top" style="color:#c5f2ff; text-decoration:none;">Back to top ↑</a>
      </p>
    </footer>
  </div> <!-- end .page -->

  <!-- Toast notification -->
  <div id="toast" class="toast">Copied to clipboard</div>

  <!-- JavaScript -->
  <script>
    // ===== Utility: Toast =====
    function showToast(message) {
      const toast = document.getElementById("toast");
      if (!toast) return;
      toast.textContent = message;
      toast.classList.add("show");
      setTimeout(() => {
        toast.classList.remove("show");
      }, 2200);
    }

    // ===== Year in footer =====
    (function setYear() {
      const span = document.getElementById("year-span");
      if (span) {
        span.textContent = new Date().getFullYear();
      }
    })();

    // ===== Citation Helper =====
    const citeTextEl = document.getElementById("cite-text");
    const citeSelectEl = document.getElementById("cite-format");
    const copyCiteBtn = document.getElementById("copy-cite");
    const copyDoiBtn  = document.getElementById("copy-doi");

    const DOI = "10.5281/zenodo.17757109";

    const citations = {
      bibtex:
`@misc{Brown_QKDE_2025,
  author       = {Daniel Brown},
  title        = {Quantum--Kinetic Dark Energy},
  year         = {2025},
  publisher    = {Zenodo},
  doi          = {${DOI}},
  url          = {https://doi.org/${DOI}}
}`,
      ads:
"Brown, D., 2025, “Quantum–Kinetic Dark Energy,” Zenodo, doi:" + DOI,
      plain:
"Daniel Brown, \"Quantum–Kinetic Dark Energy,\" Zenodo (2025). DOI: " + DOI + "."
    };

    function updateCitation() {
      if (!citeTextEl || !citeSelectEl) return;
      const fmt = citeSelectEl.value || "bibtex";
      citeTextEl.textContent = citations[fmt] || citations.bibtex;
    }

    if (citeSelectEl) {
      citeSelectEl.addEventListener("change", updateCitation);
      // initialize
      updateCitation();
    }

    async function copyTextToClipboard(text) {
      try {
        await navigator.clipboard.writeText(text);
        showToast("Copied to clipboard");
      } catch (err) {
        console.error("Clipboard copy failed:", err);
        showToast("Unable to copy");
      }
    }

    if (copyCiteBtn && citeTextEl) {
      copyCiteBtn.addEventListener("click", () => {
        copyTextToClipboard(citeTextEl.textContent.trim());
      });
    }

    if (copyDoiBtn) {
      copyDoiBtn.addEventListener("click", () => {
        copyTextToClipboard(DOI);
      });
    }
<script>
/* ============================================================
   ΛCDM CALCULATOR LOGIC
   ------------------------------------------------------------
   Computes background quantities (H(z), distances, w_eff, q)
   using correct FRW relations and Simpson integration.
   ============================================================ */

function E_LCDM(z, Om, Or, Ol) {
  return Math.sqrt(
    Om * Math.pow(1 + z, 3) +
    Or * Math.pow(1 + z, 4) +
    Ol
  );
}

function integrate_chi(H0, Om, Or, Ol, zmax, steps) {
  const c = 299792.458; // km/s
  const N = (steps % 2 === 0 ? steps : steps + 1);
  const dz = zmax / N;

  let S = 0;
  for (let i = 0; i <= N; i++) {
    const z = i * dz;
    const w = (i === 0 || i === N) ? 1 : (i % 2 === 0 ? 2 : 4);
    S += w / E_LCDM(z, Om, Or, Ol);
  }
  return (c / H0) * (dz / 3) * S;
}

function w_eff_LCDM(z, Om, Or, Ol) {
  const zp = 1 + z;
  const rho_m = Om * zp**3;
  const rho_r = Or * zp**4;
  const rho_L = Ol;

  const rho = rho_m + rho_r + rho_L;
  if (rho <= 0) return NaN;

  const p = (1/3) * rho_r - rho_L;
  return p / rho;
}

function fmt(x, n=4) {
  return (isFinite(x) ? x.toFixed(n) : "NaN");
}

function computeLCDM() {
  const z   = parseFloat(document.getElementById("lcdm-z").value);
  const H0  = parseFloat(document.getElementById("lcdm-h0").value);
  const Om  = parseFloat(document.getElementById("lcdm-om").value);
  const Or  = parseFloat(document.getElementById("lcdm-or").value);
  const Ol  = parseFloat(document.getElementById("lcdm-ol").value);
  const stp = parseInt(document.getElementById("lcdm-steps").value);

  const out = document.getElementById("lcdm-output");
  out.classList.remove("error");

  if (!isFinite(z) || z < 0) {
    out.textContent = "Redshift z must be ≥ 0";
    out.classList.add("error");
    return;
  }

  const Ez = E_LCDM(z, Om, Or, Ol);
  if (!isFinite(Ez) || Ez <= 0) {
    out.textContent = "Invalid Ω parameters: H(z)^2 ≤ 0";
    out.classList.add("error");
    return;
  }

  const Hz = H0 * Ez;
  const chi = integrate_chi(H0, Om, Or, Ol, z, stp);
  const DL  = (1 + z) * chi;
  const DA  = chi / (1 + z);
  const muSN = 5 * Math.log10(DL) + 25;

  const w   = w_eff_LCDM(z, Om, Or, Ol);
  const q   = 0.5 * (1 + 3 * w);

  const lines = [];
  lines.push("ΛCDM background:");
  lines.push(`  H(z)     = ${fmt(Hz, 3)} km/s/Mpc`);
  lines.push(`  E(z)     = ${fmt(Ez, 5)}`);
  lines.push("");
  lines.push("Distances:");
  lines.push(`  χ(z)     = ${fmt(chi, 3)} Mpc`);
  lines.push(`  D_L(z)   = ${fmt(DL, 3)} Mpc`);
  lines.push(`  D_A(z)   = ${fmt(DA, 3)} Mpc`);
  lines.push(`  μ_SN     = ${fmt(muSN, 3)} mag`);
  lines.push("");
  lines.push("Effective equation of state:");
  lines.push(`  w_eff    = ${fmt(w, 4)}`);
  lines.push(`  q(z)     = ${fmt(q, 4)}   (q < 0 ⇒ acceleration)`);

  out.textContent = lines.join("\n");
}

/* ============================================================
   QKDE RUNNING–K VISUALIZER
   ------------------------------------------------------------
   Illustrates the drift of the kinetic normalization:
        K(N) = 1 + K0 e^{-pN}
   ============================================================ */

function computeQKDE() {
  const z  = parseFloat(document.getElementById("qkde-z").value);
  const K0 = parseFloat(document.getElementById("qkde-k0").value);
  const p  = parseFloat(document.getElementById("qkde-p").value);

  const out = document.getElementById("qkde-output");
  out.classList.remove("error");

  if (!isFinite(z) || z < 0) {
    out.textContent = "Redshift z must be ≥ 0";
    out.classList.add("error");
    return;
  }

  const N = -Math.log(1 + z);
  const a = Math.exp(N);

  const expTerm = Math.exp(-p * N);
  const K = 1 + K0 * expTerm;
  const Kprime_over_K = (-p * K0 * expTerm) / K;

  const K_via_z = 1 + K0 * Math.pow(1 + z, p);

  const lines = [];
  lines.push("QKDE Running–K:");
  lines.push(`  N(z)          = ${fmt(N, 5)}`);
  lines.push(`  a(z)          = ${fmt(a, 5)}`);
  lines.push("");
  lines.push(`  K(N)          = ${fmt(K, 6)}`);
  lines.push(`  K'(N)/K(N)    = ${fmt(Kprime_over_K, 6)}`);
  lines.push("");
  lines.push(`  K(z) via (1+z)^p = ${fmt(K_via_z, 6)}`);
  lines.push("");
  lines.push("Notes:");
  lines.push("• This is a visualizer only.");
  lines.push("• The full QKDE background system requires solving coupled ODEs.");
  lines.push("• Exact equations are in the monograph and GitHub repo.");

  out.textContent = lines.join("\n");
}

/* ============================================================
   EVENT BINDINGS
   ============================================================ */

document.getElementById("lcdm-button")
  .addEventListener("click", computeLCDM);

document.getElementById("qkde-button")
  .addEventListener("click", computeQKDE);

// Allow Enter key to trigger computation
["lcdm-z","lcdm-h0","lcdm-om","lcdm-or","lcdm-ol","lcdm-steps"]
  .forEach(id => {
    const el = document.getElementById(id);
    el.addEventListener("keyup", e => {
      if (e.key === "Enter") computeLCDM();
    });
  });

["qkde-z","qkde-k0","qkde-p"]
  .forEach(id => {
    const el = document.getElementById(id);
    el.addEventListener("keyup", e => {
      if (e.key === "Enter") computeQKDE();
    });
  });

</script>

</body>
</html>

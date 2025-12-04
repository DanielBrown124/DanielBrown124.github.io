---
layout: none
title: Quantum–Kinetic Dark Energy (QKDE)
---

<script>
  window.MathJax = { tex: { inlineMath: [['$','$'], ['\\(','\\)']] } };
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<style>
.alt-button {
  background: #fff0b3;
  color: #0b0c10;
}

.alt-button:hover {
  background: #ffe680;
  box-shadow: 0 0 14px rgba(255, 230, 128, 0.8);
}

.alt-cite-btn {
  background: #c8f5ff;
}

.alt-cite-btn:hover {
  background: #aee8f7;
}

.author-box {
  align-items: center;
  background: rgba(15, 22, 32, 0.55);
  border: 1px solid rgba(102,252,241,0.12);
  border-radius: 14px;
  box-shadow: inset 0 0 15px rgba(102,252,241,0.09);
  display: flex;
  gap: 25px;
  padding: 25px;
}

.author-photo {
  border: 2px solid rgba(102,252,241,0.22);
  border-radius: 8px;
  box-shadow: 0 0 12px rgba(102,252,241,0.26);
  height: 130px;
  object-fit: cover;
  width: 130px;
}

body {
  background: url("cosmos.jpeg") no-repeat center center fixed;
  background-size: cover;
  color: #e8e9ef;
  font-family: "Inter", sans-serif;
  line-height: 1.75;
  margin: 0;
  overflow-x: hidden;
  padding: 0;
}

.center {
  text-align: center;
}

.cite-box {
  background: rgba(15, 22, 32, 0.55);
  border: 1px solid rgba(102, 252, 241, 0.12);
  border-radius: 12px;
  box-shadow: 0 0 20px rgba(102,252,241,0.12);
  margin-top: 40px;
  padding: 20px 25px;
}

.cite-buttons {
  display: flex;
  gap: 14px;
  margin-top: 14px;
}

.cite-header h3 {
  font-size: 1.45rem;
  margin-bottom: 4px;
}

.cite-label {
  color: #c5f2ff;
  display: block;
  font-family: "Merriweather", serif;
  font-size: 0.95rem;
  margin-bottom: 6px;
}

.cite-select {
  background: rgba(20, 30, 45, 0.7);
  border: 1px solid rgba(102,252,241,0.20);
  border-radius: 6px;
  color: #e8e9ef;
  font-size: 0.95rem;
  margin-bottom: 14px;
  padding: 6px 10px;
}

.cite-select:hover {
  border-color: rgba(102,252,241,0.40);
  cursor: pointer;
}

.cite-subtext {
  color: #c9e6f8;
  font-size: 0.9rem;
  margin-top: 0;
  opacity: 0.8;
}

.cite-text {
  background: rgba(0, 0, 0, 0.45);
  border: 1px solid rgba(120,160,200,0.25);
  border-radius: 8px;
  color: #e8e9ef;
  font-family: "JetBrains Mono", "Menlo", "Consolas", monospace;
  font-size: 0.88rem;
  max-height: 220px;
  overflow-y: auto;
  padding: 14px 16px;
  transition: max-height 0.3s ease;
}

.details-body {
  font-size: 0.95rem;
  margin-top: 14px;
}

details {
  background: rgba(15, 22, 32, 0.45);
  border: 1px solid rgba(102,252,241,0.14);
  border-radius: 12px;
  margin-top: 30px;
  padding: 16px 20px;
}

details + details {
  margin-top: 22px;
}

details summary {
  color: #c5f2ff;
  cursor: pointer;
  font-family: "Merriweather", serif;
  font-size: 1.1rem;
  font-weight: 300;
  list-style: none;
}

details summary::-webkit-details-marker {
  display: none;
}

details[open] .summary-label::before {
  transform: rotate(90deg);
}

.enhanced-cite {
  background: linear-gradient(
      to bottom right,
      rgba(15, 22, 32, 0.7),
      rgba(12, 18, 28, 0.55)
    );
  border: 1px solid rgba(102,252,241,0.18);
  border-radius: 14px;
  box-shadow: 0 0 25px rgba(102,252,241,0.15);
  margin-top: 55px;
  padding: 28px 28px 32px;
  position: relative;
}

.enhanced-cite::before {
  background: linear-gradient(to right, #66fcf1, #45a0c9, #66fcf1);
  border-top-left-radius: 14px;
  border-top-right-radius: 14px;
  content: "";
  height: 3px;
  left: 0;
  opacity: 0.8;
  position: absolute;
  top: 0;
  width: 100%;
}

h1, h2, h3 {
  color: #9be7ff;
  font-family: "Merriweather", serif;
  font-weight: 300;
  margin-top: 0;
}

h1 {
  font-size: 2.4rem;
  letter-spacing: 0.5px;
  text-align: center;
}

h2 {
  font-size: 1.8rem;
  margin-top: 40px;
}

h3 {
  color: #b9ecff;
  margin-bottom: 12px;
}

html {
  scroll-behavior: smooth;
}

[id] {
  scroll-margin-top: 90px;
}

.nav-header {
  background: linear-gradient(
    to right,
    rgba(5, 10, 20, 0.94),
    rgba(8, 15, 28, 0.94)
  );
  backdrop-filter: blur(10px);
  border-bottom: 1px solid rgba(102,252,241,0.18);
  border-top-left-radius: 14px;
  border-top-right-radius: 14px;
  box-shadow: 0 4px 18px rgba(0,0,0,0.55);
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  justify-content: center;
  margin: -30px -30px 25px;
  padding: 12px 18px;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.nav-header a {
  border: 1px solid transparent;
  border-radius: 999px;
  color: #c8eaff;
  font-size: 0.9rem;
  letter-spacing: 0.03em;
  padding: 6px 10px;
  text-decoration: none;
  text-transform: uppercase;
  transition: 0.18s ease;
}

.nav-header a:hover {
  background: rgba(102,252,241,0.09);
  border-color: rgba(102,252,241,0.6);
  color: #ffffff;
  text-shadow: 0 0 6px rgba(102,252,241,0.9);
}

.nav-header .nav-button {
  background: linear-gradient(135deg, #66fcf1, #45c9c9);
  border: 1px solid rgba(255,255,255,0.15);
  border-radius: 14px;
  box-shadow: 0 0 6px rgba(102,252,241,0.35);
  color: #0a0f12;
  display: inline-block;
  font-size: 0.83rem;
  font-weight: 600;
  margin-left: 10px;
  padding: 6px 14px;
  text-decoration: none;
  text-transform: none;
  transition: all 0.25s ease;
  white-space: nowrap;
}

.nav-header .nav-button:hover {
  background: linear-gradient(135deg, #8afef4, #5edbd8);
  box-shadow: 0 0 10px rgba(102,252,241,0.5);
  color: #000;
  transform: translateY(-1px);
}

.page {
  background: rgba(10, 13, 20, 0.72);
  backdrop-filter: blur(12px);
  border: 1px solid rgba(102,252,241,0.12);
  border-radius: 18px;
  box-shadow: 0 0 35px rgba(102,252,241,0.18);
  margin: 90px auto;
  max-width: 900px;
  padding: 50px;
}

.paper-box {
  background: rgba(15, 22, 32, 0.45);
  border: 1px solid rgba(102,252,241,0.10);
  border-radius: 14px;
  box-shadow: 0 0 20px rgba(102,252,241,0.12);
  padding: 30px;
}

.paper-button {
  background: #d2f2ff;
  border-radius: 7px;
  color: #0b0c10;
  display: inline-block;
  font-size: 1.05rem;
  padding: 12px 28px;
  text-decoration: none;
  transition: 0.2s;
}

.paper-button:hover {
  background: #bfe6f7;
  box-shadow: 0 0 16px rgba(174,234,255,0.8);
}

.ref-list {
  color: #ffffff;
  font-size: 0.92rem;
  margin: 0;
  padding-left: 22px;
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

.ref-list li {
  color: #ffffff;
  margin-bottom: 6px;
}

.site-footer {
  border-top: 1px solid rgba(102,252,241,0.10);
  color: #a8c3d9;
  font-size: 0.85rem;
  margin-top: 55px;
  opacity: 0.8;
  padding-top: 20px;
  text-align: center;
}

.social-box {
  background: rgba(15, 22, 32, 0.45);
  border: 1px solid rgba(102,252,241,0.10);
  border-radius: 12px;
  margin-top: 25px;
  padding: 18px 25px;
}

.social-icon {
  flex-shrink: 0;
  height: 20px;
  width: 20px;
}

.social-icon img {
  height: 22px;
  margin-right: 8px;
  vertical-align: middle;
  width: 22px;
}

.social-icon svg {
  fill: #aeeaff;
  height: 100%;
  width: 100%;
}

.social-link {
  align-items: center;
  color: #aeeaff;
  display: flex;
  gap: 10px;
  margin-bottom: 8px;
  text-decoration: none;
  transition: 0.2s ease;
}

.social-link:hover {
  color: #66fcf1;
  text-shadow: 0 0 8px rgba(102,252,241,0.8);
}

.summary-label {
  padding-left: 18px;
  position: relative;
}

.summary-label::before {
  content: "▸";
  font-size: 0.9rem;
  left: 0;
  position: absolute;
  top: 0;
  transition: transform 0.15s ease;
}

.symbol-table {
  border-collapse: collapse;
  font-size: 0.9rem;
  width: 100%;
}

.symbol-table td,
.symbol-table th {
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

.toast {
  background: rgba(20, 160, 200, 0.9);
  border-radius: 8px;
  bottom: 28px;
  color: white;
  font-size: 0.9rem;
  opacity: 0;
  padding: 12px 18px;
  position: fixed;
  right: 28px;
  transform: translateY(20px);
  transition: all 0.35s ease;
  z-index: 9999;
}

.toast.show {
  opacity: 1;
  transform: translateY(0);
}

/* RESPONSIVE FIXES */
/* Slightly shrink narrow screens so 2 cards still fit */
@media (max-width: 980px) {
  .calc-card {
    flex: 1 1 calc(50% - 20px);
    max-width: 350px;
  }
}

/* Mobile: one card per row */
@media (max-width: 600px) {
  .calc-card {
    flex: 1 1 100%;
    max-width: 100%;
  }
}adding: 18px 18px 20px;
  }
 .calc-grid {
  margin-top: 14px;
  display: flex;
  flex-wrap: wrap;
  gap: 18px;
  justify-content: center;
}
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
  <a href="#comparison-qkde">Comparisons</a>
  <a href="#references-qkde">References</a>
  <a href="#cite-qkde">Cite</a>
  <a href="calculator.html">Calculator</a>
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

  <a href="https://doi.org/10.5281/zenodo.17774687" class="social-link" target="_blank">
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
  <summary><span class="summary-label">Symbol Index</span></summary>
  <div class="details-body">

    <p>
      Complete list of symbols used in the QKDE framework. Natural units
      \(c=\hbar=1\) are used. Mass dimension is shown where meaningful.
      Definitions match <em>exactly</em> those used in the monograph.
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

        <!-- COSMOLOGY BASICS -->
        <tr><th colspan="3" style="background:rgba(80,120,150,0.25);">Cosmological background</th></tr>

        <tr>
          <td>\(a(t)\)</td>
          <td>1</td>
          <td>Scale factor; normalized to \(a_0=1\).</td>
        </tr>
        <tr>
          <td>\(N\)</td>
          <td>1</td>
          <td>E-fold time: \(N=\ln a\). Derivatives: \(f'=\mathrm{d}f/\mathrm{d}N\).</td>
        </tr>
        <tr>
          <td>\(z\)</td>
          <td>1</td>
          <td>Redshift: \(z=e^{-N}-1\).</td>
        </tr>
        <tr>
          <td>\(H=\dot a/a,\ H_0\)</td>
          <td>M</td>
          <td>Hubble rate and present value.</td>
        </tr>
        <tr>
          <td>\(E\)</td>
          <td>1</td>
          <td>Dimensionless Hubble derivative: \(E = H'/H\).</td>
        </tr>
        <tr>
          <td>\(R\)</td>
          <td>M\(^2\)</td>
          <td>Ricci scalar in FRW: \(R = 6H^2(2+E)\).</td>
        </tr>
        <tr>
          <td>\(q\)</td>
          <td>1</td>
          <td>Deceleration parameter: \(q = -1 - E\).</td>
        </tr>
        <tr>
          <td>\(w_{\rm eff}\)</td>
          <td>1</td>
          <td>Effective equation of state: \(w_{\rm eff} = -1 - \tfrac{2}{3}E\).</td>
        </tr>

        <!-- ENERGY CONTENT -->
        <tr><th colspan="3" style="background:rgba(80,120,150,0.25);">Energy densities, matter components</th></tr>

        <tr>
          <td>\(\rho_i,p_i\)</td>
          <td>M\(^4\)</td>
          <td>Energy density and pressure of component \(i\in\{m,r,\phi\}\).</td>
        </tr>
        <tr>
          <td>\(\Omega_i\)</td>
          <td>1</td>
          <td>Density fraction: \(\Omega_i = \rho_i/(3M_{\rm pl}^2H^2)\).</td>
        </tr>
        <tr>
          <td>\(M_{\rm pl}\)</td>
          <td>M</td>
          <td>Reduced Planck mass: \(M_{\rm pl} = (8\pi G)^{-1/2}\).</td>
        </tr>

        <!-- DISTANCES & OBSERVABLES -->
        <tr><th colspan="3" style="background:rgba(80,120,150,0.25);">Distances & observable functions</th></tr>

        <tr>
          <td>\(\chi(z)\)</td>
          <td>M\(^{-1}\)</td>
          <td>Comoving distance: \(\chi=\int_0^z H^{-1}\,\mathrm{d}z'\).</td>
        </tr>
        <tr>
          <td>\(D_A, D_L\)</td>
          <td>M\(^{-1}\)</td>
          <td>Angular-diameter and luminosity distances. \(D_L=(1+z)^2D_A\).</td>
        </tr>
        <tr>
          <td>\(D_V(z)\)</td>
          <td>M\(^{-1}\)</td>
          <td>BAO distance: \(D_V=[(1+z)^2D_A^2 z/H]^{1/3}\).</td>
        </tr>
        <tr>
          <td>\(F_{\rm AP}\)</td>
          <td>1</td>
          <td>Alcock–Paczyński parameter: \(F_{\rm AP}=(1+z)D_A/H\).</td>
        </tr>
        <tr>
          <td>\(r_d\)</td>
          <td>M\(^{-1}\)</td>
          <td>Sound horizon at drag epoch.</td>
        </tr>
        <tr>
          <td>\(\mu_{\rm SN}\)</td>
          <td>1</td>
          <td>Distance modulus: \(\mu=5\log_{10}(D_L/{\rm Mpc})+25\).</td>
        </tr>

        <!-- SCALAR FIELD -->
        <tr><th colspan="3" style="background:rgba(80,120,150,0.25);">Scalar-field sector</th></tr>

        <tr>
          <td>\(\phi\)</td>
          <td>M</td>
          <td>Homogeneous scalar field.</td>
        </tr>
        <tr>
          <td>\(s\)</td>
          <td>1</td>
          <td>Scalar velocity in e-folds: \(s = \phi'\).</td>
        </tr>
        <tr>
          <td>\(X\)</td>
          <td>M\(^4\)</td>
          <td>Kinetic invariant: \(X=-\tfrac12 g^{\mu\nu}\partial_\mu\phi\partial_\nu\phi\). FRW: \(X=\tfrac12\dot\phi^2\).</td>
        </tr>
        <tr>
          <td>\(V(\phi)\)</td>
          <td>M\(^4\)</td>
          <td>Scalar potential.</td>
        </tr>
        <tr>
          <td>\(K(t)\)</td>
          <td>1</td>
          <td>Kinetic normalization; must satisfy \(K>0\) (ghost freedom).</td>
        </tr>
        <tr>
          <td>\(\rho_\phi,p_\phi\)</td>
          <td>M\(^4\)</td>
          <td>\(\rho_\phi=KX+V,\quad p_\phi=KX-V.\)</td>
        </tr>
        <tr>
          <td>\(w_\phi\)</td>
          <td>1</td>
          <td>Scalar equation of state: \(w_\phi=(KX-V)/(KX+V)\).</td>
        </tr>

        <!-- QKDE KINETIC MODELS -->
        <tr><th colspan="3" style="background:rgba(80,120,150,0.25);">QKDE kinetic-normalization models</th></tr>

        <tr>
          <td>\(\alpha, M\)</td>
          <td>1, M</td>
          <td>Curvature-driven model: \(K=1+\alpha R/M^2\).</td>
        </tr>
        <tr>
          <td>\(K_0,p,N_p\)</td>
          <td>1,1,1</td>
          <td>Running form: \(K(N)=1+K_0 e^{-pN}\).\newline 
              Optional shifted form: \(K=1+K_p e^{-p(N-N_p)}\).</td>
        </tr>
        <tr>
          <td>\(K'/K\)</td>
          <td>1</td>
          <td>E-fold derivative of \(K\). Exact expression in curvature model.</td>
        </tr>

        <!-- PERTURBATIONS -->
        <tr><th colspan="3" style="background:rgba(80,120,150,0.25);">Perturbations and EFT–DE</th></tr>

        <tr>
          <td>\(\Phi,\Psi\)</td>
          <td>1</td>
          <td>Newtonian potentials; in QKDE: \(\Phi=\Psi\).</td>
        </tr>
        <tr>
          <td>\(v,z\)</td>
          <td>M, M</td>
          <td>Scalar perturbation variables: \(v=a(\delta\phi+\dot\phi\,\Phi/H)\); \(z^2=a^2K\dot\phi^2/H^2\).</td>
        </tr>
        <tr>
          <td>\(\mathcal{R}\)</td>
          <td>1</td>
          <td>Comoving curvature perturbation: \(\mathcal{R}=v/z\).</td>
        </tr>
        <tr>
          <td>\(c_s^2\)</td>
          <td>1</td>
          <td>Scalar sound speed; QKDE enforces \(c_s^2=1\).</td>
        </tr>
        <tr>
          <td>\(c_T^2\)</td>
          <td>1</td>
          <td>Tensor propagation speed; QKDE requires \(c_T^2=1\).</td>
        </tr>

        <tr>
          <td>\(\alpha_K\)</td>
          <td>1</td>
          <td>Kinetic EFT–DE function: \(\alpha_K = K\dot\phi^2/(H^2 M_{\rm pl}^2)\ge 0\).</td>
        </tr>
        <tr>
          <td>\(\alpha_B,\alpha_M,\alpha_T,\alpha_H\)</td>
          <td>1</td>
          <td>EFT–DE functions; all vanish in QKDE.</td>
        </tr>
        <tr>
          <td>\(\mu(a,k)\)</td>
          <td>1</td>
          <td>Effective Newton constant; QKDE predicts \(\mu=1\).</td>
        </tr>
        <tr>
          <td>\(\Sigma(a,k)\)</td>
          <td>1</td>
          <td>Lensing modifier; QKDE predicts \(\Sigma=1\).</td>
        </tr>
        <tr>
          <td>\(\eta(a,k)\)</td>
          <td>1</td>
          <td>Slip parameter; QKDE predicts \(\eta=0\).</td>
        </tr>

        <!-- GROWTH -->
        <tr><th colspan="3" style="background:rgba(80,120,150,0.25);">Growth of structure</th></tr>

        <tr>
          <td>\(D(a)\)</td>
          <td>1</td>
          <td>Linear growth factor, obeying GR growth equation with modified \(H(a)\).</td>
        </tr>
        <tr>
          <td>\(f\)</td>
          <td>1</td>
          <td>Growth rate: \(f=\mathrm{d}\ln D/\mathrm{d}\ln a\).</td>
        </tr>
        <tr>
          <td>\(\sigma_{8,0}\)</td>
          <td>1</td>
          <td>Amplitude of matter fluctuations at \(z=0\).</td>
        </tr>
        <tr>
          <td>\(f\sigma_8(z)\)</td>
          <td>1</td>
          <td>RSD observable: \(f(z)\sigma_{8,0}D(z)/D(0)\).</td>
        </tr>

        <!-- RESIDUALS / CONSISTENCY -->
        <tr><th colspan="3" style="background:rgba(80,120,150,0.25);">Consistency & residuals</th></tr>

        <tr>
          <td>\(C_F\)</td>
          <td>1</td>
          <td>Friedmann-closure residual: \(1-\Omega_m-\Omega_r-\Omega_\phi\).</td>
        </tr>
        <tr>
          <td>\(C_R\)</td>
          <td>1</td>
          <td>Raychaudhuri residual in e-fold form.</td>
        </tr>
        <tr>
          <td>\(C_\phi\)</td>
          <td>1</td>
          <td>Klein–Gordon residual.</td>
        </tr>
        <tr>
          <td>\(C_{R/H^2}\)</td>
          <td>1</td>
          <td>Residual of identity \(R/H^2 = 6(2+H'/H)\).</td>
        </tr>
        <tr>
          <td>\(C_{\nabla\cdot T_\phi}\)</td>
          <td>1</td>
          <td>Residual from non-conservation due to time-dependent \(K'(N)\).</td>
        </tr>

        <!-- MISC -->
        <tr><th colspan="3" style="background:rgba(80,120,150,0.25);">Miscellaneous</th></tr>

        <tr>
          <td>\(k,\ell\)</td>
          <td>M, 1</td>
          <td>Comoving wavenumber and multipole index.</td>
        </tr>
        <tr>
          <td>\(P(k,z)\)</td>
          <td>M\(^{-3}\)</td>
          <td>Linear matter power spectrum \(P(k,z)=D^2(z)P(k,0)\).</td>
        </tr>
        <tr>
          <td>\(Q_\mu\)</td>
          <td>M\(^3\)</td>
          <td>Interaction four-vector for bookkeeping when energy exchange is considered (unused in minimal QKDE).</td>
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
      QKDE framework, organized into nested dropdowns for clarity. Every expression
      matches the notation and equations in the monograph. No heuristic steps are omitted:
      all transformations, identities, and definitions are stated explicitly. Where relevant,
      we also note subtle points (e.g., sign conventions for \(X\), gauge choices, and
      assumptions about background time dependence) to ensure full reproducibility and
      referee-level transparency.
    </p>

    <!-- ===================================================== -->
    <!-- 0. Covariant Action and Variational Foundations      -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">0. Covariant action → field equations</span></summary>
      <div class="details-body">

        <p><strong>Starting point:</strong></p>

        <p>
          QKDE is defined by a <em>covariant</em> scalar–tensor action in which the kinetic
          normalization is a <em>background function of time</em>, consistent with the EFT of
          Dark Energy (unitary-gauge coefficient depending on the background clock
          \(\phi_0(t)\)):
        </p>

        \[
        S = \int d^4x\,\sqrt{-g}\,
        \left[\frac12 M_{\rm pl}^2 R + K(t)X - V(\phi)\right],
        \qquad
        X = -\frac12 g^{\mu\nu}\partial_\mu\phi\partial_\nu\phi .
        \]

        <p>
          Since \(g^{00}=-1\), the kinetic invariant becomes
          \(X = \frac12 \dot\phi^2\). We make this sign explicit to avoid
          confusion when comparing conventions.
        </p>

        <h4>(a) Energy–momentum tensor</h4>

        \[
        T_{\mu\nu} = K\,\partial_\mu\phi\partial_\nu\phi 
        - g_{\mu\nu}\left(KX - V\right).
        \]

        In FRW:

        \[
        \rho_\phi = KX + V, \qquad p_\phi = KX - V.
        \]

        <h4>(b) Scalar equation of motion</h4>

        \[
        \nabla_\mu(K \nabla^\mu \phi) + V_{,\phi} = 0.
        \]

        Because \(K = K(t)\):

        \[
        \nabla_\mu(K \nabla^\mu\phi)
        = K \Box\phi + K_{,\mu}\nabla^\mu\phi .
        \]

        In FRW, using \(\dot K = H K'\):

        \[
        K(\ddot\phi + 3H\dot\phi) + HK' \dot\phi + V_{,\phi}=0.
        \]

        <h4>(c) Einstein equations</h4>

        \[
        3M_{\rm pl}^2 H^2 = \rho_m + \rho_r + \rho_\phi ,
        \qquad
        M_{\rm pl}^2 (2\dot H + 3H^2) = -p_m - p_r - p_\phi .
        \]

        <p>
          QKDE does <em>not</em> modify the Einstein–Hilbert gravitational sector:
          all departures from ΛCDM arise solely through the scalar-field energy budget via
          \(K(t)\).
        </p>

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
        \qquad 
        f' \equiv \frac{df}{dN} = \frac{1}{H}\frac{df}{dt},
        \qquad
        E \equiv \frac{H'}{H} = \frac{d\ln H}{dN}.
        \]

        <h4>(b) Scalar velocity variable</h4>

        Define:

        \[
        s \equiv \phi' = \frac{\dot\phi}{H}.
        \]

        Then:

        \[
        X = \frac12\dot\phi^2 = \frac12 H^2 s^2.
        \]

        <p>
          This identity is exact and makes the scalar dynamics depend only on
          \((s, K, V)\) once the Hubble rate is known.
        </p>

        <h4>(c) Transforming the scalar EOM</h4>

        Starting from:

        \[
        K(\ddot\phi + 3H\dot\phi) + \dot K\,\dot\phi + V_{,\phi} = 0,
        \]

        use:

        \[
        \dot\phi = Hs, \qquad
        \ddot\phi = H^2 s' + H^2 E s, \qquad
        \dot K = H K'.
        \]

        Substitute:

        \[
        K(H^2 s' + H^2 E s + 3H^2 s)
        + HK'Hs + V_{,\phi} = 0.
        \]

        Divide by \(H^2 K\):

        \[
        s' = -(3+E)s - \frac{K'}{K}s - \frac{V_{,\phi}}{H^2K}.
        \]

        <h4>(d) Final closed background system</h4>

        \[
        \phi' = s,
        \qquad
        s' = -(3+E)s - \frac{K'}{K}s - \frac{V_{,\phi}}{H^2K},
        \qquad
        E = \frac{H'}{H}.
        \]

        <p>
          Once \(K'/K(N)\) is specified (e.g., curvature-induced or running),
          the system becomes fully deterministic and requires no numerical differentiation.
        </p>

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
        R = 6(2H^2 + \dot H)
        = 6H^2(2 + E).
        \]

        <h4>(b) Derivative of \(R\)</h4>

        Using:

        \[
        R = 6H^2(2+E),
        \]

        differentiate:

        \[
        \frac{R'}{R}
        = 2E + \frac{E'}{2+E}.
        \]

        <p>
          We emphasize this identity because it closes the curvature–K system analytically:
          no finite differencing of \(H(N)\) is required in numerical evolution.
        </p>

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

            <p>
              The UV-motivated curvature model takes \(K\) to be sourced by the Ricci scalar:
            </p>

            \[
            K = 1 + \frac{\alpha R}{M^2}.
            \]

            Then:

            \[
            \frac{K'}{K}
            = \frac{\alpha R'}{M^2 + \alpha R}.
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

            <p>
              This form is fully analytic and eliminates numerical instability in evaluating
              \(K'/K\).
            </p>

            <p><strong>Viability:</strong></p>

            \[
            M^2 + \alpha R \neq 0, \qquad
            K > 0.
            \]

            These prevent poles and ensure ghost freedom.

          </div>
        </details>

        <!-- Running Model -->
        <details>
          <summary><span class="summary-label">3b. Running form \(K(N)\)</span></summary>
          <div class="details-body">

            <p>Phenomenological parameterization:</p>

            \[
            K(N) = 1 + K_0 e^{-pN}.
            \]

            Then:

            \[
            \frac{K'}{K} =
            \frac{-p K_0 e^{-pN}}{1 + K_0 e^{-pN}}.
            \]

            <p>
              This model provides a clean analytic handle for intuition and improves sampling
              efficiency during parameter scans. It also approximates curvature-induced
              evolution in the slow-variation regime.
            </p>

          </div>
        </details>

      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 4. Energy–momentum and EOS                           -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">4. Energy–momentum components & equation of state</span></summary>
      <div class="details-body">
        \[
        \rho_\phi = KX + V,
        \qquad
        p_\phi = KX - V.
        \]

        With \(X = \frac12H^2 s^2\):

        \[
        w_\phi = \frac{KX - V}{KX + V}.
        \]

        <p>
          Note that even if \(V(\phi)\) is constant, time variation in \(K(N)\)
          produces an evolving equation of state — this is the core physical
          mechanism behind QKDE’s background acceleration.
        </p>

      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 5. KG equation                                       -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">5. Full Klein–Gordon derivation in e-fold time</span></summary>
      <div class="details-body">

        From:

        \[
        K(\ddot\phi + 3H\dot\phi) + \dot K\,\dot\phi + V_{,\phi}=0,
        \]

        substitute:

        \[
        \ddot\phi = H^2 s' + H^2 E s,
        \qquad
        \dot\phi = H s,
        \qquad
        \dot K = HK'.
        \]

        Then:

        \[
        s' = -(3+E)s - \frac{K'}{K}s - \frac{V_{,\phi}}{H^2K}.
        \]

        <p>
          This expression shows explicitly how time-variation in the kinetic normalization
          modifies damping, while preserving the canonical sound speed and GR structure.
        </p>

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

        implies:

        \[
        \alpha_K = \frac{K\dot\phi^2}{H^2 M_{\rm pl}^2},
        \qquad
        \alpha_B = 0,\ \alpha_M=0,\ \alpha_T=0,\ \alpha_H=0.
        \]

        <p>
          Therefore QKDE occupies the GR-preserving, luminal-tensor, constant-\(M_{\rm pl}\)
          corner of EFT–DE, differentiating it sharply from Horndeski,
          beyond-Horndeski, DHOST, or modified-gravity families.
        </p>

      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 7. Perturbations & sound speed                       -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">7. Perturbation theory & sound speed derivation</span></summary>
      <div class="details-body">

        <h4>(a) Second-order action</h4>

        Expand in Newtonian gauge:

        \[
        S^{(2)} = \int d^4x\, a^3
        \left[
          K \dot\phi^2 (\dot{\delta\phi})^2
          - K \frac{(\nabla\delta\phi)^2}{a^2}
          + \ldots
        \right].
        \]

        <h4>(b) Canonical variable</h4>

        \[
        v = a(\delta\phi + \dot\phi\,\Phi/H),
        \qquad
        z^2 = a^2 K\dot\phi^2/H^2.
        \]

        Then:

        \[
        S^{(2)} = \frac12 \int d\eta\, d^3k 
        \left[v'^2 - c_s^2 k^2 v^2 + \frac{z''}{z} v^2\right].
        \]

        <h4>(c) Sound speed</h4>

        <p>
          Both the gradient and kinetic terms are multiplied by the same coefficient \(K\),
          so the physical sound speed is:
        </p>

        \[
        c_s^2 = 1.
        \]

        <h4>(d) Metric potentials</h4>

        In linear Einstein equations:

        \[
        \Phi = \Psi,\qquad \mu = \Sigma = 1,\qquad \eta = 0.
        \]

        <p>
          Thus, QKDE produces <em>no modified-gravity signatures</em> in perturbations.
          All observable deviations originate solely from the background expansion.
        </p>

      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 8. Growth equation                                   -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">8. Growth of structure derivation</span></summary>
      <div class="details-body">

        Matter growth (GR, subhorizon) satisfies:

        \[
        \ddot D + 2H \dot D - \frac{3}{2}H^2 \Omega_m D = 0.
        \]

        In e-fold variables:

        \[
        D' = \frac{\dot D}{H},\qquad
        D'' = \frac{\ddot D}{H^2} - E D'.
        \]

        So:

        \[
        D'' + (2 + E)D' - \frac{3}{2}\Omega_m D = 0.
        \]

        <p>
          Since QKDE preserves GR, the growth equation is <em>identical</em> to ΛCDM
          except for the modified background expansion \(H(N)\).
        </p>

      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 9. Stability conditions                               -->
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
        M^2 + \alpha R \neq 0,\qquad K = 1 + \frac{\alpha R}{M^2} > 0.
        \]

        <p>
          These ensure well-posed dynamics and exclude pathological operator choices.
        </p>

      </div>
    </details>

    <!-- ===================================================== -->
    <!-- 10. Numerical consistency checks                     -->
    <!-- ===================================================== -->
    <details>
      <summary><span class="summary-label">10. Numerical identity checks (pipeline)</span></summary>
      <div class="details-body">

        <p>
          The monograph implements several diagnostic identities to guarantee
          algebraic closure and verify that the system evolves consistently
          at machine precision:
        </p>

        <ul>
          <li>\(C_F = 1 - \Omega_m - \Omega_r - \Omega_\phi\)</li>
          <li>\(C_R = R/H^2 - 6(2+E)\)</li>
          <li>\(C_\phi\) from the KG equation</li>
          <li>\(C_{\nabla\cdot T_\phi}\) verifying scalar conservation</li>
          <li>\(C_{R/H^2}\) checking the Ricci identity closure</li>
        </ul>

        <p>
          These checks quantify reproducibility and ensure that no hidden assumptions
          or numerical artifacts enter the construction of QKDE.
        </p>

      </div>
    </details>

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
        <p>
          In flat ΛCDM the late–time acceleration of the Universe is attributed to a strict
          cosmological constant, with no additional scalar degree of freedom. The action in this
          case is simply the Einstein–Hilbert term plus minimally coupled matter and a constant
          vacuum term, \(S \supset \int \sqrt{-g}\,\Lambda\). There is no scalar kinetic sector,
          no field \(\phi\), and therefore no kinetic invariant \(X\) or kinetic normalization
          \(K(t)\). The effective dark energy equation of state is exactly \(w=-1\) at all times,
          and all departures from matter–dominated expansion are driven by the fixed parameter
          \(\Lambda\).
        </p>

        <p>
          QKDE reduces continuously to ΛCDM in the double limit where the kinetic normalization is
          constant and the potential is effectively constant,
          \[
            K(t) \to K_\star = \text{const}, \qquad V(\phi) \to \Lambda_\star = \text{const},
          \]
          with the scalar frozen on its background. In this limit, the scalar behaves as a pure
          vacuum term and does not introduce any new physical degree of freedom beyond that already
          encoded by \(\Lambda\). Operationally, the Einstein equations, background expansion
          \(H(a)\), and linear perturbations (including structure growth and lensing) become
          identical to those of ΛCDM. Thus ΛCDM appears as a specific corner of QKDE parameter
          space, but generic QKDE solutions depart from it through a slow kinetic drift rather than
          through a change in the metric sector or a large deviation in \(w(a)\).
        </p>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">Quintessence</span></summary>
      <div class="details-body">
        <p>
          Canonical quintessence is defined by a minimally coupled scalar field with fixed
          normalization,
          \[
            P_{\rm quint}(X,\phi) = X - V(\phi),
          \]
          where the entire phenomenology is encoded in the choice of potential \(V(\phi)\). The
          kinetic term is time–independent and canonically normalized; there is no operator that
          rescales \(X\) as the Universe evolves. In this framework the effective equation of state
          \(w_\phi(a)\) and the background expansion \(H(a)\) are driven by the rolling of the
          scalar down its potential. In the EFT–DE language, quintessence has a nonzero
          \(\alpha_K\) originating from the canonical kinetic term, but the normalization of that
          kinetic term does not drift in time at the level of the EFT coefficients.
        </p>

        <p>
          QKDE shares several structural features with quintessence: it lives in pure GR (no
          modification to the Einstein–Hilbert sector), introduces a single scalar degree of
          freedom, predicts luminal gravitational waves, and keeps the scalar sound speed
          canonical, \(c_s^2 = 1\). However, the key difference is that in QKDE the kinetic
          normalization is promoted to a slowly varying function of time,
          \[
            P_{\rm QKDE}(X,\phi,t) = K(t)X - V(\phi), \qquad K(t) > 0,
          \]
          with \(K(t)\) motivated by curvature–suppressed operators such as \(R\,X\) and by
          integrating out heavy fields in quantum field theory in curved spacetime. This time
          dependence is not equivalent, at the EFT level, to a re–labeling of the field or a
          reshaping of the potential: attempting to absorb \(K(t)\) into \(\phi\) or \(V(\phi)\)
          generically introduces derivative couplings or changes the mapping to the EFT–DE
          functions, spoiling the simple pattern \(\alpha_B = \alpha_M = \alpha_T = \alpha_H = 0\).
        </p>

        <p>
          In other words, while both quintessence and QKDE reside in the GR–preserving corner of
          theory space, quintessence is <em>potential–driven with fixed kinetic normalization</em>,
          whereas QKDE is <em>kinetic–normalization–driven with a UV–motivated time dependence in
          \(K(t)\)</em>. No choice of quintessence potential reproduces the same EFT–DE structure as
          QKDE without introducing additional operators or altering the gravitational sector, and
          this observationally distinguishes the two classes.
        </p>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">k-essence</span></summary>
      <div class="details-body">
        <p>
          k-essence generalizes quintessence by allowing an arbitrary functional dependence on the
          kinetic invariant,
          \[
            P_{\rm k\text{-}ess}(X,\phi) = F(X,\phi),
          \]
          often including higher powers of \(X\) and nontrivial mixing between \(X\) and \(\phi\).
          In such models the scalar sound speed is typically noncanonical,
          \(c_s^2 = P_{,X}/(P_{,X} + 2X P_{,XX}) \neq 1\), and the clustering properties of dark
          energy can be quite different from those of a canonical scalar. Many k-essence models
          generate scale–dependent growth, have nontrivial stability conditions, and can exhibit
          regimes in which the effective sound horizon and Jeans scale play a central role in
          large–scale–structure observables.
        </p>

        <p>
          QKDE can be viewed as occupying a narrow, highly constrained corner of the broad
          k-essence theory space. Formally, it is of the form
          \[
            P_{\rm QKDE}(X,\phi,t) = K(t)X - V(\phi),
          \]
          which is linear in \(X\) and has no higher–order kinetic self–interactions. As a
          consequence, the sound speed is exactly canonical at all times, \(c_s^2 = 1\), and dark
          energy does not develop additional clustering modes beyond those already present in GR
          with a smooth component. The only deviation from a canonical scalar resides in the
          <em>background</em> normalization \(K(t)\), which drifts slowly in time but does not
          introduce any new spatial derivative structure.
        </p>

        <p>
          This distinction matters both theoretically and observationally. Theoretically,
          generic k-essence allows almost arbitrary functional freedom in \(F(X,\phi)\), whereas
          QKDE explicitly restricts the operator content to a UV–motivated, curvature–driven
          kinetic drift with a single active EFT–DE function \(\alpha_K\). Observationally,
          generic k-essence often predicts non-luminal scalar perturbations, scale–dependent
          modifications to growth, or nontrivial signatures in large–scale structure that are
          absent in QKDE. Thus, although one can embed QKDE in the broad k-essence taxonomy by
          reading it as a special case of \(F(X,\phi)\), its combination of <em>linear kinetic
          structure, canonical sound speed, GR metric sector,</em> and <em>time–only drift in
          \(K(t)\)</em> defines a much more predictive subclass with a different phenomenological
          footprint.
        </p>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">Modified Gravity (Horndeski, DHOST, f(R), …)</span></summary>
      <div class="details-body">
        <p>
          Modified-gravity (MG) theories such as \(f(R)\) gravity, Horndeski and beyond-Horndeski
          models, and DHOST theories typically alter the Einstein–Hilbert term or introduce
          nonminimal couplings between the scalar and curvature. In the EFT–DE language this is
          reflected in nonzero functions like \(\alpha_M\) (running Planck mass), \(\alpha_B\)
          (braiding between scalar and metric), \(\alpha_T\) (tensor speed excess), or \(\alpha_H\)
          (beyond-Horndeski operators). These changes generically modify the Poisson equation,
          introduce gravitational slip \(\Phi\neq\Psi\), affect the propagation of gravitational
          waves, and often lead to scale-dependent growth, screening mechanisms, or environment-
          dependent forces.
        </p>

        <p>
          QKDE is constructed to be explicitly <em>orthogonal</em> to these MG classes. The metric
          sector is exactly Einsteinian, and the EFT–DE description is characterized by
          \[
            \alpha_K > 0, \qquad
            \alpha_B = \alpha_M = \alpha_T = \alpha_H = 0.
          \]
          There is no running Planck mass, no braiding, no deviation of GW speed from unity, and
          no beyond-Horndeski operator content. As a result, the linearized field equations for
          metric perturbations reduce to those of GR, with
          \(\Phi = \Psi\), \(\mu(a,k) = 1\), \(\Sigma(a,k) = 1\), and \(\eta(a,k) = 0\), and the
          linear growth equation is exactly the GR one with a modified background expansion
          \(H(a)\).
        </p>

        <p>
          From an observational standpoint, this means that any robust detection of scale-dependent
          growth, gravitational slip, or deviations in the propagation of gravitational waves would
          rule out QKDE but might still be accommodated by MG models. Conversely, if future data
          continue to support GR on large scales while allowing modest departures in the late–time
          expansion history, QKDE provides a natural alternative to MG theories by attributing
          those departures solely to a scalar-sector kinetic drift rather than to modifications of
          the gravitational sector itself.
        </p>
      </div>
    </details>

    <details>
      <summary><span class="summary-label">Interacting / Unified Dark Sector</span></summary>
      <div class="details-body">
        <p>
          Interacting dark-energy models introduce explicit couplings between dark energy and
          dark matter, typically through an interaction four-vector \(Q_\mu\) that appears in the
          conservation equations for the individual components. Such couplings can alter the
          background evolution of \(\rho_m\) and \(\rho_\phi\), modify the growth rate, and
          generate additional features in large–scale structure. Unified dark-sector models, such
          as Chaplygin-type fluids or single barotropic components, aim to describe dark matter
          and dark energy as a single effective fluid, often with nontrivial sound speed and
          clustering properties that interpolate between matter–like and vacuum–like behavior.
        </p>

        <p>
          QKDE, in the formulation presented in the monograph, does <em>not</em> introduce any
          explicit dark-sector interaction and does <em>not</em> attempt to unify dark matter and
          dark energy into a single component. Matter and radiation obey standard conservation
          equations, \(\nabla_\mu T^{\mu\nu}_{(m,r)} = 0\), and the scalar sector has its own
          well-defined energy–momentum tensor whose non-conservation arises only from the
          time-dependent normalization \(K(t)\) and is handled consistently within the EFT
          framework. The scalar plays the role of a dark energy component with a controlled kinetic
          drift, while cold dark matter remains a separate, pressureless species.
        </p>

        <p>
          Phenomenologically, this means QKDE does not exhibit the characteristic signatures of
          interacting or unified dark-sector models: there is no energy exchange between matter and
          dark energy in the background equations, no effective dark fluid that simultaneously
          behaves as CDM and DE, and no interaction-driven modifications to clustering beyond those
          induced by the altered background expansion. This separation of sectors makes QKDE easier
          to confront with data, since standard ΛCDM pipelines for matter and radiation can be
          reused with only the background dark-energy component modified.
        </p>
      </div>
    </details>

    <!-- ============================================================
         5. NON-EQUIVALENCE
    ============================================================ -->
    <details>
      <summary><span class="summary-label">Non-Equivalence Summary</span></summary>
      <div class="details-body">
        <p>
          Taken together, the comparisons above show that QKDE occupies a <em>distinct</em>
          position in theory space. It is not simply quintessence in disguise: the time-dependent
          kinetic normalization \(K(t)\) cannot, in general, be absorbed into a redefined potential
          without introducing additional operators or altering the clean EFT–DE pattern with a
          single active function \(\alpha_K\). It is not generic k-essence, because the kinetic
          sector is strictly linear in \(X\) and enforces a canonical sound speed
          \(c_s^2 = 1\), avoiding the broad functional freedom and scale-dependent clustering
          effects usually associated with k-essence. It is not modified gravity, since the
          Einstein–Hilbert term is untouched and all gravitational EFT coefficients besides
          \(\alpha_K\) vanish, leading to GR values \(\mu=\Sigma=1\) and \(\eta=0\) on linear
          scales. Nor is it an interacting or unified dark-sector model, as the matter and radiation
          sectors remain separately conserved and dark energy is not merged with dark matter into a
          single fluid.
        </p>

        <p>
          The combination of (i) a GR metric sector, (ii) a single scalar with canonical
          perturbations, (iii) a UV-motivated, time-dependent kinetic normalization \(K(t)\), and
          (iv) a sharply constrained EFT–DE imprint (only \(\alpha_K\neq0\)) yields a framework
          whose predictions are tightly specified and falsifiable. In this sense, QKDE is not a
          repackaging of existing classes but a well-defined, minimal corner of the EFT–DE
          landscape with a unique observational footprint.
        </p>
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
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
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
    apa: `Brown, D. (2025). *Quantum–Kinetic Dark Energy (QKDE).* Zenodo. https://doi.org/10.5281/zenodo.17774687`,
    mla: `Brown, Daniel. *Quantum–Kinetic Dark Energy (QKDE).* Zenodo, 2025, doi:10.5281/zenodo.17774687.`,
    chicago: `Brown, Daniel. 2025. *Quantum–Kinetic Dark Energy (QKDE).* Zenodo. https://doi.org/10.5281/zenodo.17774687.`,
    ieee: `D. Brown, "Quantum–Kinetic Dark Energy (QKDE)," Zenodo, 2025. doi:10.5281/zenodo.17774687.`,
    harvard: `Brown, D. (2025) “Quantum–Kinetic Dark Energy (QKDE).” Zenodo. doi:10.5281/zenodo.17774687.`
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



<footer class="site-footer">
  © 2025 Daniel Brown — Quantum–Kinetic Dark Energy (QKDE)
</footer>
</div> <!-- end page -->

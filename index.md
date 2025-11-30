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

/* Global resets */
body {
  margin: 0;
  padding: 0;
  font-family: "Inter", sans-serif;
  color: #e8e9ef;
  line-height: 1.75;
  background: #000;
  overflow-x: hidden;
}

/* Starfield background */
body {
  background:
    radial-gradient(circle at 20% 20%, rgba(40,60,80,0.4), transparent 70%),
    radial-gradient(circle at 80% 80%, rgba(30,40,60,0.4), transparent 70%),
    black;
}

.star-layer {
  position: fixed;
  top: 0; left: 0;
  width: 200%;
  height: 200%;
  z-index: -2;
  background-image:
    radial-gradient(2px 2px at 20% 30%, rgba(255,255,255,0.9), transparent 60%),
    radial-gradient(2px 2px at 70% 80%, rgba(255,255,255,0.7), transparent 60%),
    radial-gradient(1.5px 1.5px at 40% 60%, rgba(255,255,255,0.8), transparent 60%),
    radial-gradient(1px 1px at 90% 20%, rgba(255,255,255,0.6), transparent 60%);
  animation: drift 140s linear infinite;
  opacity: 0.7;
}

.star-layer:nth-child(1) { animation-duration: 220s; opacity: 0.45; }
.star-layer:nth-child(2) { animation-duration: 150s; opacity: 0.7; }
.star-layer:nth-child(3) { animation-duration: 90s; opacity: 0.9; }

@keyframes drift {
  from { transform: translate(0,0); }
  to   { transform: translate(-400px, -400px); }
}

/* Page container */
.page {
  max-width: 900px;
  margin: 90px auto;
  background: rgba(10, 13, 20, 0.70);
  padding: 50px;
  border-radius: 18px;
  border: 1px solid rgba(102,252,241,0.12);
  box-shadow: 0 0 35px rgba(102,252,241,0.18);
  backdrop-filter: blur(12px);
}

/* Headings (no bold) */
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
  margin-bottom: 15px;
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

.social-box {
  background: rgba(15, 22, 32, 0.45);
  padding: 18px 25px;
  border-radius: 12px;
  border: 1px solid rgba(102,252,241,0.10);
  margin-top: 25px;
}

.social-link {
  display: block;
  color: #aeeaff;
  text-decoration: none;
  margin-bottom: 8px;
  transition: 0.2s ease;
}

.social-link:hover {
  color: #66fcf1;
  text-shadow: 0 0 8px rgba(102,252,241,0.8);
}

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
  font-size: 1.1rem;
  border-radius: 7px;
  text-decoration: none;
  transition: 0.2s;
}

.paper-button:hover {
  background: #bfe6f7;
  box-shadow: 0 0 16px rgba(174,234,255,0.8);
}

.center { text-align: center; }

</style>

<!-- Stars -->
<div class="star-layer"></div>
<div class="star-layer"></div>
<div class="star-layer"></div>

<div class="page">

<h1>Quantum–Kinetic Dark Energy (QKDE)</h1>
<p style="text-align:center; margin-top:-10px; font-style: italic;">
A GR-preserving, background-only extension of ΛCDM
</p>

<!-- Author -->
<div class="author-box">
  <img src="photoDaniel.jpg" alt="Author photo" class="author-photo">

  <div>
    <h2>Daniel Brown</h2>
    <p>Cosmology enthusiast and independent researcher</p>
    <p>Graduate of the University of Utah</p>
    <p>Research interests: dark energy, scalar fields, late-time expansion</p>
    <p>Based in Salt Lake City, Utah</p>
  </div>
</div>

<div class="social-box">
  <a href="https://orcid.org/0009-0001-8082-9702" class="social-link" target="_blank">ORCID</a>
  <a href="https://github.com/DanielBrown124/QKDE" class="social-link" target="_blank">GitHub Repository</a>
  <a href="https://doi.org/10.5281/zenodo.17757109" class="social-link" target="_blank">Zenodo DOI</a>
  <a href="https://independent.academia.edu/DanielBrown462" class="social-link" target="_blank">Academia.edu</a>
</div>

<hr>

<h2>What This Work Proposes</h2>

<div class="paper-box">

<h3>1. A minimal and GR-respecting dark energy model</h3>

<p>QKDE introduces a time-dependent kinetic normalization for a scalar field while leaving General Relativity fully intact. The scalar sector is</p>

\[
P(X,\phi,t) = K(t)\,X - V(\phi), \qquad K(t) > 0,
\]

\[
X = -\tfrac12 g^{\mu\nu}\partial_\mu\phi\,\partial_\nu\phi.
\]

<p>This structure arises naturally from curvature-suppressed operators in quantum field theory in curved spacetime.</p>

<hr>

<h3>2. Gravity remains exactly Einsteinian</h3>

<p>The Einstein–Hilbert metric sector is unchanged. This implies:</p>

<p>Gravitational waves propagate at the speed of light</p>
<p>The Planck mass is constant</p>
<p>No braiding or fifth forces are generated</p>
<p>No gravitational slip</p>

\[
\Phi = \Psi
\]

<hr>

<h3>3. Observable effects originate only from background evolution</h3>

<p>The model predicts deviations from ΛCDM solely through</p>

\[
H(a), \qquad D(a),
\]

<p>not through modified perturbations or new forces.</p>

<hr>

<h3>4. EFT of Dark Energy characterization</h3>

\[
\alpha_K > 0,
\]

\[
\alpha_B = \alpha_M = \alpha_T = \alpha_H = 0.
\]

<p>This places QKDE in the GR-preserving corner of EFT–DE.</p>

<hr>

<h3>5. Two forms of K(t)</h3>

<p>Curvature-based:</p>

\[
K = 1 + \frac{\alpha R}{M^2}
\]

<p>Running parameterization:</p>

\[
K = 1 + K_0 (1+z)^p
\]

<div class="center" style="margin-top: 35px;">
  <a class="paper-button" href="Quantum_Kinetic_Dark_Energy_QKDE.pdf">
    QKDE Paper (PDF)
  </a>
</div>

</div> <!-- end paper-box -->

</div> <!-- end page -->

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
}

.ref-list li {
  margin-bottom: 6px;
}

</style>

<!-- Stars -->
<div class="star-layer"></div>
<div class="star-layer"></div>
<div class="star-layer"></div>

<div class="page">

<h1>Quantum–Kinetic Dark Energy (QKDE)</h1>
<p style="text-align:center; margin-top:-10px; font-style: italic;">
An effective dark energy framework with the Einstein–Hilbert metric sector intact and a time-dependent scalar kinetic normalization
</p>

<div class="author-box">
  <img src="photoDaniel.jpg" alt="Author photo" class="author-photo">

  <div>
    <h2>Daniel Brown</h2>
    <p>Cosmology enthusiast and independent researcher</p>
    <p>Graduate of the University of Utah</p>
    <p>Investigating dark energy, scalar fields, and late-time cosmic expansion</p>
    <p>Based in Salt Lake City, Utah</p>
  </div>
</div>

<div class="social-box">

  <a href="https://orcid.org/0009-0001-8082-9702" class="social-link" target="_blank">
    <span class="social-icon">
      <!-- ORCID logo (simplified circular) -->
      <svg viewBox="0 0 24 24" aria-hidden="true">
        <circle cx="12" cy="12" r="10.5" />
        <rect x="10.4" y="7.2" width="1.8" height="9.6" />
        <path d="M14.2 9.2a2.5 2.5 0 0 1 0 5h-.9v-1.4h.8a1.1 1.1 0 0 0 0-2.2h-.8V9.2z" />
      </svg>
    </span>
    <span>ORCID</span>
  </a>

  <a href="https://github.com/DanielBrown124/QKDE" class="social-link" target="_blank">
    <span class="social-icon">
      <!-- GitHub mark (simplified) -->
      <svg viewBox="0 0 24 24" aria-hidden="true">
        <path d="M12 1.5A10.5 10.5 0 0 0 1.5 12c0 4.63 3 8.56 7.17 9.95.53.1.73-.23.73-.5v-1.75c-2.92.64-3.54-1.4-3.54-1.4-.48-1.2-1.17-1.52-1.17-1.52-.96-.65.07-.63.07-.63 1.06.08 1.62 1.1 1.62 1.1.95 1.63 2.5 1.16 3.11.89.1-.7.37-1.16.68-1.43-2.33-.27-4.78-1.18-4.78-5.25 0-1.16.42-2.1 1.1-2.84-.11-.27-.48-1.36.1-2.83 0 0 .9-.29 2.95 1.08a10.1 10.1 0 0 1 5.38 0c2.05-1.37 2.95-1.08 2.95-1.08.58 1.47.21 2.56.1 2.83.68.74 1.1 1.68 1.1 2.84 0 4.08-2.45 4.98-4.79 5.25.38.33.73.97.73 1.96v2.9c0 .27.2.6.73.5A10.52 10.52 0 0 0 22.5 12 10.5 10.5 0 0 0 12 1.5Z" />
      </svg>
    </span>
    <span>GitHub Repository</span>
  </a>

  <a href="https://doi.org/10.5281/zenodo.17757109" class="social-link" target="_blank">
    <span class="social-icon">
      <!-- Zenodo-like badge (simplified) -->
      <svg viewBox="0 0 24 24" aria-hidden="true">
        <rect x="3" y="4" width="18" height="16" rx="3" />
        <path d="M9 9h6v1.5H11.3L15 14.9V16H9v-1.5h3.7L9 10.1z" />
      </svg>
    </span>
    <span>Zenodo DOI</span>
  </a>

  <a href="https://independent.academia.edu/DanielBrown462" class="social-link" target="_blank">
    <span class="social-icon">
      <!-- Academia-like tower mark (simplified) -->
      <svg viewBox="0 0 24 24" aria-hidden="true">
        <path d="M12 3 4.5 20.5h2.4l1.6-4h7l1.6 4h2.4zm-1.8 11.1L12 7.9l1.8 6.2z" />
      </svg>
    </span>
    <span>Academia.edu</span>
  </a>

</div>

<hr>

<h2>What This Work Proposes</h2>

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
  <a class="paper-button" href="Quantum_Kinetic_Dark_Energy_QKDE.pdf">
    QKDE Paper (PDF)
  </a>
</div>

</div> <!-- end paper-box -->

<hr>

<details>
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

<details>
  <summary><span class="summary-label">References</span></summary>
  <div class="details-body">

    <ol class="ref-list">
      <li>B. P. Abbott et al. GW170817: Observation of gravitational waves from a binary neutron star inspiral. Physical Review Letters, 119:161101, 2017. doi: 10.1103/PhysRevLett.119.161101.</li>
      <li>Jeremy Sakstein and Bhuvnesh Jain. Implications of the neutron star merger GW170817 for cosmological scalar-tensor theories. Physical Review Letters, 119:251303, 2017. doi: 10.1103/PhysRevLett.119.251303.</li>
      <li>Giulia Gubitosi, Federico Piazza, and Filippo Vernizzi. The effective field theory of dark energy. JCAP, 02:032, 2013. doi: 10.1088/1475-7516/2013/02/032.</li>
      <li>Jolyon K. Bloomfield, Eanna E. Flanagan, Minjoon Park, and Scott Watson. Dark energy or modified gravity? An effective field theory approach. JCAP, 08:010, 2013. doi: 10.1088/1475-7516/2013/08/010.</li>
      <li>Emiliano Bellini and Ignacy Sawicki. Maximal freedom at minimum cost: Linear large-scale structure in general modifications of gravity. JCAP, 07:050, 2014. doi: 10.1088/1475-7516/2014/07/050.</li>
      <li>Jaume Garriga and Viatcheslav Mukhanov. Perturbations in k-inflation. Physics Letters B, 458:219–225, 1999. doi: 10.1016/S0370-2693(99)00602-4.</li>
      <li>N. D. Birrell and P. C. W. Davies. Quantum Fields in Curved Space. Cambridge University Press, 1982. doi: 10.1017/CBO9780511622632.</li>
      <li>Leonard Parker. Particle creation in expanding universes. Physical Review, 183:1057–1068, 1969. doi: 10.1103/PhysRev.183.1057.</li>
      <li>Leonard Parker and Stephen A. Fulling. Adiabatic regularization of the energy-momentum tensor of a quantum field in homogeneous cosmologies. Physical Review D, 9:341–354, 1974. doi: 10.1103/PhysRevD.9.341.</li>
      <li>T. S. Bunch. Calculation of the renormalized stress tensor in de Sitter space via point-splitting. Journal of Physics A, 13:1297, 1980. doi: 10.1088/0305-4470/13/4/022.</li>
      <li>I. L. Buchbinder, S. D. Odintsov, and I. L. Shapiro. Effective Action in Quantum Gravity. IOP Publishing, 1992.</li>
      <li>Leonard Parker and David J. Toms. Quantum Field Theory in Curved Spacetime. Cambridge University Press, 2009. doi: 10.1017/CBO9780511813924.</li>
      <li>A. O. Barvinsky and G. A. Vilkovisky. The generalized Schwinger–DeWitt technique in gauge theories and quantum gravity. Physics Reports, 119:1–74, 1985.</li>
      <li>John F. Donoghue. General relativity as an effective field theory: The leading quantum corrections. Physical Review D, 50:3874–3888, 1994. doi: 10.1103/PhysRevD.50.3874.</li>
      <li>Bharat Ratra and P. J. E. Peebles. Cosmological consequences of a rolling homogeneous scalar field. Astrophysical Journal Letters, 325:L17–L20, 1988. doi: 10.1086/185100.</li>
      <li>Robert R. Caldwell, Rahul Dave, and Paul J. Steinhardt. Cosmological imprint of an energy component with general equation of state. Physical Review Letters, 80:1582–1585, 1998. doi: 10.1103/PhysRevLett.80.1582.</li>
      <li>Cristian Armendariz-Picon, Viatcheslav Mukhanov, and Paul Steinhardt. Essentials of k-essence. Physical Review D, 63:103510, 2001. doi: 10.1103/PhysRevD.63.103510.</li>
      <li>Chung-Pei Ma and Edmund Bertschinger. Cosmological perturbation theory in the synchronous and conformal Newtonian gauges. Astrophysical Journal, 455:7–25, 1995. doi: 10.1086/176550.</li>
      <li>Planck Collaboration. Planck 2018 results. VI. Cosmological parameters. Astronomy and Astrophysics, 641:A6, 2020. doi: 10.1051/0004-6361/201833910.</li>
      <li>Eric V. Linder. Cosmic growth history and expansion history. Physical Review D, 72:043529, 2005. doi: 10.1103/PhysRevD.72.043529.</li>
      <li>Daniel J. Eisenstein et al. Detection of the baryon acoustic peak in the large-scale correlation function of SDSS luminous red galaxies. Astrophysical Journal, 633:560–574, 2005. doi: 10.1086/466512.</li>
      <li>Clifford Cheung, Paolo Creminelli, A. Liam Fitzpatrick, Jared Kaplan, and Leonardo Senatore. The effective field theory of inflation. Journal of High Energy Physics, 2008(03):014, 2008. doi: 10.1088/1126-6708/2008/03/014.</li>
      <li>Viatcheslav Mukhanov. Physical Foundations of Cosmology. Cambridge University Press, 2005. doi: 10.1017/CBO9780511790553.</li>
      <li>Scott Dodelson. Modern Cosmology. Academic Press, 2003.</li>
      <li>Earl A. Coddington and Norman Levinson. Theory of Ordinary Differential Equations. McGraw–Hill, 1955.</li>
      <li>C. P. Burgess. Quantum gravity in everyday life: General relativity as an effective field theory. Living Reviews in Relativity, 7:5, 2004. doi: 10.12942/lrr-2004-5.</li>
      <li>Éric Aubourg, Stephen Bailey, Julian E. Bautista, et al. Cosmological implications of baryon acoustic oscillation measurements. Physical Review D, 92:123516, 2015. doi: 10.1103/PhysRevD.92.123516.</li>
      <li>Planck Collaboration. Planck 2018 results. VI. Cosmological parameters. Astronomy and Astrophysics, 641:A6, 2020. doi: 10.1051/0004-6361/201833910.</li>
      <li>Steven Weinberg. The Quantum Theory of Fields, Volume II: Modern Applications. Cambridge University Press, 1996.</li>
      <li>Michael E. Peskin and Daniel V. Schroeder. An Introduction to Quantum Field Theory. Westview Press, 1995.</li>
      <li>Michel Chevallier and David Polarski. Accelerating universes with scaling dark matter? International Journal of Modern Physics D, 10:213–224, 2001. doi: 10.1142/S0218271801000822.</li>
      <li>Eric V. Linder. Exploring the expansion history of the universe. Physical Review Letters, 90:091301, 2003. doi: 10.1103/PhysRevLett.90.091301.</li>
      <li>Antonio De Felice and Shinji Tsujikawa. \(f(R)\) theories. Living Reviews in Relativity, 13:3, 2010. doi: 10.12942/lrr-2010-3.</li>
      <li>Steven Weinberg. Cosmology. Oxford University Press, 2008.</li>
      <li>Austin Joyce, Bhuvnesh Jain, Justin Khoury, and Mark Trodden. Beyond the cosmological standard model. Physics Reports, 568:1–98, 2015. doi: 10.1016/j.physrep.2014.12.002.</li>
      <li>Tsutomu Kobayashi. Horndeski theory and beyond. Reports on Progress in Physics, 82:086901, 2019. doi: 10.1088/1361-6633/ab2429.</li>
      <li>Jeremy Gleyzes, David Langlois, Federico Piazza, and Filippo Vernizzi. Healthy theories beyond Horndeski. Physical Review Letters, 114:211101, 2015. doi: 10.1103/PhysRevLett.114.211101.</li>
      <li>Thomas P. Sotiriou and Valerio Faraoni. \(f(R)\) theories of gravity. Reviews of Modern Physics, 82:451–497, 2010. doi: 10.1103/RevModPhys.82.451.</li>
      <li>Timothy Clifton, Pedro G. Ferreira, Antonio Padilla, and Constantinos Skordis. Modified gravity and cosmology. Physics Reports, 513:1–189, 2012. doi: 10.1016/j.physrep.2012.01.001.</li>
      <li>David W. Hogg. Distance measures in cosmology, 1999.</li>
      <li>Charles Alcock and Bohdan Paczyński. An evolution free test for non-zero cosmological constant? Nature, 281:358–359, 1979. doi: 10.1038/281358a0.</li>
      <li>Wayne Hu and Naoshi Sugiyama. Small-scale cosmological perturbations: An analytic approach. Astrophysical Journal, 471:542–570, 1996. doi: 10.1086/177989.</li>
      <li>Daniel J. Eisenstein and Wayne Hu. Baryonic features in the matter transfer function. Astrophysical Journal, 496:605–614, 1998. doi: 10.1086/305424.</li>
      <li>P. J. E. Peebles. The Large-Scale Structure of the Universe. Princeton University Press, 1980.</li>
      <li>Yong-Seon Song and Will J. Percival. Reconstructing the redshift-space distortion parameter beta from galaxy power spectrum measurements. JCAP, 10:004, 2009. doi: 10.1088/1475-7516/2009/10/004.</li>
      <li>D. N. Limber. The analysis of counts of the extragalactic nebulae in terms of a fluctuating density field. Astrophysical Journal, 119:655, 1954. doi: 10.1086/145870.</li>
      <li>Marilena LoVerde and Niayesh Afshordi. Extended Limber approximation. Physical Review D, 78:123506, 2008. doi: 10.1103/PhysRevD.78.123506.</li>
      <li>Matthias Bartelmann and Peter Schneider. Weak gravitational lensing. Physics Reports, 340:291–472, 2001. doi: 10.1016/S0370-1573(00)00082-X.</li>
      <li>R. K. Sachs and A. M. Wolfe. Perturbations of a cosmological model and angular variations of the microwave background. Astrophysical Journal, 147:73–90, 1967. doi: 10.1086/148982.</li>
      <li>J. R. Dormand and P. J. Prince. A family of embedded Runge–Kutta formulae. Journal of Computational and Applied Mathematics, 6:19–26, 1980. doi: 10.1016/0771-050X(80)90013-3.</li>
      <li>Ernst Hairer, Syvert P. Norsett, and Gerhard Wanner. Solving Ordinary Differential Equations I: Nonstiff Problems. Springer, 1993.</li>
      <li>R. Piessens, E. de Doncker-Kapenga, C. W. Uberhuber, and D. Kahaner. QUADPACK: A Subroutine Package for Automatic Integration. Springer, 1983.</li>
      <li>Max Tegmark, Andy Taylor, and Alan Heavens. Karhunen–Loève eigenmode analysis of galaxy redshift surveys. Astrophysical Journal, 480:22–35, 1997. doi: 10.1086/303939.</li>
      <li>Max Tegmark. Measuring cosmological parameters with galaxy surveys. Physical Review Letters, 79:3806–3809, 1997. doi: 10.1103/PhysRevLett.79.3806.</li>
      <li>Yong-Seon Song and Will J. Percival. Reconstructing the redshift-space distortion parameter beta from galaxy power spectrum measurements. JCAP, 10:004, 2009. doi: 10.1088/1475-7516/2009/10/004.</li>
      <li>R. E. Smith, J. A. Peacock, A. Jenkins, et al. Stable clustering, the halo model and nonlinear cosmological power spectra. Monthly Notices of the Royal Astronomical Society, 341:1311–1332, 2003. doi: 10.1046/j.1365-8711.2003.06503.x.</li>
      <li>Ryuichi Takahashi, Masanori Sato, Takahiro Nishimichi, Atsushi Taruya, and Masamune Oguri. Revising the halofit model for the nonlinear matter power spectrum. Astrophysical Journal, 761:152, 2012. doi: 10.1088/0004-637X/761/2/152.</li>
      <li>Robert M. Wald. General Relativity. University of Chicago Press, 1984.</li>
      <li>Misao Sasaki. Large scale quantum fluctuations in the inflationary universe. Progress of Theoretical Physics, 76:1036–1046, 1986. doi: 10.1143/PTP.76.1036.</li>
      <li>Viatcheslav F. Mukhanov. Quantum theory of gauge invariant cosmological perturbations. Soviet Physics JETP, 67:1297–1302, 1988.</li>
      <li>Hideo Kodama and Misao Sasaki. Cosmological perturbation theory. Progress of Theoretical Physics Supplement, 78:1–166, 1984. doi: 10.1143/PTPS.78.1.</li>
      <li>Rachel Bean and Olivier Doré. Probing dark energy perturbations: The dark energy equation of state and speed of sound as measured by WMAP. Physical Review D, 69:083503, 2004. doi: 10.1103/PhysRevD.69.083503.</li>
      <li>Wayne Hu. Structure formation with generalized dark matter. Astrophysical Journal, 506:485–494, 1998. doi: 10.1086/306274.</li>
      <li>Luca Amendola and Shinji Tsujikawa. Dark Energy: Theory and Observations. Cambridge University Press, 2010. doi: 10.1017/CBO9780511750823.</li>
    </ol>

  </div>
</details>

</div> <!-- end page -->

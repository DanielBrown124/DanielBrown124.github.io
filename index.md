---
layout: none
title: Quantum–Kinetic Dark Energy (QKDE)
---

<!-- ============================
     COSMOLOGY THEME + FONTS
     ============================ -->

<!-- Load MathJax for LaTeX equations -->
<script>
  window.MathJax = {
    tex: {inlineMath: [['$','$'], ['\\(','\\)']]}
  };
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<style>

/* Cosmic background */
body {
  margin: 0;
  padding: 0;
  background: linear-gradient(135deg, #0b0c10, #121725 70%);
  color: #e8e9eb;
  font-family: "Inter", sans-serif;
  line-height: 1.75;
}

/* Page wrapper */
.page {
  max-width: 900px;
  margin: 70px auto;
  background: rgba(15, 20, 30, 0.57);
  padding: 50px;
  border-radius: 18px;
  box-shadow: 0 0 30px rgba(102, 252, 241, 0.25);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(102, 252, 241, 0.12);
}

/* Headings */
h1, h2 {
  font-family: "Merriweather", serif;
  color: #66fcf1;
  margin-top: 0;
}

h1 {
  text-align: center;
  margin-bottom: 10px;
}

/* AUTHOR CARD */
.author-box {
  display: flex;
  gap: 25px;
  align-items: center;
  background: rgba(10, 15, 22, 0.55);
  padding: 25px;
  border-radius: 14px;
  margin-bottom: 50px;
  box-shadow: inset 0 0 15px rgba(102, 252, 241, 0.1),
              0 0 15px rgba(102, 252, 241, 0.15);
  border: 1px solid rgba(102, 252, 241, 0.12);
}

.author-photo {
  width: 135px;
  height: 135px;
  object-fit: cover;
  border-radius: 10px;
  box-shadow: 0 0 20px rgba(102, 252, 241, 0.35);
  border: 2px solid rgba(102, 252, 241, 0.2);
}

.author-info h2 {
  margin: 0 0 6px 0;
  color: #66fcf1;
  font-size: 1.6rem;
}

.author-info p {
  margin: 4px 0;
  opacity: 0.9;
}

/* Section divider */
hr {
  border: none;
  height: 1px;
  margin: 50px 0;
  background: linear-gradient(to right, transparent, #45a29e, transparent);
}

/* PAPER BOX */
.paper-box {
  background: rgba(12, 17, 26, 0.55);
  padding: 30px 28px;
  border-radius: 14px;
  box-shadow: 0 0 20px rgba(102, 252, 241, 0.15);
  border: 1px solid rgba(102, 252, 241, 0.1);
  transition: 0.25s ease;
}

.paper-box:hover {
  transform: translateY(-4px);
  box-shadow: 0 0 28px rgba(102, 252, 241, 0.25);
}

/* PAPER BUTTON */
.paper-button {
  display: inline-block;
  padding: 14px 32px;
  background: #66fcf1;
  color: #0b0c10;
  font-weight: 700;
  font-size: 1.08rem;
  border-radius: 8px;
  text-decoration: none;
  box-shadow: 0 0 18px rgba(102, 252, 241, 0.7);
  transition: 0.22s ease;
}

.paper-button:hover {
  background: #3fc7c1;
  box-shadow: 0 0 28px rgba(102, 252, 241, 1);
}

/* Centering helper */
.center { text-align: center; }
</style>


<!-- ============================
          PAGE CONTENT
     ============================ -->

<div class="page">

# Quantum–Kinetic Dark Energy (QKDE)
### *A GR-Preserving, Background-Only Extension of ΛCDM*

---

<!-- ABOUT THE AUTHOR FIRST -->
<div class="author-box">
  <img src="photoDaniel.jpg" alt="Daniel Brown" class="author-photo">
  <div class="author-info">
    <h2>Daniel Brown</h2>
    <p><strong>Independent Researcher in Cosmology & Scalar-Field Theory</strong></p>
    <p>Specializing in GR-consistent models of cosmic acceleration.</p>
    <p>Focus areas: EFT of DE, scalar-field dynamics, QFT in curved spacetime.</p>
  </div>
</div>

<hr>

<!-- PAPER SECTION SECOND -->
<section class="paper-box">

## 📘 What This Paper Proposes

**QKDE introduces a new dark-energy framework where gravity is *fully unchanged*.**  
Instead, the only modification occurs in the scalar sector:

### **The Lagrangian**
\[
P(X,\phi,t) = K(t)\,X - V(\phi), \qquad K(t) > 0,
\]

where  
\[
X = -\tfrac12 g^{\mu\nu}\partial_\mu\phi\,\partial_\nu\phi.
\]

Here, **\(K(t)\)** is a slowly drifting kinetic normalization derived from curvature-suppressed operators in QFT in curved spacetime.

This leads to a dark-energy model that is:

### ✔ Fully GR-preserving
- Einstein–Hilbert action unchanged  
- Planck mass constant  
- Gravitational waves stay luminal  
- No braiding, no fifth forces  
- No gravitational slip:  
  \[
  \Phi = \Psi
  \]

### ✔ Predictive and falsifiable
All observable deviations from ΛCDM appear through:

\[
H(a) \qquad \text{and} \qquad D(a),
\]

not through modified perturbation equations.

### ✔ Clean EFT interpretation
Only **one** EFT-of-DE parameter is active:

\[
\alpha_K = \frac{K\,\dot{\phi}^2}{H^2 M_{\rm pl}^2} > 0,
\]

while  
\[
\alpha_B = \alpha_M = \alpha_T = \alpha_H = 0.
\]

### ✔ Two forms of \(K(t)\) explored
- **Curvature-driven:**  
  \[
  K = 1 + \frac{\alpha R}{M^2}
  \]
- **Phenomenological running:**  
  \[
  K = 1 + K_0 (1+z)^{p}
  \]

### ✔ Includes:
- Closed background system in e-folds  
- Full linear perturbation theory  
- Exact sensitivity-based forecast pipeline  
- Numerical stability & admissibility checks  
- Null tests:  
  \[
  \mu = \Sigma = 1, \quad \text{slip} = 0
  \]

---

<div class="center" style="margin-top: 35px;">
  <a class="paper-button" href="Quantum_Kinetic_Dark_Energy_QKDE.pdf">
    📄 Download: *Quantum–Kinetic Dark Energy (QKDE)*
  </a>
</div>

</section>

</div>

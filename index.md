---
layout: none
title: Quantum–Kinetic Dark Energy (QKDE): An effective dark energy framework with the Einstein–Hilbert metric sector intact and a time–dependent scalar kinetic normalization
---

<!-- MathJax for LaTeX -->
<script>
  window.MathJax = { tex: { inlineMath: [['$','$'], ['\\(','\\)']] } };
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<!-- ============================
     GLOBAL STYLE + STARFIELD
     ============================ -->

<style>

/* Reset + font */
body {
  margin: 0;
  padding: 0;
  font-family: "Inter", sans-serif;
  color: #e8e9ef;
  line-height: 1.7;
  background: #000; /* fallback */
  overflow-x: hidden;
}

/* NEW WORKING STARFIELD (layered gradients + animation) */
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
.star-layer:nth-child(3) { animation-duration: 90s;  opacity: 0.9; }

@keyframes drift {
  from { transform: translate(0,0); }
  to   { transform: translate(-400px, -400px); }
}

/* ============================
           PAGE WRAPPER
   ============================ */

.page {
  max-width: 900px;
  margin: 90px auto;
  background: rgba(10, 13, 20, 0.70);
  backdrop-filter: blur(12px);
  padding: 50px;
  border-radius: 18px;
  border: 1px solid rgba(102,252,241,0.12);
  box-shadow: 0 0 35px rgba(102,252,241,0.18);
}

/* Headings */
h1, h2 {
  font-family: "Merriweather", serif;
  color: #9be7ff;
}

h1 {
  text-align: center;
  margin-bottom: 12px;
  font-size: 2.4rem;
}

h2 {
  margin-top: 35px;
  margin-bottom: 12px;
  font-size: 1.75rem;
}

/* Divider */
hr {
  border: none;
  height: 1px;
  background: linear-gradient(to right, transparent, #568ea6, transparent);
  margin: 45px 0;
}

/* ============================
           AUTHOR CARD
   ============================ */

.author-box {
  display: flex;
  gap: 25px;
  align-items: center;
  background: rgba(15, 22, 32, 0.55);
  padding: 25px;
  border-radius: 14px;
  box-shadow: inset 0 0 15px rgba(102,252,241,0.09),
              0 0 18px rgba(102,252,241,0.15);
  border: 1px solid rgba(102,252,241,0.12);
}

.author-photo {
  width: 135px;
  height: 135px;
  border-radius: 10px;
  object-fit: cover;
  box-shadow: 0 0 15px rgba(102,252,241,0.26);
  border: 2px solid rgba(102,252,241,0.22);
}

.author-info p {
  margin: 4px 0;
  opacity: 0.95;
}

/* ============================
         SOCIAL LINKS BOX
   ============================ */

.social-box {
  background: rgba(15, 22, 32, 0.45);
  padding: 18px 25px;
  border-radius: 12px;
  margin-top: 25px;
  margin-bottom: 40px;
  border: 1px solid rgba(102,252,241,0.10);
}

.social-link {
  display: block;
  margin-bottom: 8px;
  color: #aeeaff;
  font-weight: 500;
  text-decoration: none;
  transition: 0.2s ease;
}

.social-link:hover {
  color: #66fcf1;
  text-shadow: 0 0 10px rgba(102,252,241,0.9);
}

/* ============================
         PAPER BOX + BUTTON
   ============================ */

.paper-box {
  background: rgba(15, 22, 32, 0.45);
  padding: 30px;
  border-radius: 14px;
  border: 1px solid rgba(102,252,241,0.10);
  box-shadow: 0 0 20px rgba(102,252,241,0.12);
}

.paper-button {
  display: inline-block;
  padding: 12px 26px;
  background: #aeeaff;
  color: #0b0c10;
  font-weight: 600;
  font-size: 1.15rem;
  border-radius: 7px;
  text-decoration: none;
  transition: 0.2s;
  box-shadow: 0 0 10px rgba(174,234,255,0.5);
}

.paper-button:hover {
  background: #94d9f0;
  box-shadow: 0 0 18px rgba(174,234,255,0.8);
}

/* Helpers */
.center { text-align: center; }

</style>

<!-- Background star layers -->
<div class="star-layer"></div>
<div class="star-layer"></div>
<div class="star-layer"></div>


<!-- ============================
           PAGE CONTENT
   ============================ -->

<div class="page">

# **Quantum–Kinetic Dark Energy (QKDE)**  
### *A GR-Preserving, Background-Only Extension of ΛCDM*

---

## 👤 **About the Author**

<div class="author-box">
  <img src="photoDaniel.jpg" alt="Author photo" class="author-photo">

  <div class="author-info">
    <h2>Daniel Brown</h2>
    <p><strong>Cosmology Enthusiast & Independent Researcher</strong></p>
    <p>Graduate of the University of Utah.</p>
    <p>Investigating dark energy, scalar fields, and late-time cosmic expansion.</p>
    <p>Based in Salt Lake City, Utah.</p>
  </div>
</div>

<!-- Social links -->
<div class="social-box">
  <a href="https://orcid.org/0009-0001-8082-9702" class="social-link" target="_blank">🔗 ORCID</a>
  <a href="https://github.com/DanielBrown124/QKDE" class="social-link" target="_blank">💻 GitHub: QKDE Repo</a>
  <a href="https://doi.org/10.5281/zenodo.17757109" class="social-link" target="_blank">📘 Zenodo (Published DOI)</a>
  <a href="https://independent.academia.edu/DanielBrown462" class="social-link" target="_blank">🎓 Academia.edu</a>
</div>

<hr>

## 📘 **What This Paper Proposes**

<div class="paper-box">

### **A Minimal, GR-Respecting Origin for Dark Energy**

QKDE proposes that cosmic acceleration is not caused by modifying gravity, but by allowing the **scalar kinetic normalization** to drift gently with time:

\[
P(X,\phi,t) = K(t)\,X - V(\phi),\quad K(t) > 0,
\]
\[
X = -\tfrac12 g^{\mu\nu}\partial_\mu\phi\,\partial_\nu\phi.
\]

This idea is motivated by curvature-suppressed operators in **quantum field theory in curved spacetime**, which naturally induce such a running.

---

### **Key Principles**

#### ✔ **Gravity remains fully GR**
- Einstein–Hilbert sector unchanged  
- Planck mass constant  
- Gravitational waves stay luminal  

#### ✔ **No modified-gravity operators**
- No braiding  
- No fifth forces  
- No slip:  
  \[
  \Phi = \Psi
  \]

#### ✔ **Predictive and falsifiable**
All deviations from ΛCDM arise through:
\[
H(a),\quad D(a),
\]
not through modified perturbations.

---

### **EFT-of-DE Mapping**

Only one EFT parameter is active:
\[
\alpha_K > 0,
\]
while
\[
\alpha_B = \alpha_M = \alpha_T = \alpha_H = 0.
\]

---

### **Forms of \(K(t)\) Explored**
- **Curvature-driven:**  
  \[
  K = 1 + \frac{\alpha R}{M^2}
  \]
- **Running form:**  
  \[
  K = 1 + K_0 (1+z)^{p}
  \]

---

<div class="center" style="margin-top: 35px;">
  <a class="paper-button" href="Quantum_Kinetic_Dark_Energy_QKDE.pdf">
    📄 QKDE Paper
  </a>
</div>

</div> <!-- end paper box -->

</div> <!-- end page -->

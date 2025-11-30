---
layout: none
title: Quantum–Kinetic Dark Energy (QKDE)
---

<!-- Load MathJax for LaTeX rendering -->
<script>
  window.MathJax = {
    tex: {inlineMath: [['$','$'], ['\\(','\\)']]}
  };
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<style>

/* ===============================
       STARFIELD BACKGROUND
   =============================== */

body {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
  color: #e8e9eb;
  font-family: "Inter", sans-serif;
  line-height: 1.7;
}

/* 3-layer parallax starfield */
body::before, body::after, body div.starfield {
  content: "";
  position: fixed;
  top: 0; left: 0;
  width: 200%;
  height: 200%;
  pointer-events: none;
  background-repeat: repeat;
  z-index: -3;
}

/* Deep star layer */
body::before {
  background-image: url('https://raw.githubusercontent.com/konpa/devicon/master/icons/html5/html5-original.svg');
  /* Instead of an image, we use CSS-generated stars */
  background: transparent;
  box-shadow:
    1000px 400px #fff,
    400px 800px #fff,
    200px 300px #fff,
    1400px 900px #fff,
    900px 500px #fff,
    1200px 200px #fff;
  animation: drift 120s linear infinite;
}

/* Medium star layer */
body::after {
  background: transparent;
  box-shadow:
    600px 200px #fff,
    200px 900px #fff,
    800px 600px #fff,
    1500px 300px #fff,
    100px 700px #fff;
  animation: drift 180s linear infinite;
}

/* Foreground tiny stars */
div.starfield {
  background: transparent;
  box-shadow:
    300px 400px #fff,
    900px 200px #fff,
    500px 1000px #fff,
    1300px 700px #fff,
    50px 300px #fff;
  animation: drift 300s linear infinite;
}

@keyframes drift {
  from { transform: translate3d(0,0,0); }
  to   { transform: translate3d(-500px, -500px, 0); }
}


/* ===============================
            PAGE WRAPPER
   =============================== */

.page {
  max-width: 900px;
  margin: 80px auto;
  background: rgba(10, 15, 22, 0.65);
  padding: 50px;
  border-radius: 18px;
  backdrop-filter: blur(12px);
  border: 1px solid rgba(102, 252, 241, 0.13);
  box-shadow: 0 0 36px rgba(102, 252, 241, 0.25);
}

/* Headings */
h1, h2 {
  font-family: "Merriweather", serif;
  color: #66fcf1;
  margin-top: 0;
}

h1 {
  text-align: center;
  margin-bottom: 12px;
}

/* ===============================
            AUTHOR BOX
   =============================== */

.author-box {
  display: flex;
  gap: 25px;
  align-items: center;
  background: rgba(12, 18, 27, 0.55);
  padding: 25px;
  border-radius: 14px;
  margin-bottom: 50px;
  box-shadow: inset 0 0 15px rgba(102,252,241,0.08), 0 0 15px rgba(102,252,241,0.12);
  border: 1px solid rgba(102, 252, 241, 0.12);
}

.author-photo {
  width: 135px;
  height: 135px;
  object-fit: cover;
  border-radius: 10px;
  box-shadow: 0 0 20px rgba(102,252,241,0.33);
  border: 2px solid rgba(102,252,241,0.25);
}

.author-info h2 {
  margin: 0 0 6px 0;
  font-size: 1.6rem;
}

.author-info p {
  margin: 4px 0;
  opacity: 0.95;
}

/* Section divider */
hr {
  border: none;
  height: 1px;
  background: linear-gradient(to right, transparent, #45a29e, transparent);
  margin: 50px 0;
}

/* ===============================
            PAPER BOX
   =============================== */

.paper-box {
  background: rgba(12, 17, 26, 0.55);
  padding: 30px;
  border-radius: 14px;
  border: 1px solid rgba(102, 252, 241, 0.1);
  box-shadow: 0 0 20px rgba(102,252,241,0.12);
  transition: 0.25s ease;
}

.paper-box:hover {
  transform: translateY(-4px);
  box-shadow: 0 0 28px rgba(102,252,241,0.25);
}

/* Button */
.paper-button {
  display: inline-block;
  padding: 14px 32px;
  background: #66fcf1;
  color: #0b0c10;
  font-weight: 700;
  font-size: 1.1rem;
  border-radius: 8px;
  text-decoration: none;
  box-shadow: 0 0 22px rgba(102,252,241,0.7);
  transition: 0.22s ease;
}

.paper-button:hover {
  background: #3fc7c1;
  box-shadow: 0 0 28px rgba(102,252,241,1);
}

.center { text-align: center; }

</style>

<div class="starfield"></div>


<!-- ===============================
           PAGE CONTENT
   =============================== -->

<div class="page">

# **Quantum–Kinetic Dark Energy (QKDE)**  
### *A GR-Preserving, Background-Only Extension of ΛCDM*

---

## 👤 **About the Author**

<div class="author-box">
  <img src="photoDaniel.jpg" alt="Daniel Brown" class="author-photo">
  <div class="author-info">
    <h2>Daniel Brown</h2>
    <p><strong>Cosmology Enthusiast & Independent Researcher</strong></p>
    <p>Graduate of the University of Utah.</p>
    <p>Investigating the mysteries of dark energy, scalar fields, and cosmic expansion.</p>
    <p>Based in Salt Lake City, Utah.</p>
  </div>
</div>

<hr>

## 📘 **What This Paper Proposes**

<div class="paper-box">

**Quantum–Kinetic Dark Energy (QKDE)** introduces a dark-energy model where **General Relativity is fully preserved**, and the only modification comes from a gently time-varying **kinetic normalization**:

\[
P(X,\phi,t) = K(t)\,X - V(\phi), \qquad K(t) > 0,
\]
\[
X = -\tfrac12 g^{\mu\nu}\partial_\mu\phi\,\partial_\nu\phi.
\]

### 🔹 Why this matters  
Instead of altering gravity, QKDE treats late-time cosmic acceleration as an imprint of quantum-field corrections in curved spacetime, which naturally introduce a drifting \(K(t)\).

### 🔹 Key Predictions  
- Gravity stays exactly GR  
- Gravitational waves remain luminal  
- No fifth forces, no braiding  
- No gravitational slip:  
  \[
  \Phi = \Psi
  \]
- Linear structure formation follows GR  
- **All deviations from ΛCDM come from \(H(a)\) and \(D(a)\)**

### 🔹 EFT-of-DE Mapping  
Only one EFT parameter is active:
\[
\alpha_K > 0,
\]
while  
\[
\alpha_B = \alpha_M = \alpha_T = \alpha_H = 0.
\]

### 🔹 Forms of \(K(t)\) explored  
- Curvature-driven:  
  \[
  K = 1 + \frac{\alpha R}{M^2}
  \]
- Phenomenological running:  
  \[
  K = 1 + K_0 (1+z)^p
  \]

---

<div class="center" style="margin-top: 30px;">
  <a class="paper-button" href="Quantum_Kinetic_Dark_Energy_QKDE.pdf">
    📄 Download the Full QKDE Paper (PDF)
  </a>
</div>

</div> <!-- end paper box -->

</div> <!-- end page -->

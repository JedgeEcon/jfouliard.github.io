---
permalink: /
title: "Jérémy Fouliard"
---

<style>
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  margin: 0;
  padding: 0;
  color: #222;
  line-height: 1.6;
  background-color: #f9f9f9;
}

a {
  color: #0366d6;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

/* Sidebar discrète */
.sidebar {
  position: fixed;
  left: 0;
  top: 0;
  width: 60px;
  height: 100%;
  background-color: #fff;
  border-right: 1px solid #e1e4e8;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 2em;
}

.sidebar a.github-icon {
  font-size: 28px;
  margin-top: 1em;
  color: #0366d6;
}

/* Contenu principal */
.main-content {
  margin-left: 80px;
  padding: 2em;
  max-width: 900px;
  margin-right: auto;
  margin-left: auto;
}

/* Nom principal */
.main-content h1 {
  font-size: 3em;
  margin-bottom: 0.2em;
  font-weight: 700;
  color: #111;
}

/* Profile container */
.profile-container {
  display: flex;
  flex-wrap: wrap;
  align-items: flex-start;
  margin-top: 2em;
  margin-bottom: 2em;
}

.profile-picture {
  flex: 0 0 300px;
  margin-right: 2em;
}

.profile-picture img {
  width: 300px;
  height: 300px;
  object-fit: cover;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  border: 2px solid #ddd;
}

.profile-text {
  flex: 1;
  font-size: 1.2em;
  line-height: 1.5em;
}

.profile-info {
  margin-top: 1.5em;
  font-size: 1.1em;
}

.profile-info a {
  margin-right: 1.5em;
  font-weight: bold;
}

/* Section titles */
h2.section-title {
  font-size: 2em;
  margin-top: 2em;
  margin-bottom: 0.8em;
  border-bottom: 2px solid #e1e4e8;
  padding-bottom: 0.2em;
}

/* Details style */
details summary {
  font-weight: bold;
  cursor: pointer;
  margin-top: 0.5em;
}

details p {
  margin: 0.5em 0 1em 0;
}

/* Responsive */
@media (max-width: 768px) {
  .sidebar {
    position: relative;
    width: 100%;
    height: auto;
    flex-direction: row;
    justify-content: flex-end;
    border-right: none;
    border-bottom: 1px solid #e1e4e8;
    padding: 1em;
  }
  .main-content {
    margin-left: 0;
    padding: 1em;
  }
  .profile-container {
    flex-direction: column;
    align-items: center;
  }
  .profile-picture {
    margin-right: 0;
    margin-bottom: 1em;
  }
  .profile-text {
    text-align: center;
  }
}
</style>

<!-- Sidebar -->
<div class="sidebar">
  <a href="https://github.com/JedgeEcon" target="_blank" class="github-icon">
    &#xf09b; <!-- GitHub FontAwesome icon -->
  </a>
</div>

<div class="main-content">
  <h1>Jérémy Fouliard</h1>

  <div class="profile-container">
    <div class="profile-picture">
      <img src="images/jfouliard.jpeg" alt="Jeremy Fouliard">
    </div>
    <div class="profile-text">
      <p>High Civil Servant specialized in Economics and Statistics, and PhD student at the Paris School of Economics.</p>
      <p>My research focuses on macroeconomic forecasting, sequential prediction methods, and financial stability applications. I also study national accounts, profit shifting, crypto-assets measurement, and social exclusion.</p>
    </div>
  </div>

  <div class="profile-info">
    <a href="files/jeremy_fouliard_cv.pdf" target="_blank">[Curriculum Vitae]</a> ·
    <a href="mailto:jeremy.fouliard@insee.fr">jeremy.fouliard@insee.fr</a> ·
    <a href="mailto:jeremy.fouliard@psemail.eu">jeremy.fouliard@psemail.eu</a>
  </div>

  <!-- Working Papers -->
  <h2 class="section-title">Working Papers</h2>
<a href="files/queenpaper.pdf"><strong>Answering the Queen: Machine Learning and Financial Crises</strong></a>
with Michael Howell (CbC), Hélène Rey (LBS), and Vania Stavrakeva (LBS).
Coverage: <a href="https://www.nber.org/papers/w28302">NBER</a>, <a href="https://cepr.org/publications/dp15618">CEPR</a>, <a href="https://www.bis.org/publ/work926.pdf">BIS</a>

<details> <summary>Abstract</summary> <p> Financial crises cause severe economic and social disruptions. We develop a sequential prediction framework based on online learning and model aggregation to forecast systemic financial crises twelve quarters ahead. Our approach guarantees asymptotic outperformance relative to any single forecasting model and allows us to identify which models contribute most to predictive power over time and across countries. </p> </details>

<a href="files/time.pdf"><strong>Is This Time Different? Financial Follies Across Centuries</strong></a>
with Hélène Rey (LBS) and Vania Stavrakeva (LBS)

<details> <summary>Abstract</summary> <p> Using models estimated on pre-1922 data, we show that it is possible to predict the Great Depression of 1929 as well as major systemic financial crises of the 20th and 21st centuries out of sample. </p> </details>

<strong>Predictable Returns</strong>

<details> <summary>Abstract</summary> <p> This paper proposes a market-based indicator of systemic risk in the euro area based on time-varying stock return predictability. Using a multi-task online learning framework and long historical stock market data, we study whether increases in predictability are systematically associated with the buildup of financial crises. </p> </details>

<strong>Volume Output Measurement for Public Education</strong>
with Mats Le Floch (INSEE) and Pauline Mendras (INSEE)

<details> <summary>Abstract</summary> <p> We compare alternative volume measures of nonmarket education output in France and evaluate several quality adjustments, including class size, PISA scores, and teacher experience. Quality adjustments have modest effects on aggregate volume growth. </p> </details>

  <!-- Other Publications (Sociology) -->
  <h2 class="section-title">Other Publications (Sociology)</h2>

<a href="files/exclusion.pdf"><strong>L’exclusion sociale est-elle réductible à la situation d’assistance ?</strong></a>
with Éléonore Richard (DREES)

<details> <summary>Abstract</summary> <p> Using French survey data, we show that perceived social assistance has no additional effect on the feeling of social exclusion once labor market detachment, poverty, country of birth, and geographic isolation are accounted for. </p> </details> 
</div>


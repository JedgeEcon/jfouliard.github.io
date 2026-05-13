---
permalink: /
title: ""
---
<style>
@import url('https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;1,400&family=Outfit:wght@300;400;500&display=swap');

/* ===== Reset & base ===== */
html, body {
  margin: 0;
  padding: 0;
  height: 100%;
}

body {
  font-family: 'EB Garamond', Georgia, serif;
  font-size: 18px;
  line-height: 1.75;
  color: #1a1a1a;
  background: #fafaf8;
}

a {
  color: #1a1a1a;
  text-decoration: underline;
  text-decoration-color: rgba(0,0,0,0.3);
  text-underline-offset: 3px;
  transition: text-decoration-color 0.2s ease;
}

a:hover {
  text-decoration-color: #1a1a1a;
}

.main {
  width: 100% !important;
  max-width: 100% !important;
  margin-top: 2em;
  animation: intro 0.4s both;
  animation-delay: 0.35s;
  padding-left: 0;
}

.article, .page {
  width: 100% !important;
  padding: 0 !important;
}

/* ===== Sticky header ===== */
.header-name {
  position: sticky;
  top: 0;
  width: 100%;
  background: rgba(250, 250, 248, 0.92);
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
  border-bottom: 1px solid rgba(0,0,0,0.08);
  z-index: 100;
}

.header-inner {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.9em 2em;
  max-width: 820px;
  margin: 0 auto;
}

.header-name h1 {
  font-family: 'Outfit', sans-serif;
  font-size: 0.95em;
  font-weight: 400;
  letter-spacing: 0.03em;
  margin: 0;
  color: #1a1a1a;
}

.header-github-mobile {
  display: none;
}

.header-github-desktop {
  display: none;
}

/* ===== Main layout ===== */
.main-content {
  max-width: 820px;
  margin: 0 auto;
  padding: 4em 2em 6em;
}

/* ===== Profile section ===== */
.profile-container {
  display: flex;
  flex-wrap: wrap;
  align-items: flex-start;
  gap: 3.5em;
  margin-bottom: 3em;
}

.profile-picture {
  flex: 0 0 200px;
  position: relative;
}

.profile-picture img {
  width: 100%;
  aspect-ratio: 3/4;
  object-fit: cover;
  border-radius: 4px;
  filter: grayscale(8%);
}

.profile-text {
  flex: 1;
  min-width: 280px;
  font-size: 1em;
}

.profile-text p {
  margin-top: 0;
  margin-bottom: 1.1em;
}

.profile-info {
  margin-top: 2em;
  font-family: 'Outfit', sans-serif;
  font-size: 0.78em;
  font-weight: 400;
  letter-spacing: 0.02em;
  color: #555;
  display: flex;
  flex-wrap: wrap;
  gap: 0.15em 0;
}

.profile-info a {
  color: #444;
  text-decoration: none;
  border-bottom: 1px solid rgba(0,0,0,0.2);
  padding-bottom: 1px;
  transition: border-color 0.2s;
}

.profile-info a:hover {
  border-color: #1a1a1a;
  text-decoration: none;
}

/* ===== Section titles ===== */
h2.section-title {
  font-family: 'Outfit', sans-serif;
  font-size: 0.7em;
  font-weight: 500;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: #888;
  margin-top: 3.5em;
  margin-bottom: 1.5em;
  padding-bottom: 0;
  border-bottom: none;
  border-top: 1px solid #e8e8e4;
  padding-top: 1.8em;
}

/* ===== Publications ===== */
.sub-publications {
  padding-left: 0;
  list-style: none;
}

.publication {
  margin-bottom: 2em;
}

.publication a,
.sub-publications > a {
  font-style: italic;
  font-weight: 500;
  color: #1a1a1a;
  text-decoration: none;
  border-bottom: 1px solid rgba(0,0,0,0.25);
  padding-bottom: 1px;
  transition: border-color 0.2s;
}

.publication a:hover,
.sub-publications > a:hover {
  border-color: #1a1a1a;
}

.publication a strong,
.sub-publications > a strong {
  font-weight: 500;
}

.coauthor {
  font-size: 0.92em;
  color: #777;
  font-style: normal;
}

/* Coverage links */
.sub-publications p a,
.sub-publications > p a {
  font-family: 'Outfit', sans-serif;
  font-size: 0.75em;
  letter-spacing: 0.02em;
  color: #555;
  text-decoration: none;
  border-bottom: 1px solid rgba(0,0,0,0.2);
}

/* ===== Abstract (details/summary) ===== */
details {
  margin-top: 0.8em;
}

details summary {
  font-family: 'Outfit', sans-serif;
  font-size: 0.73em;
  font-weight: 500;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: #999;
  cursor: pointer;
  list-style: none;
  display: inline-flex;
  align-items: center;
  gap: 0.4em;
  transition: color 0.2s;
}

details summary::-webkit-details-marker { display: none; }

details summary::before {
  content: '+';
  font-size: 1.1em;
  font-weight: 300;
  transition: transform 0.2s;
  display: inline-block;
}

details[open] summary::before {
  transform: rotate(45deg);
}

details summary:hover {
  color: #555;
}

details p {
  font-size: 0.92em;
  color: #444;
  line-height: 1.8;
  margin: 1em 0 1em 0;
  padding-left: 1em;
  border-left: 2px solid #e0e0da;
}

/* ===== Responsive ===== */
@media (max-width: 700px) {
  .profile-container {
    flex-direction: column;
    gap: 2em;
  }

  .profile-picture {
    flex: 0 0 auto;
    width: 140px;
    margin: 0 auto;
  }

  .profile-text {
    text-align: left;
  }

  .header-github-mobile {
    display: inline-flex;
    align-items: center;
    gap: 0.3em;
    font-family: 'Outfit', sans-serif;
    font-size: 0.8em;
    color: #555;
    text-decoration: none;
  }

  .header-inner {
    padding: 0.7em 1.2em;
  }

  .main-content {
    padding: 2.5em 1.2em 4em;
  }
}

/* ===== Animations ===== */
@keyframes intro {
  from { opacity: 0; transform: translateY(6px); }
  to   { opacity: 1; transform: translateY(0); }
}
</style>

<!-- ===== Sticky header ===== -->
<header class="header-name">
  <div class="header-inner">
    <h1>Jérémy Fouliard</h1>
    <a class="header-github-mobile" href="https://github.com/JedgeEcon" target="_blank">
      <i class="fa-brands fa-github"></i> GitHub
    </a>
  </div>
</header>

<div class="main-content">

  <!-- ===== Profile ===== -->
  <div class="profile-container">
    <div class="profile-picture">
      <img src="images/jfouliard.jpeg" alt="Jeremy Fouliard">
    </div>

    <div class="profile-text">
      <p>Welcome ! I'm a High Civil Servant specialized in Economics and Statistics, a 
      <a href="https://www.insee.fr/fr/information/8599668">Engineer in Statistics, Economics and Data Science</a> 
      and a PhD student in Economics at the 
      <a href="https://www.parisschoolofeconomics.eu/en/persons/jeremy-fouliard/">Paris School of Economics</a>.</p>

      <p>My research focuses on macroeconomic forecasting, particularly on sequential prediction methods with applications to financial stability. As a senior civil servant at the French National Institute of Statistics and Economic Studies (<a href="https://www.insee.fr/fr/accueil">INSEE</a>), I currently work in the National Accounts Department as a research methodologist. My work covers a range of topics, including the measurement of public service output in volume terms, profit shifting, and crypto-asset statistics. In my previous experiences, I also developed a strong interest in quantitative sociology.</p>

      <div class="profile-info">
        <a href="files/jeremy_fouliard_cv.pdf" target="_blank">Curriculum Vitae</a> &nbsp;·&nbsp;
        <a href="mailto:jeremy.fouliard@insee.fr">jeremy.fouliard@insee.fr</a> &nbsp;·&nbsp;
        <a href="mailto:jeremy.fouliard@psemail.eu">jeremy.fouliard@psemail.eu</a> &nbsp;·&nbsp;
        <a href="https://github.com/JedgeEcon" target="_blank"><i class="fa-brands fa-github"></i> GitHub</a>
      </div>
    </div>
  </div>

  <!-- ===== Working Papers ===== -->
  <h2 class="section-title">Working Papers</h2>
  <div class="sub-publications">
    <a href="files/queenpaper.pdf">
      <strong>Answering the Queen: Machine Learning and Financial Crises</strong>
    </a>
    <span class="coauthor"> — with Michael Howell (CbC), Hélène Rey (LBS), and Vania Stavrakeva (LBS)</span>  
    <br>
    <small style="font-family:'Outfit',sans-serif;font-size:0.78em;color:#888;letter-spacing:0.02em;">
      Coverage: <a href="https://www.nber.org/papers/w28302">NBER</a> · <a href="https://cepr.org/publications/dp15618">CEPR</a> · <a href="https://www.bis.org/publ/work926.pdf">BIS</a>
    </small>

    <details><summary>Abstract</summary>
      <p>
        Financial crises cause economic, social and political havoc. Macroprudential policies are gaining traction but are still severely under-researched compared to monetary and fiscal policy. We use the general framework of sequential predictions, also called online machine learning, to forecast crises out-of-sample. Our methodology is based on model aggregation and is "meta-statistical", since we can incorporate any predictive model of crises in our analysis and test its ability to add information, without making any assumption on the data generating process. We predict systemic financial crises twelve quarters ahead out-of-sample with high signal-to-noise ratio. Our approach guarantees that picking certain time dependent sets of weights will be asymptotically similar for out-of-sample forecasts to the best ex post combination of models; it also guarantees that we outperform any individual forecasting model asymptotically. We analyse which models provide the most information for our predictions at each point in time and for each country, allowing us to gain some insights into economic mechanisms underlying the building of risk in economies.
      </p>
    </details>
  </div>

  <!-- ===== Other Publications (Sociology) ===== -->
  <h2 class="section-title">Other Publications — Sociology</h2>
  <ul class="sub-publications">

    <li class="publication">
      <a href="files/exclusion.pdf">
        <strong>L'exclusion sociale est-elle réductible à la situation d'assistance ?</strong>
      </a>
      <span class="coauthor"> — with Éléonore Richard (DREES)</span>

      <details>
        <summary>Abstract</summary>
        <p>
          This article aims to quantify the relative significance of various determinants of the feeling of exclusion identified in the literature. Drawing on data from the 2018 "Statistics on Resources and Living Conditions" survey conducted by INSEE, it demonstrates that social assistance has no additional or intensifying effect on feelings of exclusion once controlling for factors such as labor market detachment, country of birth, material poverty, and geographical isolation.
        </p>
      </details>
    </li>

    <li class="publication">
      <a href="https://librairie.studyrama.com/produit/4681/9782749552255/l-exclusion-sociale"><strong>L'exclusion sociale. Reconstruire les communs</strong></a>
      <span class="coauthor">, 2022, Bréal.</span>

      <details>
        <summary>Abstract</summary>
        <p>
          Anti-racist movements, feminist movements, or the Yellow Vests movement: contemporary political struggles express the widespread feeling of social exclusion. This book seeks to redefine and account for the emergence of social exclusion, laying the first foundations for a political renewal against nationalist and neoliberal projects.
        </p>
      </details>
    </li>

    <li class="publication">
      <a href="https://librairie.studyrama.com/produit/4005/9782749553573/l-exclusion-sociale"><strong>L'exclusion sociale</strong></a>
      <span class="coauthor">, 2017, Bréal.</span>

      <details>
        <summary>Abstract</summary>
        <p>
          The notion of social exclusion now occupies a fundamental place worldwide, as both a focus of public policies and activist struggles. Drawing on Castel, Simmel, and Paugam, as well as fields ranging from the microeconomics of discrimination to the history of exclusion practices, this book examines the concept while serving as an introduction to the social sciences.
        </p>
      </details>
    </li>

  </ul>
</div>

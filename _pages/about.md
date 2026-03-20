---
permalink: /
title: ""
---
<style>
/* ===== Body & global styles ===== */
html, body {
  font-family: "Times New Roman", Times, serif;
  height: 100%;
  margin: 0;
  padding: 0;
}

#main {
    width: 100% !important;
    max-width: 100% !important;
    margin-top: 2em;
    animation: intro 0.3s both;
    animation-delay: 0.35s;
    padding-left: 0;
}

.main{
  width: 100%;
}

.article, .page {
  width: 100% !important;
  padding: 0 !important;
}

.a {
  color: #0a58ca;
  text-decoration: none;
  transition: 0.2s ease;
}

.a:hover {
  text-decoration: underline;
}

/* ===== Sticky header ===== */
.header-name {
  width: 100vw;
  left: 0;
  border-bottom: 1px solid rgba(0, 0, 0, 0.10);
}

.header-inner {
  display: flex;
  justify-content: flex-start;
  padding: 0.8em 1.5em;
  align-items: center;
  max-width: 1100px;
  margin: 0 auto;
}

.header-name h1 {
  font-size: 1em;
  font-weight: 400;
  margin: 0;
}

.header-github-desktop {
  position: absolute;       /* reste visible en scroll dans le conteneur */
  top: 10px;              /* décalage depuis le haut du conteneur image */
  left: -150px;             /* décalage depuis le côté gauche de l'image */
  z-index: 10;            /* pour qu'il soit au-dessus de l'image */
  display: flex;
  align-items: center;
  gap: 0.5em;
  background: rgba(255,255,255,0.8); /* optionnel, lisibilité sur l'image */
  padding: 0.2em 0.4em;
  border-radius: 6px;
  font-size: 1em;
  text-decoration: none;
}

.header-github-mobile {
  display: none;
}

.header-github i {
  font-size: 1.4em;
}

.header-github:hover {
  text-decoration: none; 
}

.fa-github {
  color: #000000;
  text-decoration: none;
}

/* ===== Main content ===== */
.main-content {
  margin: 0 auto;
  padding: 3em 2em;
  max-width: 1100px;
}

/* ===== Profile section ===== */
.profile-container {
  display: flex;
  flex-wrap: wrap;
  align-items: stretch; 
  margin-top: 2.5em;
  margin-bottom: 2.5em;
  gap: 3em;
}

.profile-picture {
  flex: 0 0 260px;
  display: flex;
  justify-content: center;
  position: relative;
}

.profile-picture img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 14px;
  box-shadow: 0 12px 35px rgba(0,0,0,0.12);
}

.profile-text {
  flex: 1;
  font-size: 1.05em;
  max-width: 700px;
}

.profile-info {
  margin-top: 1em;
  font-size: 0.9em;
  color: #555;
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 0.3em;
}

.profile-info a {
  color: #0366d6;
  text-decoration: none;
}

.profile-info a:hover {
  text-decoration: underline;
}

/* ===== Section titles ===== */
.h2.section-title {
  font-size: 1.5em;
  margin-top: 2.5em;
  margin-bottom: 0.8em;
  border-bottom: 2px solid #e6e6e6;
  padding-bottom: 0.35em;
}

.sub-publications {
  padding-left: 1.2em;
}

.publication a {
  font-weight: normal;
  text-decoration: underline;
}

.coauthor {
  font-weight: 400;
  color: #555;
  margin-left: 0.3em;
}

.main-content p {
  margin-bottom: 1em;
}

details summary {
  font-weight: 600;
  cursor: pointer;
  margin-top: 0.6em;
  margin-left: 1.5em;
}

details p {
  margin: 0.6em 0 1.2em 2em;
}

/* ===== Responsive ===== */
@media (max-width: 900px) {
  .profile-container {
    flex-direction: column;
    align-items: center;
  }

  .profile-text {
    text-align: center;
  }

  .profile-info {
    flex-direction: column;
    gap: 0.2em;
    text-align: center; 
  }

  .publication {
    margin-bottom: 20px;
  }

}

@media (max-width: 1330px) {
  .header-github-desktop {
    display: none;
  }

  /* Affiche le GitHub dans le header */
  .header-github-mobile {
    display: inline-flex;
    font-size: 1.2em;         /* plus gros sur mobile */
    margin-left: 0.5em;
    vertical-align: middle;
    text-decoration: none;
    background: rgba(255,255,255,0.8);
    padding: 0.3em 0.6em;     /* un peu plus grand */
    border-radius: 6px;
    color: #000000;           /* texte noir */
  }

  .header-github-mobile i {
    font-size: 1.6em;         /* icône un peu plus grande */
    color: #000000;           /* icône noire */
  }

  .header-inner {
    justify-content: space-around;
    position: relative;
  }
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
        <a class="header-github-desktop" href="https://github.com/JedgeEcon" target="_blank">
          <i class="fa-brands fa-github"></i> GitHub
        </a>
      <img src="images/jfouliard.jpeg" alt="Jeremy Fouliard">
    </div>

    <div class="profile-text">
      <p>Welcome ! I'm a High Civil Servant specialized in Economics and Statistics, a 
      <a href="https://www.insee.fr/fr/information/8599668">Engineer in Statistics, Economics and Data Science</a> 
      and a PhD student in Economics at the 
      <a href="https://www.parisschoolofeconomics.eu/en/persons/jeremy-fouliard/">Paris School of Economics</a>.</p>

      <p>My research focuses on macroeconomic forecasting, particularly on sequential prediction methods with applications to financial stability. As a senior civil servant at the French National Institute of Statistics and Economic Studies (<a href="https://www.insee.fr/fr/accueil">INSEE</a>), I currently work in the National Accounts Department as a research methodologist. My work covers a range of topics, including the measurement of public service output in volume terms, profit shifting, and crypto-asset statistics. In my previous experiences, I also developed a strong interest in quantitative sociology.</p>
    </div>
  </div>

  <div class="profile-info">
    <a href="files/jeremy_fouliard_cv.pdf" target="_blank">Curriculum Vitae</a> ·
    <a href="mailto:jeremy.fouliard@insee.fr">jeremy.fouliard@insee.fr</a> ·
    <a href="mailto:jeremy.fouliard@psemail.eu">jeremy.fouliard@psemail.eu</a>
  </div>

  <!-- ===== Working Papers ===== -->
<h2 class="section-title">Working Papers</h2>
  <div class="sub-publications">
    <a href="files/queenpaper.pdf">
      <strong>Answering the Queen: Machine Learning and Financial Crises</strong>
    </a>
    <span class="coauthor"> — with Michael Howell (CbC), Hélène Rey (LBS), and Vania Stavrakeva (LBS)</span>  
    <br>
    Coverage: <a href="https://www.nber.org/papers/w28302">NBER</a>, <a href="https://cepr.org/publications/dp15618">CEPR</a>, <a href="https://www.bis.org/publ/work926.pdf">BIS</a>

    <details><summary>Abstract</summary>
      <p>
        Financial crises cause economic, social and political havoc. Macroprudential policies are gaining traction but are still severely under-researched compared to monetary and fiscal policy. We use the general framework of sequential predictions, also called online machine learning, to forecast crises out-of-sample. Our methodology is based on model aggregation and is “meta-statistical”, since we can incorporate any predictive model of crises in our analysis and test its ability to add information, without making any assumption on the data generating process. We predict systemic financial crises twelve quarters ahead out-of-sample with high signal-to-noise ratio. Our approach guarantees that picking certain time dependent sets of weights will be asymptotically similar for out-of-sample forecasts to the best ex post combination of models; it also guarantees that we outperform any individual forecasting model asymptotically. We analyse which models provide the most information for our predictions at each point in time and for each country, allowing us to gain some insights into economic mechanisms underlying the building of risk in economies.
      </p>
    </details>
  </div>

  <!-- ===== Other Publications (Sociology) ===== -->
<h2 class="section-title">Other Publications (Sociology)</h2>
  <ul class="sub-publications">

    <li class="publication">
      <a href="files/exclusion.pdf">
        <strong>L’exclusion sociale est-elle réductible à la situation d’assistance ?</strong>
      </a>
      <span class="coauthor"> — with Éléonore Richard (DREES)</span>

      <details>
        <summary>Abstract</summary>
        <p>
          This article aims to quantify the relative significance of various determinants of the feeling of exclusion identified in the literature. Drawing on data from the 2018 “Statistics on Resources and Living Conditions” survey (“Statistiques sur les ressources et les conditions de vie” or “SRCV”) conducted by France’s National Institute of Statistics and Economic Studies (Insee), it demonstrates that social assistance, defined as households’ perception of social transfers, has no additional or intensifying effect on feelings of exclusion once controlling for factors such as labor market detachment, country of birth, material poverty, and geographical isolation. These findings contribute to the ongoing debate in the literature by refuting the hypothesis that feelings of exclusion are primarily attributable to the situation of being assisted, which binds individuals to society.
        </p>
      </details>
    </li>

    <li class="publication">
      <a href="https://librairie.studyrama.com/produit/4681/9782749552255/l-exclusion-sociale"><strong>L’exclusion sociale. Reconstruire les communs</strong></a>, 2022, Bréal.

      <details>
        <summary>Abstract</summary>
        <p>
          Anti-racist movements, feminist movements, or the Yellow Vests movement: contemporary political struggles express the widespread feeling of social exclusion — a sense of being deprived of access to the legitimate spheres of social life. If the feeling of social exclusion reflects a new way of framing the social question — that is, the question of social cohesion — the notion itself remains poorly defined, even though it has become an explicit objective of public policy. Faced with the nationalist and neoliberal projects that currently shape political horizons, this book seeks to redefine and account for the emergence of social exclusion. In doing so, it lays the first foundations for a political renewal.
        </p>
      </details>
    </li>

    <li class="publication">
      <a href="https://librairie.studyrama.com/produit/4005/9782749553573/l-exclusion-sociale"><strong>L’exclusion sociale</strong></a>, 2017, Bréal.

      <details>
        <summary>Abstract</summary>
        <p>
          The notion of social exclusion now occupies a fundamental place worldwide. It is both the focus of public policies and activist struggles, and has also become the subject of extensive academic research. Social exclusion is often seen as representative of the ills affecting our societies as a whole — from unemployment and precariousness to the sense of marginalization experienced by certain individuals. Yet the use of the concept and its definition remain extremely vague, raising doubts about its ability to make sense of the world we live in and, consequently, about the possibility of providing a social explanation for these phenomena. Drawing on the analyses of Castel, Simmel, and Paugam, as well as on fields as diverse as the microeconomics of discrimination and the history of exclusion practices, this book aims to examine the concept of social exclusion while also serving as an introduction to the social sciences, thanks to pedagogical boxed sections. This book is intended for students in the social sciences and economics.
        </p>
      </details>
    </li>

  </ul>
</div>
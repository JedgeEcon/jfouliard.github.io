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
      <p>Welcome !  I'm a High Civil Servant specialized in Economics and Statistics, a <a href="https://www.insee.fr/fr/information/8599668"> Engineer in Statistics, Economics and Data Science </a> and a PhD student in Economics at the <a href="https://www.parisschoolofeconomics.eu/en/persons/jeremy-fouliard/"> Paris School of Economics </a>.</p>
      <p>My research focuses on macroeconomic forecasting, particularly on sequential prediction methods with applications to financial stability. As a senior civil servant at the French National Institute of Statistics and Economic Studies (<a href="https://www.insee.fr/fr/accueil">INSEE</a>), I currently work in the National Accounts Department as a research methodologist. My work covers a range of topics, including the measurement of public service output in volume terms, profit shifting, and crypto-asset statistics. In my previous experiences, I also developed a strong interest in quantitative sociology.</p>

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
Coverage: <a href="https://www.nber.org/papers/w28302">NBER</a>, <a href="https://cepr.org/publications/dp15618">CEPR</a>, <a href="https://www.bis.org/publ/work926.pdf">BIS</a>, 

<details> <summary>Abstract</summary> <p> Financial crises cause economic, social and political havoc. Macroprudential policies are gaining traction but are still severely under-researched compared to monetary and fiscal policy. We use the general framework of sequential predictions, also called online machine learning, to forecast crises out-of-sample. Our methodology is based on model aggregation and is “meta-statistical”, since we can incorporate any predictive model of crises in our analysis and test its ability to add information, without making any assumption on the data generating process. We predict systemic financial crises twelve quarters ahead out-of-sample with high signal-to-noise ratio. Our approach guarantees that picking certain time dependent sets of weights will be asymptotically similar for out-of-sample forecasts to the best ex post combination of models; it also guarantees that we outperform any individual forecasting model asymptotically. We analyse which models provide the most information for our predictions at each point in time and for each country, allowing us to gain some insights into economic mechanisms underlying the building of risk in economies. </p> </details>

<a href="files/time.pdf"><strong>Is This Time Different? Financial Follies Across Centuries</strong></a>
with Hélène Rey (LBS) and Vania Stavrakeva (LBS). 
Talks : <a href="https://www.fmg.ac.uk/seminars time-different-financial-follies-across-centuries">FMG</a>, <a href="https://talks.ox.ac.uk/talks/id/857cb144-e2c2-4150-832a-4f8b201bb8d6">University of Oxford</a>, <a href="https://calendar.mit.edu/event/tba_7583">MIT</a>

<details> <summary>Abstract</summary> <p> Carmen Reinhart and Ken Rogoff have written that "no matter how different the latest financial frenzyor crisis always appears, there are usually remarkable similarities with past experience from other countries and from history". Can we really use the same models to predict the 20th century Great Depression and the 21st century Great Recession? We find that based exclusively on models estimated on the period 1874-1922, we can predict out-of-sample the 1929 Great Depression and all the 20th and 21st century systemic financial crises. </p> </details>

<strong>Predictable Returns</strong>

<details> <summary>Abstract</summary> <p> This paper proposes a market-based indicator of systemic risk in the euro area based on time-varying stock return predictability. Using a multi-task online learning framework and long historical stock market data, we study whether increases in predictability are systematically associated with the buildup of financial crises. </p> </details>

<strong>Volume Output Measurement for Public Education</strong>
with Mats Le Floch (INSEE) and Pauline Mendras (INSEE)
Coverage: <a href="https://journees-methodologie-statistique.insee.net/wp-content/uploads/2025/S09_3_RESUME_FOULIARD_LEFLOCH_JMS2025.pdf">JMS</a>

<details> <summary>Abstract</summary> <p> Measuring the volume of public services output is a fundamental challenge for national accounts, due to the absence of market prices. In France, the volume of nonmarket education is measured using an output approach based on student enrollment. This study compares alternative volume measurements, and examines different quality adjustments to effectively capture other features of the service provided. It introduces a theoretical framework that incorporates quality adjustments into output volume measures based on the contribution of quality to human capital, drawing on estimates consistent with the existing literature. Between 2013 and 2022, the class-size adjustment raises annual growth slightly (+0.016 percentage point on average, peaking at +0.037 point in 2020), while the adjustment based on PISA scores lowers it (-0.012 point on average, -0.021 point in 2022). Adjusting for the share of novice teachers has a negligible effect (below 0.01 point). Overall, quality adjustments have a minor effect on the estimated volume of education output, reflecting the low sensitivity of future earnings to the quality indicator considered. We also test a stratification of the education service adapted to pupils with disabilities, which increases cumulative volume growth by about one percentage point over 2006–2023, due to their rising enrollment in regular classes in France. </p> </details>

  <!-- Other Publications (Sociology) -->
  <h2 class="section-title">Other Publications (Sociology)</h2>

<a href="files/exclusion.pdf"><strong>L’exclusion sociale est-elle réductible à la situation d’assistance ?</strong></a>
with Éléonore Richard (DREES)

<details> <summary>Abstract</summary> <p> This article aims to quantify the relative significance of various determinants of the feeling of exclusion identified in the literature. Drawing on data from the 2018 “Statistics on Resources and Living Conditions” survey (“Statistiques sur les ressources et les conditions de vie” or “SRCV”) conducted by France’s National Institute of Statistics and Economic Studies (Insee), it demonstrates that social assistance, defined as households’ perception of social transfers, has no additional or intensifying effect on feelings of exclusion once controlling for factors such as labor market detachment, country of birth, material poverty, and geographical isolation. These findings contribute to the ongoing debate in the literature by refuting the hypothesis that feelings of exclusion are primarily attributable to the situation of being assisted, which binds individuals to society. </p> </details> 
</div>

<a href="https://librairie.studyrama.com/produit/4681/9782749552255/l-exclusion-sociale)"><strong>L’exclusion sociale. Reconstruire les communs </strong>, 2022, Bréal.</a>


<details> <summary>Abstract</summary> <p> Anti-racist movements, feminist movements, or the Yellow Vests movement: contemporary political struggles express the widespread feeling of social exclusion — a sense of being deprived of access to the legitimate spheres of social life.
If the feeling of social exclusion reflects a new way of framing the social question — that is, the question of social cohesion — the notion itself remains poorly defined, even though it has become an explicit objective of public policy. Faced with the nationalist and neoliberal projects that currently shape political horizons, this book seeks to redefine and account for the emergence of social exclusion. In doing so, it lays the first foundations for a political renewal. </p> </details> 
</div>


<a href="https://librairie.studyrama.com/produit/4005/9782749553573/l-exclusion-sociale"><strong>L’exclusion sociale </strong>, 2017, Bréal.</a>


<details> <summary>Abstract</summary> <p> The notion of social exclusion now occupies a fundamental place worldwide. It is both the focus of public policies and activist struggles, and has also become the subject of extensive academic research. Social exclusion is often seen as representative of the ills affecting our societies as a whole — from unemployment and precariousness to the sense of marginalization experienced by certain individuals. Yet the use of the concept and its definition remain extremely vague, raising doubts about its ability to make sense of the world we live in and, consequently, about the possibility of providing a social explanation for these phenomena. Drawing on the analyses of Castel, Simmel, and Paugam, as well as on fields as diverse as the microeconomics of discrimination and the history of exclusion practices, this book aims to examine the concept of social exclusion while also serving as an introduction to the social sciences, thanks to pedagogical boxed sections.This book is intended for students in the social sciences and economics. </p> </details> 
</div>
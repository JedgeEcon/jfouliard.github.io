---
permalink: /
title: ""
---
<style>
@import url('https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;1,400&family=Outfit:wght@300;400;500&display=swap');

/* ===== Force beige background everywhere ===== */
html, body,
#main, #page, .page, .page__content,
.page__inner-wrap, .initial-content,
.layout--single, div[id="main"],
.page__content, article.page,
div.page__inner-wrap, div.page__content {
  background: #fafaf8 !important;
  background-color: #fafaf8 !important;
}

/* Kill the white box Academic Pages adds */
.page__content {
  padding: 0 !important;
  border: none !important;
  box-shadow: none !important;
}

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
  font-weight: 600;
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
  align-items: center;
  gap: 3.5em;
  margin-bottom: 3em;
}

.profile-picture {
  flex: 0 0 280px;
  margin-left: -6em;
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
  margin-right: -4em;
  text-align: justify;
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
    width: 200px;
    margin-left: 0;
    margin: 0 auto;
  }

  .profile-text {
    text-align: left;
    margin-right: 0;
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
      <img src="images/jfouliard.jpeg" alt="Jérémy Fouliard">
    </div>

    <div class="profile-text">
      <p>Welcome! I am a PhD candidate in Economics at the
      <a href="https://www.parisschoolofeconomics.eu/en/persons/jeremy-fouliard/">Paris School of Economics</a>,
      advised by Pierre-Cyrille Hautcoeur and Eric Monnet, and a senior French civil servant, member of the State corps of
      <a href="https://www.insee.fr/fr/information/8599668"><em>Ingénieurs de la statistique, de l'économie et de la donnée</em></a>.</p>

      <p>My research is in macroeconomic and financial forecasting and in economic measurement. Both ask what the data available today can reliably tell us about an economy that we observe imperfectly and with delay. I currently work as a research methodologist in the National Accounts Department of the French National Institute of Statistics and Economic Studies (<a href="https://www.insee.fr/fr/accueil">INSEE</a>), on the measurement of public sector output, profit shifting by multinational firms and crypto-assets. Before my PhD, I worked at London Business School on Hélène Rey's ERC project and at the Bank for International Settlements.</p>

      <div class="profile-info">
        <a href="files/jeremy_fouliard_cv.pdf" target="_blank">Curriculum Vitae</a> &nbsp;·&nbsp;
        <a href="mailto:jeremy.fouliard@psemail.eu">jeremy.fouliard@psemail.eu</a> &nbsp;·&nbsp;
        <a href="mailto:jeremy.fouliard@insee.fr">jeremy.fouliard@insee.fr</a> &nbsp;·&nbsp;
        <a href="https://github.com/JedgeEcon" target="_blank"><i class="fa-brands fa-github"></i> GitHub</a>
      </div>
    </div>
  </div>

  <!-- ===== Job Market Paper ===== -->
  <h2 class="section-title">Job Market Paper</h2>
  <ul class="sub-publications">

    <li class="publication">
      <!-- Upload the PDF to files/ and keep this name, or change the link -->
      <a href="files/fouliard_jmp.pdf">
        <strong>Slow to Catch Up: Return Predictability on the Paris Bourse, 1845–2025</strong>
      </a><br>
      <details open><summary>Abstract</summary>
        <p>
          Whether stock returns can be predicted has fascinated academics, practitioners and policymakers for more than a century. I revisit this old question with a new security-level dataset of stock returns on the Paris Bourse. To answer it, I adopt the framework of sequential prediction, in which forecasts combine models as they become available through Bernstein Online Aggregation, an aggregation rule with a bounded regret that assumes nothing about the return-generating process. The results depend on the level of prediction. The market index is barely predictable: macro-financial predictors explain 0.5% of its half-monthly variance, mostly in crises, and the larger predictability of lagged index returns is a stale-price artefact. Individual stocks are more predictable, by about 0.6%, mostly because they react to market-wide news with a delay that is strongest in small stocks, not explained by stale prices, and unchanged over 155 years. Momentum earns 7% a year net of costs in almost every decade since 1900, while the historical volatility and beta premia vanish after 1977. Markets became better at pricing risk, but not faster at absorbing information.
        </p>
      </details>
    </li>

  </ul>

  <!-- ===== Working Papers ===== -->
  <h2 class="section-title">Working Papers</h2>
  <ul class="sub-publications">

    <li class="publication">
      <a href="files/QUEEN.pdf">
        <strong>Answering the Queen: Machine Learning and Financial Crises</strong>
      </a>
      <span class="coauthor"> — with Michael Howell (CrossBorder Capital), Hélène Rey (BIS) and Vania Stavrakeva (LBS)</span><br>
      <small style="font-family:'Outfit',sans-serif;font-size:0.78em;color:#888;letter-spacing:0.02em;">
        New version, 2026
      </small><br>
      <small style="font-family:'Outfit',sans-serif;font-size:0.78em;color:#888;letter-spacing:0.02em;">
        Earlier versions: <a href="https://www.nber.org/papers/w28302">NBER WP 28302</a> · <a href="https://cepr.org/publications/dp15618">CEPR</a> · <a href="https://www.bis.org/publ/work926.pdf">BIS</a>
      </small>
      <details><summary>Abstract</summary>
        <p>
          Financial crises cause economic, social and political havoc. Macroprudential policies are gaining traction but are still severely under-researched compared to monetary and fiscal policy. This paper designs an aggregation procedure for probabilistic forecasts that issues a warning up to twelve quarters before a financial crisis, identifies in real time which channel of vulnerability drives the warning, and comes with a formal performance guarantee of the type established in the online learning literature. Applied in real time to France, Germany, Sweden and the United Kingdom from 2001 to 2025, with models estimated on the crises of the early 1990s only, the procedure raises an alarm before each of the four crises of 2007–2008, with leads of one to five years, and separates pre-crisis from calm quarters with an out-of-sample AUROC between 0.83 and 0.96.
        </p>
      </details>
    </li>

    <li class="publication">
      <a href="files/volume_fouliard.pdf">
        <strong>Volume Output Measurement of Public Services: The Case of Education</strong>
      </a>
      <span class="coauthor"> — with M. Le Floch (INSEE) and P. Mendras (INSEE)</span><br>
      <small style="font-family:'Outfit',sans-serif;font-size:0.78em;color:#888;letter-spacing:0.02em;">
        Revise and resubmit, <em>Review of Income and Wealth</em>
      </small><br>
      <small style="font-family:'Outfit',sans-serif;font-size:0.78em;color:#888;letter-spacing:0.02em;">
        Coverage: <a href="https://journees-methodologie-statistique.insee.net/wp-content/uploads/2025/S09_3_PRES_fouliard_JMS2025.pdf">JMS</a> · <a href="https://unece.org/statistics/documents/2026/04/working-documents/volume-measures-non-market-education-output-france-0">UNECE</a>
      </small>
      <details><summary>Abstract</summary>
        <p>
          Measuring the volume of public services output is a fundamental challenge for national accounts, due to the absence of market prices. In France, the volume of non-market education is measured using an output approach based on student enrollment. As this indicator mainly reflects demographic trends, the recent decline in the number of students mechanically reduces the estimated volume of education, even if quality teaching could have improved, for example through smaller class sizes. This study compares alternative volume measurements, and examines different quality adjustments to capture other features of the service provided. It introduces a theoretical framework that incorporates quality adjustments into output volume measures based on the contribution of quality to human capital, drawing on estimates consistent with the existing literature. Between 2013 and 2022, the adjustment based on PISA scores lowers annual growth rates (−0.056 percentage points on average) while the class-size adjustment slightly raises annual growth (+0.015 percentage points on average). Overall, quality adjustments have a modest effect on the estimated volume of education output, but moderate effects could accumulate over time and result in visible change in trend.
        </p>
      </details>
    </li>

    <li class="publication">
      <span style="font-style:italic;font-weight:500;">Quality-Adjusted Output and Productivity of the Non-Market Health Sector in France</span><br>
      <small style="font-family:'Outfit',sans-serif;font-size:0.78em;color:#888;letter-spacing:0.02em;">
        Draft coming soon · Presented at the OECD Working Party on National Accounts, 2026
      </small>
      <details><summary>Abstract</summary>
        <p>
          Despite an extensive literature on health care productivity, measuring quality-adjusted output in non-market settings remains an open challenge. This paper derives a welfare-based, quality-adjusted output index from a social planner's cost-minimisation problem, and identifies the distinct sources of productivity growth. Quality adjustment rests on a disease-based output specification in which each treatment contributes to aggregate health through two channels: a survival component, measured by severity-adjusted mortality rates, and a health-related quality-of-life component, measured by QALY gains per episode. Rather than importing QALY values from external tariffs, we estimate them directly from individual-level administrative data from the French Système National des Données de Santé (SNDS), which covers virtually the entire French population over 2012–2022. This exhaustive coverage enables a counterfactual analysis that isolates hospital-produced health gains from secular trends in population health. The framework is directly portable to any health system with diagnosis-related group tariffs and linked administrative records.
        </p>
      </details>
    </li>

    <li class="publication">
      <span style="font-style:italic;font-weight:500;">Profit Shifting and the Measurement of Value Added: Evidence from a Distribution of French National Accounts by Type of Firm</span>
      <span class="coauthor"> — with U. Di Nallo (INSEE)</span><br>
      <small style="font-family:'Outfit',sans-serif;font-size:0.78em;color:#888;letter-spacing:0.02em;">
        Draft coming soon · Presented at the INSEE National Accounts Seminar and the OECD EG-MG Conference, 2026
      </small>
      <details><summary>Abstract</summary>
        <p>
          National accounts record value added in the economy where the producing unit is resident, but multinational groups can separate the location of their profits from the location of their production. We develop a method that distributes the production account across any partition of firms, following each legal unit from its tax return to published value added, and apply it to the breakdown recommended by the 2025 SNA: foreign-controlled corporations, domestic multinational groups and other domestic corporations. Combining country-by-country reports with tax returns for 2019–2023, we estimate profit shifting at the group level and pass this estimate through the compilation of French national accounts, to assess whether a correction for profit shifting can be produced within official statistics.
        </p>
      </details>
    </li>

    <li class="publication">
      <a href="files/thistimeisdifferent.pdf">
        <strong>Is This Time Different? Financial Follies across Centuries</strong>
      </a>
      <span class="coauthor"> — with Hélène Rey (BIS) and Vania Stavrakeva (LBS)</span><br>
      <details><summary>Abstract</summary>
        <p>
          Carmen Reinhart and Ken Rogoff write that "no matter how different the latest financial frenzy or crisis always appears, there are usually remarkable similarities with past experience from other countries and from history". Can we really use the same models to predict the 20th century Great Depression and the 21st century Great Recession? We find that we can predict out-of-sample the 1929 Great Depression and all the 20th and 21st century systemic financial crises in a panel of countries. We also generally do not over-predict crises during the Bretton Woods period.
        </p>
      </details>
    </li>

  </ul>

  <!-- ===== Work in Progress ===== -->
  <h2 class="section-title">Work in Progress</h2>
  <ul class="sub-publications">

    <li class="publication">
      <span style="font-style:italic;font-weight:500;">AI and the Transatlantic Productivity Gap: Who Captures the Gains from US Innovation?</span><br>
      <small style="font-family:'Outfit',sans-serif;font-size:0.78em;color:#888;letter-spacing:0.02em;">
        Draft coming soon
      </small>
      <details><summary>Abstract</summary>
        <p>
          Frontier AI is produced mainly in the United States and China, while Europe, which produces little of it, will be a large user. Focusing on the transatlantic link, I study what this asymmetry implies for the productivity gap between Europe and the United States. I build a two-country model in the spirit of Baqaee and Farhi, in which production is a network of an AI sector, AI-using traded sectors and a sheltered sector, calibrated on international input-output tables. Innovation is concentrated in the United States and financed by the rents of AI producers, European adoption is endogenous and disciplined by occupational exposure to AI, compute is an accumulated capital stock, and the exchange rate is determined in equilibrium. The model separates the productivity gains that Europe obtains from AI from the value added it captures, the difference being the rent paid to US producers and the change in the terms of trade. It also shows how hedonic deflation and the capitalisation of AI spending shape measured European productivity, and when the constant-price and current-PPP readings of the transatlantic gap can each be right.
        </p>
      </details>
    </li>

  </ul>

  <!-- ===== Teaching ===== -->
  <h2 class="section-title">Teaching</h2>
  <ul class="sub-publications">
    <li class="publication" style="margin-bottom:0.6em;"><strong>Programming for Economists</strong> <span class="coauthor">— Paris School of Economics, graduate course (Python, Git workflows), 2027</span></li>
    <li class="publication" style="margin-bottom:0.6em;"><strong>Economic Measurement</strong> <span class="coauthor">— Sciences Po, graduate course, co-taught with E. Richard (DREES), 2027</span></li>
    <li class="publication" style="margin-bottom:0.6em;"><strong>Teaching Assistant, Microeconomics and Statistics</strong> <span class="coauthor">— Sciences Po, second-year undergraduate students, 2022–2024</span></li>
  </ul>

  <!-- ===== References ===== -->
  <h2 class="section-title">References</h2>
  <ul class="sub-publications">
    <li class="publication" style="margin-bottom:0.6em;"><strong>Hélène Rey</strong> <span class="coauthor">— Economic Adviser and Head of the Monetary and Economic Department, Bank for International Settlements</span></li>
    <li class="publication" style="margin-bottom:0.6em;"><strong>Eric Monnet</strong> <span class="coauthor">— Professor of Economics, Paris School of Economics</span></li>
    <li class="publication" style="margin-bottom:0.6em;"><strong>Pierre-Cyrille Hautcoeur</strong> <span class="coauthor">— Professor of Economics, Paris School of Economics</span></li>
    <li class="publication" style="margin-bottom:0.6em;"><strong>Sébastien Roux</strong> <span class="coauthor">— Programme Director, Augmented National Accounts, INSEE</span></li>
  </ul>

</div>
---
layout: default
title: "About Yogi & Linga"
permalink: /about/
description: "Yogi & Linga is an independent sexual wellness publication staffed by writers, researchers, and testers who believe honest product review and evidence-based information can coexist in the same place."
---

<style>
.about-hero {
  max-width: 860px;
  margin: 0 auto;
  padding: 5rem 2rem 3rem;
  text-align: center;
}
.about-eyebrow {
  font-size: 0.62rem;
  letter-spacing: 0.3em;
  text-transform: uppercase;
  color: var(--rose-gold);
  margin-bottom: 1.5rem;
}
.about-headline {
  font-family: var(--font-serif);
  font-size: clamp(2.2rem, 4vw, 3.5rem);
  font-weight: 300;
  line-height: 1.1;
  color: var(--cream);
  margin-bottom: 1.75rem;
}
.about-headline em { font-style: italic; color: var(--rose-gold-bright); }
.about-lead {
  font-size: 1.05rem;
  line-height: 1.9;
  color: var(--cream-dim);
  max-width: 620px;
  margin: 0 auto;
}
.about-divider {
  width: 60px;
  height: 0.5px;
  background: linear-gradient(90deg, transparent, var(--rose-gold), transparent);
  margin: 3.5rem auto;
}
.about-body {
  max-width: 720px;
  margin: 0 auto;
  padding: 0 2rem 3rem;
  font-size: 1rem;
  line-height: 1.9;
  color: var(--cream-dim);
}
.about-body h2 {
  font-family: var(--font-serif);
  font-size: 2rem;
  font-weight: 300;
  font-style: italic;
  color: var(--cream);
  margin: 3rem 0 1.25rem;
}
.about-body p { margin-bottom: 1.5rem; }
.about-body strong { color: var(--cream); font-weight: 400; }

/* Score criteria table */
.score-table {
  width: 100%;
  border-collapse: collapse;
  margin: 1.5rem 0 2rem;
  font-size: 0.88rem;
}
.score-table th {
  text-align: left;
  font-size: 0.62rem;
  letter-spacing: 0.18em;
  text-transform: uppercase;
  color: var(--rose-gold);
  padding: 0.5rem 1rem 0.5rem 0;
  border-bottom: 0.5px solid rgba(201,149,108,0.25);
  font-weight: 400;
}
.score-table td {
  padding: 0.75rem 1rem 0.75rem 0;
  vertical-align: top;
  border-bottom: 0.5px solid rgba(255,255,255,0.05);
  color: var(--cream-dim);
  line-height: 1.6;
}
.score-table td:first-child { color: var(--cream); font-weight: 400; white-space: nowrap; }

.team-section {
  max-width: 1000px;
  margin: 0 auto;
  padding: 3rem 2rem 5rem;
}
.team-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5rem;
  margin-top: 2.5rem;
}
.team-card {
  background: rgba(255,255,255,0.025);
  border: 0.5px solid var(--border);
  padding: 2rem 1.75rem;
}
.team-avatar {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  background: radial-gradient(circle at 40% 40%, var(--wine-light), var(--wine-deep));
  border: 0.5px solid rgba(201,149,108,0.2);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 1.25rem;
  font-family: var(--font-serif);
  font-size: 1.5rem;
  font-style: italic;
  color: var(--rose-gold);
  opacity: 0.7;
}
.team-name {
  font-family: var(--font-serif);
  font-size: 1.25rem;
  font-weight: 300;
  color: var(--cream);
  margin-bottom: 0.25rem;
}
.team-role {
  font-size: 0.62rem;
  letter-spacing: 0.22em;
  text-transform: uppercase;
  color: var(--rose-gold);
  opacity: 0.75;
  margin-bottom: 1rem;
}
.team-bio { font-size: 0.82rem; line-height: 1.75; color: var(--cream-dim); }

.values-section {
  border-top: 0.5px solid var(--border);
  border-bottom: 0.5px solid var(--border);
  background: rgba(255,255,255,0.012);
}
.values-inner {
  max-width: 1000px;
  margin: 0 auto;
  padding: 4rem 2rem;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2.5rem;
}
.value-item {}
.value-num {
  font-family: var(--font-serif);
  font-size: 2.5rem;
  font-weight: 300;
  color: var(--rose-gold);
  opacity: 0.3;
  line-height: 1;
  margin-bottom: 0.75rem;
}
.value-title {
  font-size: 0.68rem;
  letter-spacing: 0.22em;
  text-transform: uppercase;
  color: var(--cream);
  margin-bottom: 0.75rem;
}
.value-text { font-size: 0.82rem; line-height: 1.8; color: var(--cream-dim); }

.press-bar {
  max-width: 720px;
  margin: 0 auto;
  padding: 2.5rem 2rem;
  text-align: center;
  border-top: 0.5px solid var(--border);
}
.press-label {
  font-size: 0.58rem;
  letter-spacing: 0.3em;
  text-transform: uppercase;
  color: var(--cream-dim);
  opacity: 0.5;
  margin-bottom: 1.5rem;
}
.press-items {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem 2.5rem;
  justify-content: center;
  align-items: center;
}
.press-item {
  font-family: var(--font-serif);
  font-size: 1rem;
  font-style: italic;
  color: var(--cream-dim);
  opacity: 0.35;
  letter-spacing: 0.04em;
}

@media (max-width: 768px) {
  .team-grid { grid-template-columns: 1fr; }
  .values-inner { grid-template-columns: 1fr; }
}
</style>

<div class="about-hero">
  <p class="about-eyebrow">Who We Are</p>
  <h1 class="about-headline">
    Sexual wellness deserves<br>
    the same rigor as any<br>
    other <em>health category.</em>
  </h1>
  <p class="about-lead">
    Yogi & Linga is an independent publication covering sexual wellness products, evidence-based research, and the intersection of pleasure and health. We test products, read studies, and write about both with the same care we'd apply to any serious health topic.
  </p>
</div>

<div class="about-divider"></div>

<div class="about-body">
  <h2>Why this publication exists</h2>
  <p>
    Sexual wellness content has a credibility problem. The category is dominated by content that is either breathlessly promotional — every product is "life-changing" — or so hedged and clinical that it fails the people it's meant to help.
  </p>
  <p>
    We started Yogi & Linga because we believed there was space for a third approach: honest, cited, and genuinely useful. The kind of publication that will tell you when a $200 toy isn't meaningfully better than a $40 one, and will explain <em>why</em> with reference to how the motors actually work.
  </p>
  <p>
    We cover sexual wellness the same way a good health publication covers nutrition or exercise — with skepticism toward marketing claims, respect for peer-reviewed research, and a commitment to helping readers make genuinely informed decisions.
  </p>

  <h2>How we test</h2>
  <p>
    Every product we review is either purchased independently with our own funds or received as a press sample with <strong>no editorial conditions attached</strong>. We never accept payment for reviews, positive ratings, or sponsored placement within editorial content.
  </p>
  <p>
    We test products over a minimum of three weeks before publishing a review. For products with app connectivity, we evaluate the app across multiple devices and software versions. For material safety claims — particularly "body-safe silicone" or "phthalate-free" — we request third-party documentation from manufacturers and note when it cannot be provided.
  </p>

  <h2>Our scoring system</h2>
  <p>
    Each review is scored on a 10-point scale, reflecting a weighted average of the following criteria:
  </p>

  <table class="score-table">
    <thead>
      <tr>
        <th>Criterion</th>
        <th>Weight</th>
        <th>What We Evaluate</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Motor / stimulation quality</td>
        <td>30%</td>
        <td>Power, pattern variety, ramp-up speed, consistency across settings</td>
      </tr>
      <tr>
        <td>Material safety</td>
        <td>20%</td>
        <td>Body-safe certification, silicone quality, absence of phthalates or porous materials</td>
      </tr>
      <tr>
        <td>Build quality & design</td>
        <td>15%</td>
        <td>Seam quality, button feel, ergonomics, water resistance claims vs. real-world performance</td>
      </tr>
      <tr>
        <td>App & connectivity</td>
        <td>15%</td>
        <td>App stability, Bluetooth reliability, feature depth (for app-enabled products only)</td>
      </tr>
      <tr>
        <td>Battery & noise</td>
        <td>10%</td>
        <td>Runtime at max power, recharge time, noise level in real conditions</td>
      </tr>
      <tr>
        <td>Value for money</td>
        <td>10%</td>
        <td>Performance relative to price; comparison to competitors at the same price point</td>
      </tr>
    </tbody>
  </table>

  <p>
    Scores reflect our team's collective assessment across multiple testers where possible. We note clearly when anatomy or personal preference meaningfully affects a rating.
  </p>

  <h2>On affiliate relationships</h2>
  <p>
    We participate in affiliate programs for the brands we review. This means we may earn a commission when you purchase through a link on our site, at no additional cost to you. Our <a href="/affiliate-disclosure/" style="color: var(--rose-gold);">full affiliate disclosure</a> lists every program we participate in.
  </p>
  <p>
    Affiliate relationships do not affect scores or recommendations. We have published negative-to-neutral reviews of products from brands in our affiliate network, and will continue to do so. We believe our credibility with readers is worth more than any individual commission.
  </p>

  <h2>On the topic itself</h2>
  <p>
    Sexual wellness is a legitimate health category. Research consistently links sexual health — including solo practice — to measurable outcomes in sleep quality, stress regulation, and emotional wellbeing. We treat it as such.
  </p>
  <p>
    We also recognize that this topic remains stigmatized in ways that make honest information harder to find. We're trying to contribute to changing that, one well-sourced article at a time.
  </p>
</div>

<section class="team-section">
  <div style="text-align: center; margin-bottom: 1rem;">
    <p style="font-size: 0.62rem; letter-spacing: 0.3em; text-transform: uppercase; color: var(--rose-gold);">The Team</p>
    <h2 style="font-family: var(--font-serif); font-size: 2.2rem; font-weight: 300; font-style: italic; color: var(--cream); margin-top: 0.75rem;">The people behind the reviews</h2>
  </div>

  <div class="team-grid">
    <div class="team-card">
      <div class="team-avatar">S</div>
      <p class="team-name">Sasha Mercer</p>
      <p class="team-role">Editor-in-Chief</p>
      <p class="team-bio">Sasha has spent eight years covering health and wellness for digital publications. She came to sexual wellness after noticing that product coverage in the category was almost universally uncritical. She holds a background in health journalism and brings the same skepticism to a vibrator review that she'd apply to a supplement claim. She oversees editorial standards, scoring methodology, and affiliate disclosure compliance.</p>
    </div>
    <div class="team-card">
      <div class="team-avatar">R</div>
      <p class="team-name">Rowan Ellis</p>
      <p class="team-role">Senior Reviewer</p>
      <p class="team-bio">Rowan tests the majority of products that pass through the Yogi & Linga lab. With a background in materials science, Rowan brings technical rigor to questions of body-safe certification, motor construction, and build quality that most consumer reviewers can't. They developed our material verification protocols and are responsible for ensuring all safety claims in reviews are documented and accurate.</p>
    </div>
    <div class="team-card">
      <div class="team-avatar">M</div>
      <p class="team-name">Maya Chen</p>
      <p class="team-role">Wellness Research Editor</p>
      <p class="team-bio">Maya covers the science side of the publication — the neuroscience, clinical research, and the studies that are well-conducted versus the ones that are noise. She has a graduate background in health psychology and a particular interest in the intersection of sexual health and mental wellbeing. She reviews all health claims in our articles for accuracy and ensures citations link to primary sources, not press releases.</p>
    </div>
  </div>
</section>

<section class="values-section">
  <div class="values-inner">
    <div class="value-item">
      <p class="value-num">01</p>
      <p class="value-title">Independence</p>
      <p class="value-text">We are independently owned and operated. No brand has editorial input on our coverage. Products we recommend are products we tested and liked — nothing more. Affiliate commissions support the publication but never influence scores.</p>
    </div>
    <div class="value-item">
      <p class="value-num">02</p>
      <p class="value-title">Honesty</p>
      <p class="value-text">We will tell you when something isn't worth the price, when a budget option outperforms a premium one, and when a category claim isn't backed by evidence. Our negative reviews stay published.</p>
    </div>
    <div class="value-item">
      <p class="value-num">03</p>
      <p class="value-title">Safety first</p>
      <p class="value-text">Body-safe materials are non-negotiable. We will never recommend a product made with phthalates, porous rubber, or materials that put users at risk — regardless of commission rate or brand relationship.</p>
    </div>
  </div>
</section>

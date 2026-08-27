---
layout: page
title: PRAMS
permalink: /prams/
description: Pain Recognition Automated Monitoring System — an NSF-funded project developing AI-driven neonatal pain detection using federated learning.
nav: true
nav_order: 4
---

<style>
.prams-banner { width: 100%; border-radius: 8px; margin-bottom: 1.5rem; aspect-ratio: 3/1; object-fit: cover; object-position: center center; }
.prams-hero { text-align: center; margin-bottom: 2rem; }
.prams-hero h2 { font-size: 1.05rem; font-style: italic; color: var(--global-theme-color); margin-top: 0.5rem; }
.prams-highlight { border-left: 4px solid var(--global-theme-color); padding: 1rem 1.25rem; margin: 1.5rem 0; background: rgba(0,100,177,0.04); font-style: italic; font-size: 1rem; line-height: 1.7; }
.prams-highlight footer { font-style: normal; font-size: 0.85rem; margin-top: 0.5rem; font-weight: 600; }
.prams-points { margin: 1.5rem 0; }
.prams-points li { margin-bottom: 0.5rem; line-height: 1.6; }
.prams-img { display: block; margin: 1.5rem auto; max-width: 700px; width: 100%; border-radius: 6px; }
.prams-obj { counter-reset: obj; margin: 2rem 0; }
.prams-obj-card { border: 1px solid var(--global-divider-color); border-radius: 8px; padding: 1.25rem 1.5rem; margin-bottom: 1rem; }
.prams-obj-card h3 { margin-top: 0; font-size: 1.1rem; }
.prams-obj-card h3::before { counter-increment: obj; content: "Objective " counter(obj) ": "; font-weight: 700; color: var(--global-theme-color); }
.prams-impact li { margin-bottom: 0.5rem; line-height: 1.6; }
.prams-team { margin: 2rem 0; }
.prams-team ul { list-style: none; padding: 0; }
.prams-team li { padding: 0.3rem 0; font-size: 0.9rem; line-height: 1.5; }
.prams-team li strong { font-weight: 700; }
.prams-funding { display: flex; align-items: center; gap: 1rem; flex-wrap: wrap; margin-top: 1rem; }
.prams-funding img { height: 60px; }
.prams-contact { border: 1px solid var(--global-divider-color); border-radius: 8px; padding: 1.25rem 1.5rem; margin: 2rem 0; }
.prams-contact h3 { margin-top: 0; }
</style>

<img src="/assets/img/prams/baby_cover.jpg" alt="Newborn baby in neonatal care" class="prams-banner">

<div class="prams-hero">
<h2>Pain is a global health problem affecting over 15 million hospitalized babies each year. We are using federated learning to develop the first nurse-supervised Pain Recognition AI Monitoring System grounded by biological evidence of pain.</h2>
</div>

---

## The Challenge

**Understanding the Unspoken: The Need for Better Pain Monitoring**

Inability to provide self-report makes babies vulnerable to under-recognition, under treatment, and even overtreatment of pain. The critical challenge is to continuously monitor hospitalized babies for acute pain, such as surgical pain, and to evaluate the need to treat, and the duration and effectiveness of pain treatments.

<ul class="prams-points">
<li>Early-life pain is associated with abnormal structural and functional brain development and results in adverse consequences, including cognitive impairments, altered emotional functioning, psychopathologies, and global pain sensitivity.</li>
<li>Current pain assessment tools are highly dependent on nurses' availability, expertise, and experiences. Nurses only agree to the presence of baby's pain 67–87% of the time.</li>
<li>Pain assessment practices are discontinuous, inconsistent, and not based on brain-based evidence of pain. Currently, there are no AI-powered continuous pain monitoring systems.</li>
</ul>

<img src="/assets/img/prams/challenge_slide.png" alt="Overview of neonatal pain assessment challenges" class="prams-img">

---

## The Vision

**A Nurse Call Button for Babies: The PRAMS Solution**

PRAMS is an AI-driven system designed to continuously recognize and assess pain using multimodal data. It aims to:

- Improve quality of care through real-time pain alerts.
- Enhance outcomes and care equity by ensuring all babies receive timely pain management.
- Support clinicians with data-driven decision tools that complement clinical judgment.

<blockquote class="prams-highlight">
<p>"We're creating a nurse call button for babies, ensuring their discomfort never goes unnoticed."</p>
</blockquote>

<img src="/assets/img/prams/nurse_call_button.png" alt="PRAMS nurse call button concept" class="prams-img">

---

## Research Objectives

<div class="prams-obj">

<div class="prams-obj-card">
<h3>Building a Heterogeneous Pain Assessment Database</h3>
<p>We are developing a multimodal, time-series database using facial action videos, physiological data, and clinical records from 200+ babies.</p>
<ul class="prams-points">
<li>Captures diversity in gender, race, prematurity, age, and medical conditions.</li>
<li>Identifies the best performing AI features for pain prediction.</li>
<li>Explores the relative importance of continuous physiological monitoring data as a potential predictor variable.</li>
</ul>
</div>

<div class="prams-obj-card">
<h3>Advancing Federated Learning</h3>
<p>We are testing a hybrid Federated Learning framework to simulate inter-institutional learning.</p>
<ul class="prams-points">
<li>Overcomes challenges of non-IID data distributions.</li>
<li>Protects patient privacy — no raw data or gradients leave local servers.</li>
<li>Enables scalable, secure model training across healthcare networks.</li>
</ul>
</div>

<div class="prams-obj-card">
<h3>Mathematical Validation</h3>
<p>Our novel hybrid FL algorithm is designed for both convex and non-convex optimization, ensuring strong convergence and reliability for real-world applications.</p>
</div>

</div>

---

## Technology & Innovation

**AI Meets Compassionate Care**

1. **Data Labeling & Validation** — A human-centered approach where nurses collaborate with AI tools to refine data accuracy and model performance.
2. **Model Experimentation** — Comparison of machine learning models to identify optimal predictors.
3. **Real-Time Monitoring** — Edge computing enables on-site video analysis and alerts when pain is detected, prompting immediate nurse intervention.

<img src="/assets/img/prams/technology_slide.png" alt="PRAMS technology pipeline and AI architecture" class="prams-img">

---

## Why PRAMS Matters

<ul class="prams-impact">
<li>Ensures continuous, unbiased pain recognition in infants unable to self-report.</li>
<li>Promotes care equity across populations by training on diverse datasets.</li>
<li>Supports clinicians with objective, data-backed insights.</li>
<li>Improves family confidence and satisfaction through visible, data-driven monitoring.</li>
<li>Aligns with the vision of AI ethics and privacy, using federated learning to protect patient data.</li>
</ul>

---

## Future Directions

Planned extensions include:

- Deployment in real NICU settings with real-time clinical decision support.
- Publication and open collaboration across institutions.
- Expand to monitor pain in other people who cannot provide self-report.

---

## Students

<div class="prams-team">
<ul>
<li><strong>James M. DeMasi, MSN, APRN, CPNP-AC/PC, AP-PMGT</strong> — Nursing PhD Student, UTA (Children's Health Dallas)</li>
<li><strong>Michelle Pearce, BA, MSN, RNC-NIC</strong> — Nursing PhD Student, UTA (Parkland Hospital)</li>
<li><strong>Pollieanna Sepulveda</strong> — PhD Student, Nursing</li>
<li><strong>Zheyan Zhang</strong> — Industrial Engineering PhD Student, Northwestern University</li>
</ul>
</div>

## Collaborators

<div class="prams-team">
<ul>
<li><strong>Dr. Diego Klabjan</strong> — Northwestern University, College of Engineering</li>
<li><strong>Dr. Susan Horner</strong> — Post-doctoral Researcher, Ann & Robert H. Lurie Children's Hospital of Chicago</li>
<li><strong>Ashley Song, BS</strong> — Clinical Research Coordinator, Ann & Robert H. Lurie Children's Hospital of Chicago</li>
<li><strong>KaviGlobal</strong> — Industry Partner</li>
</ul>
</div>

---

*Our mission is to merge compassionate care with cutting-edge technology to give every infant a voice.*

<div class="prams-funding">
<img src="/assets/img/prams/nsf_logo.png" alt="National Science Foundation">
<strong>Funding:</strong> National Science Foundation — Grant #2205472
</div>

---

<div class="prams-contact">
<h3>Join Us in Advancing Babies Pain Research</h3>
<ul>
<li>Collaborate with our research team.</li>
<li>Contribute neonatal data or video samples.</li>
<li>Support our mission.</li>
</ul>
<p><strong>Contact:</strong> <a href="mailto:renee.manworren@tamu.edu">renee.manworren@tamu.edu</a></p>
</div>

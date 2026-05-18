---
layout: page
title: PiEvo
description: Principle-Evolvable Scientific Discovery via Uncertainty Minimization.
img: /assets/img/project_pievo/framework.png
importance: 1
category: work
related_publications: false
---

<style>
body {
    font-family: 'Source Sans Pro', sans-serif;
    line-height: 1.6;
    color: #24292e;
    background-color: #f8f9fa;
}
.header {
    padding: 2rem 0;
    border-bottom: 1px solid #eaecef;
    margin-bottom: 2rem;
}
.authors {
    font-size: 1.2rem;
    margin-bottom: 1.5rem;
}
.equal-contrib {
    font-size: 0.9rem;
    font-style: italic;
}
.affiliation {
    font-size: 0.95rem;
    margin-bottom: 1rem;
}
.paper-links {
    margin: 2rem 0;
}
.paper-links a {
    margin-right: 1rem;
    text-decoration: none;
    padding: 0.5rem 1rem;
    border-radius: 4px;
    color: #fff;
    background-color: #7b1fae;
    transition: background-color 0.3s;
}
.paper-links a:hover {
    background-color: #4a148c;
}
.section-title {
    margin-top: 2.5rem;
    margin-bottom: 1.5rem;
    font-weight: 600;
    color: #4a148c;
}
.figure-caption {
    font-size: 0.9rem;
    color: #6c757d;
    text-align: center;
    margin-top: 0.5rem;
}
.reference {
    font-family: 'Courier New', monospace;
    font-size: 0.85rem;
    background-color: #f6f8fa;
    padding: 1rem;
    border-radius: 4px;
    white-space: pre-wrap;
    margin-top: 1.5rem;
}
.highlight {
    background-color: #f3e5f5;
    padding: 1.5rem;
    border-radius: 4px;
    margin-bottom: 1.5rem;
    border-left: 5px solid #7b1fae;
}
.card {
    margin-bottom: 1.5rem;
    border: none;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}
.card-header {
    background-color: #7b1fae;
    color: white;
    font-weight: 600;
}
.scientific-takeaway {
    background-color: #f3e5f5;
    border: 1px solid #d1c4e9;
    border-left: 4px solid #7b1fae;
    padding: 1.25rem;
    margin: 1.5rem 0;
    border-radius: 0 4px 4px 0;
    font-size: 0.95rem;
}
.scientific-takeaway .diamond {
    display: inline-block;
    margin-right: 5px;
    color: #7b1fae;
}
.pievo-highlight {
    font-family: 'Courier New', monospace;
    font-weight: 600;
}
</style>

<div class="container mt-4 mb-5">
<div class="header text-center">
    <h3 class="display-4">PiEvo: Principle-Evolvable Scientific Discovery via Uncertainty Minimization</h3>
    
    <div class="authors mt-4">
        <span><a href="https://dandelionym.github.io/" target="_blank">Yingming Pu</a><sup>1,2</sup></span>,
        <span>Tao Lin<sup>2,†</sup></span>,
        <span>and Hongyu Chen<sup>1</sup></span>
    </div>
    
    <div class="affiliation">
        <sup>1</sup> Westlake University<br>
        <sup>2</sup> Zhejiang University
    </div>
    
    <div class="equal-contrib">
        <sup>†</sup> Project Lead
    </div>
    
    <div class="paper-links">
        <a href="https://arxiv.org/pdf/2602.06448" target="_blank">
            📄 PDF
        </a>
        <a href="https://github.com/amair-lab/PiEvo" target="_blank">
            💻 GitHub
        </a>
    </div>
</div>

<div class="row">
    <div class="col-md-12 text-center">
        <div class="mb-4">
            <img src="/assets/img/project_pievo/framework.png" alt="PiEvo Framework Overview" class="img-fluid rounded shadow-lg">
            <p class="figure-caption">The PiEvo framework: A Bayesian-inspired dual-loop system for evolving scientific principles.</p>
        </div>
    </div>
</div>

<div class="row">
    <div class="col-lg-12">
        <div class="highlight">
            <p>
                Large Language Model (LLM)-based scientific agents often suffer from inefficiencies due to fixed initial priors and static hypothesis spaces. We propose <strong>PiEvo</strong>, a principle-evolvable framework that treats scientific discovery as Bayesian optimization over an expanding principle space. By integrating Information-Directed Hypothesis Selection (via Gaussian Process) and an anomaly-driven augmentation mechanism, PiEvo enables agents to autonomously refine their theoretical worldview. Evaluation across four benchmarks (physics, chemistry, biology, and materials science) shows that PiEvo improves solution quality by ~30% over state-of-the-art methods and achieves an 83.3% speedup in convergence.
            </p>
        </div>
    </div>
</div>

<div class="row">
    <div class="col-lg-12">
        <h2 class="section-title">Evolvable Principle Space</h2>
        <div class="card">
            <div class="card-header">
                The Core Innovation
            </div>
            <div class="card-body">
                <p>
                    PiEvo moves the paradigm of scientific discovery from searching in a static hypothesis space to optimizing an underlying, evolvable <strong>principle space</strong>. Key components include:
                </p>
                <ul>
                    <li>
                        <strong>Principle-Directed Selection:</strong> Using Bayesian updates to refine tentative principles based on experimental evidence.
                    </li>
                    <li>
                        <strong>Anomaly-Driven Augmentation:</strong> A mechanism that catalysts the expansion of the principle space when experimental outcomes significantly deviate from current predictions (high surprisal).
                    </li>
                    <li>
                        <strong>Dual-Loop Optimization:</strong> Minimizing uncertainty across the "Principle → Hypothesis" and "Evidence → Principle" pathways.
                    </li>
                </ul>
            </div>
        </div>
    </div>
</div>

<div class="row">
    <div class="col-lg-12">
        <h2 class="section-title">Performance & Convergence</h2>
        <div class="mb-4 text-center">
            <img src="/assets/img/project_pievo/results.png" alt="PiEvo Performance Comparison" class="img-fluid rounded">
            <p class="figure-caption">Quantitative results demonstrating PiEvo's superior solution quality and faster convergence across multiple scientific domains.</p>
        </div>
        
        <div class="scientific-takeaway">
            <p class="mb-0">
                <span class="diamond">◊</span>
                <strong>Key Result:</strong> <span class="pievo-highlight">PiEvo</span> achieves an average solution quality of 90.81%–93.15%, outperforming previous SOTA methods by up to 31.1% while attaining an 83.3% speedup in convergence.
            </p>
        </div>
    </div>
</div>

<div class="row">
    <div class="col-lg-12">
        <h2 class="section-title">Case Study: Advanced Electrodynamics</h2>
        <p>
            In a blind case study involving sub-wavelength chiral optics, PiEvo successfully identified novel electrodynamic mechanisms, specifically the <strong>toroidal-electric quadrupole interference</strong>. This discovery was made possible by the system's ability to "think outside the box" when faced with anomalous FDTD simulation data, evolving its theoretical understanding to include higher-order multipole interactions.
        </p>
    </div>
</div>

<div class="row">
    <div class="col-lg-12 text-center mt-5">
        <h2 class="section-title">Reference</h2>
        <div class="reference text-start text-left">@article{pu2026pievo,
  title={Principle-Evolvable Scientific Discovery via Uncertainty Minimization},
  author={Pu, Yingming and Lin, Tao and Chen, Hongyu},
  journal={arXiv preprint arXiv:2602.06448},
  year={2026}
}</div>
            </div>
        </div>
    </div>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

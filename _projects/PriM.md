---
layout: page
title: PriM
description: We introduce a hypothesis-validation framework with language model-based multi-agent system for scientific discovery. 
img: /assets/img/prim.png
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
    background-color: #0366d6;
    transition: background-color 0.3s;
}
.paper-links a:hover {
    background-color: #0250a0;
}
.section-title {
    margin-top: 2.5rem;
    margin-bottom: 1.5rem;
    font-weight: 600;
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
    background-color: #f0f4f8;
    padding: 1.5rem;
    border-radius: 4px;
    margin-bottom: 1.5rem;
}
.card {
    margin-bottom: 1.5rem;
    border: none;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}
.card-header {
    background-color: #0366d6;
    color: white;
    font-weight: 600;
}
</style>

<div class="container mt-4 mb-5">
<div class="header text-center">
    <h3 class="display-4">PriM: Principle-Inspired Material Discovery through Multi-Agent Collaboration</h3>
    
    <div class="authors mt-4">
        <span><a href="https://zheyuanlai.github.io/" target="_blank">Zheyuan Lai</a><sup>1,†</sup></span>
        <span> and </span>
        <span><a href="https://dandelionym.github.io/" target="_blank">Yingming Pu</a><sup>2,3,†</sup> (Corresponding author)</span>
    </div>
    
    <div class="affiliation">
        <sup>1</sup> National University of Singapore<br>
        <sup>2</sup> Westlake University<br>
        <sup>3</sup> Zhejiang University
    </div>
    
    <div class="equal-contrib">
        <sup>†</sup> Equal Contribution
    </div>
    
    <div class="paper-links">
        <a href="https://openreview.net/pdf?id=lhobZk76wX" target="_blank">
            📄 PDF
        </a>
        <a href="https://github.com/amair-lab/PriM" target="_blank">
            💻 GitHub
        </a>
    </div>
</div>

<div class="row">
    <div class="col-md-12">
        <div class="mb-4">
            <img src="/assets/img/project_prim/schema.png" alt="PriM Framework Overview" class="img-fluid">
        </div>
    </div>
</div>

<div class="row">
    <div class="col-lg-12">
        <div class="highlight">
            <p>
                Complex chemical space and limited knowledge scope with biases holds immense challenge for human scientists, yet in automated materials discovery. Existing intelligent methods relies more on numerical computation, leading to inefficient exploration and results with hard-interpretability. To bridge this gap, we introduce a principles-guided materials discovery workflow powered by language inferential multi-agent system (MAS). Our framework integrates automated hypothesis generation with experimental validation in a roundtable system of MAS, enabling systematic exploration while maintaining scientific rigor. Based on our framework, the case study of nano helix demonstrates higher materials exploration rate and property value while providing transparent reasoning pathways. This approach develops an automated-and-transparent paradigm for material discovery, with broad implications for rational design of functional materials.
            </p>
        </div>
    </div>
</div>

<div class="row">
    <div class="col-lg-12">
        <h2 class="section-title">Framework Overview</h2>
        <div class="card">
            <div class="card-header">
                The PriM Multi-Agent System
            </div>
            <div class="card-body">
                <p>
                    The PriM framework bridges the gap between traditional data-driven methods and principled scientific reasoning. It achieves this by combining:
                </p>
                <ul>
                    <li>
                        <strong>Hypothesis Generation:</strong> A Literature Agent retrieves relevant scientific knowledge, and a Hypothesis Agent formulates testable propositions based on physicochemical principles.
                    </li>
                    <li>
                        <strong>Experimental Validation:</strong> An Experiment Agent designs and executes virtual experiments, while an Optimizer Agent refines the parameter space via Monte Carlo Tree Search (MCTS) to maximize the desired material property.
                    </li>
                    <li>
                        <strong>Transparent Reasoning:</strong> All decision-making is traceable through explicit, human-readable reasoning paths, facilitating deeper insights into material behavior.
                    </li>
                </ul>
            </div>
        </div>
    </div>
</div>

<div class="row">
    <div class="col-lg-12">
        <h2 class="section-title">Case Study: Nano Helix Material Discovery</h2>
        <div class="mb-4">
            <img src="/assets/img/project_prim/case_study.png" alt="Nano Helix Case Study" class="img-fluid">
            <p class="figure-caption">PriM applied to nano helix material discovery, demonstrating iterative agent collaboration and significant property improvements.</p>
        </div>
        <p>
            The system is demonstrated on a nano helix material discovery case study, where iterative agent collaboration results in significant improvements in material properties compared to conventional methods. The transparent reasoning paths provide insights into the material behavior and guide further exploration.
        </p>
    </div>
</div>

<div class="row">
    <div class="col-lg-12">
        <h2 class="section-title">Key Advantages</h2>
        <div class="row">
            <div class="col-md-4">
                <div class="card h-100">
                    <div class="card-header">
                        Principled Exploration
                    </div>
                    <div class="card-body">
                        <p>
                            Combines scientific principles with data-driven optimization, enabling more efficient navigation of complex chemical space.
                        </p>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card h-100">
                    <div class="card-header">
                        Transparent Reasoning
                    </div>
                    <div class="card-body">
                        <p>
                            Provides human-readable reasoning paths, allowing scientists to understand and validate the material discovery process.
                        </p>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card h-100">
                    <div class="card-header">
                        Collaborative Intelligence
                    </div>
                    <div class="card-body">
                        <p>
                            Multiple specialized agents work together to address different aspects of the discovery process, leading to more comprehensive solutions.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

<div class="row mt-4">
    <div class="col-lg-12">
        <h2 class="section-title">Reference</h2>
        <div class="reference">@inproceedings{pu2025prim,
  title = {PriM: Principle-Inspired Material Discovery through Multi-Agent Collaboration},
  author = {Zheyuan Lai and Yingming Pu},
  booktitle = {ICLR 2025 Workshop on AI for Accelerated Materials Design},
  year = {2025},
  month = mar,
  url = {https://openreview.net/pdf?id=lhobZk76wX},
}</div>
            </div>
        </div>
    </div>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
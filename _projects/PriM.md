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
/* Academic table styles */
.academic-table-container {
    margin: 2rem 0;
    overflow-x: auto;
}
.academic-table {
    width: 100%;
    border-collapse: collapse;
    font-size: 0.95rem;
    background-color: white;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
}
.academic-table caption {
    font-weight: 600;
    font-size: 1.1rem;
    padding: 0.75rem;
    color: #212529;
    caption-side: top;
    text-align: center;
    border-bottom: 1px solid #dee2e6;
    background-color: #f8f9fa;
}
.academic-table th {
    background-color: #f1f5f9;
    color: #334155;
    font-weight: 600;
    text-align: center;
    padding: 0.75rem;
    border: 1px solid #dee2e6;
}
.academic-table td {
    padding: 0.75rem;
    border: 1px solid #dee2e6;
    text-align: center;
}
.academic-table tbody tr:nth-of-type(even) {
    background-color: #f9fafb;
}
.academic-table tbody tr:hover {
    background-color: #f1f5f9;
}
.academic-table .highlight-row {
    background-color: rgba(13, 110, 253, 0.05) !important;
}
.scientific-takeaway {
    background-color: #f1f5f9;
    border: 1px solid #cbd5e1;
    border-left: 4px solid #0366d6;
    padding: 1.25rem;
    margin: 1.5rem 0;
    border-radius: 0 4px 4px 0;
    font-size: 0.95rem;
}
.scientific-takeaway .diamond {
    display: inline-block;
    margin-right: 5px;
    color: #0366d6;
}
.prim-highlight {
    font-family: 'Courier New', monospace;
    font-weight: 600;
}
.table-note {
    font-size: 0.85rem;
    color: #64748b;
    text-align: center;
    margin-top: 0.5rem;
    font-style: italic;
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
        <h2 class="section-title">Results and Comparative Analysis</h2>
        <p>
            We evaluated the performance of <span class="prim-highlight">PriM</span> against several baseline methods including Bayesian Optimization (BO), Deep Q-Networks (DQN), and traditional multi-agent systems. The quantitative results are presented in Table 1.
        </p>
        
        <div class="academic-table-container">
            <table class="academic-table">
                <caption>Table 1: Quantitative Comparison of <span class="prim-highlight">PriM</span> with Baseline Methods (mean ± std)</caption>
                <thead>
                    <tr>
                        <th>Method</th>
                        <th>Rationality</th>
                        <th>Optimal Value (μ)</th>
                        <th>Exploration Rate (ε)</th>
                        <th>Iteration</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>BO</td>
                        <td>N/A</td>
                        <td>1.081 (± 0.065)</td>
                        <td>467.35 (± 23.52)</td>
                        <td>14.29 (± 2.34)</td>
                    </tr>
                    <tr>
                        <td>DQN</td>
                        <td>N/A</td>
                        <td>1.050 (± 0.021)</td>
                        <td>6.75 (± 0.30)</td>
                        <td>20.00 (± 0.00)</td>
                    </tr>
                    <tr>
                        <td>Vanilla Agent</td>
                        <td>Naive Logics</td>
                        <td>0.644 (± 0.054)</td>
                        <td>24.47 (± 7.34)</td>
                        <td>9.20 (± 2.56)</td>
                    </tr>
                    <tr>
                        <td>Vanilla MAS</td>
                        <td>Naive Logics</td>
                        <td>0.923 (± 0.170)</td>
                        <td>264.65 (± 22.42)</td>
                        <td>65.40 (± 18.91)</td>
                    </tr>
                    <tr class="highlight-row">
                        <td><span class="prim-highlight">PriM</span> (Ours)</td>
                        <td>Principles</td>
                        <td>1.007 (± 0.103)</td>
                        <td>49.68 (± 10.07)</td>
                        <td>85.50 (± 8.58)</td>
                    </tr>
                </tbody>
            </table>
            <p class="table-note">n = 5 independent runs for each method; all values reported as mean ± standard deviation.</p>
        </div>
        
        <div class="scientific-takeaway">
            <p class="mb-0">
                <span class="diamond">◊</span>
                <strong>Key Finding:</strong> <span class="prim-highlight">PriM</span> achieves near-optimal material properties (μ = 1.007 ± 0.103) while maintaining scientific rationality through principle-guided approaches. The significantly lower exploration rate (ε = 49.68 ± 10.07) compared to Vanilla MAS (ε = 264.65 ± 22.42) demonstrates more efficient and targeted parameter space traversal, effectively balancing performance optimization with mechanistic understanding.
            </p>
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
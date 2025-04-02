---
layout: page
permalink: /people/
title: Group
description: Members and architectures of AMAIR
nav: true
nav_order: 7
---

<!-- Custom CSS for the lab members page -->
<style>
  /* Base styles */
  .team-section {
    padding: 2rem 0;
  }
  
  /* Team categories */
  .team-category {
    margin-bottom: 3rem;
  }
  
  .category-title {
    font-size: 1.8rem;
    font-weight: 300;
    margin-bottom: 2rem;
    position: relative;
    display: inline-block;
    color: #333;
  }
  
  .category-title::after {
    content: '';
    position: absolute;
    width: 40px;
    height: 2px;
    background-color: #b509ac;
    bottom: -10px;
    left: 0;
  }
  
  /* Member cards */
  .member-card {
    background-color: #fff;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 3px 15px rgba(0,0,0,0.05);
    transition: all 0.3s ease;
    height: 100%;
    display: flex;
    flex-direction: column;
  }
  
  .member-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(0,0,0,0.1);
  }
  
  .member-avatar {
    width: 100%;
    height: 150px;
    overflow: hidden;
    position: relative;
    background-color: #f5f7fa;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  .member-avatar img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: all 0.5s ease;
  }
  
  .member-avatar .member-initial {
    font-size: 5rem;
    font-weight: 300;
    color: #b509ac;
    opacity: 0.5;
  }
  
  .member-card:hover .member-avatar img {
    transform: scale(1.05);
  }
  
  .member-info {
    padding: 1.5rem;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }
  
  .member-name {
    font-size: 1.4rem;
    font-weight: 500;
    margin-bottom: 0.5rem;
    color: #222;
  }
  
  .member-role {
    font-size: 0.95rem;
    color: #666;
    margin-bottom: 1rem;
  }
  
  .member-bio {
    font-size: 0.95rem;
    color: #444;
    margin-bottom: 1.5rem;
    flex-grow: 1;
  }
  
  .member-links {
    display: flex;
    gap: 15px;
    margin-top: auto;
  }
  
  .member-link {
    display: inline-flex;
    align-items: center;
    color: #0366d6;
    font-size: 0.9rem;
    transition: all 0.2s ease;
  }
  
  .member-link:hover {
    color: #0250a0;
    text-decoration: none;
  }
  
  .member-link i {
    margin-right: 5px;
  }
  
  .leader-badge {
    display: inline-block;
    padding: 3px 8px;
    background-color: rgba(3, 102, 214, 0.1);
    color: #0366d6;
    border-radius: 4px;
    font-size: 0.8rem;
    font-weight: 500;
    margin-left: 10px;
    vertical-align: middle;
  }
  
  /* For mobile devices */
  @media (max-width: 768px) {
    .member-avatar {
      height: 250px;
    }
    
    .member-links {
      flex-direction: column;
      gap: 10px;
    }
  }
</style>

<!-- FontAwesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">

<div class="team-section">
  <!-- Lab Members Section -->
  <div class="team-category">
    <h2 class="category-title">Lab Members</h2>
    
    <div class="row">
      <div class="col-md-4">
        <div class="member-card">
          <div class="member-avatar">
            <!-- If you have an image, use this line instead of the div below -->
            <!-- <img src="/assets/img/members/mellen-pu.jpg" alt="Mellen Y. Pu"> -->
            <div class="member-initial">M</div>
          </div>
          <div class="member-info">
            <h3 class="member-name">Mellen Y. Pu <span class="leader-badge">Lab Leader</span></h3>
            <div class="member-role">Lab Leader</div>
            <div class="member-bio">
              Language models for scientific discovery
            </div>
            <div class="member-links">
              <a href="https://dandelionym.github.io/" class="member-link" target="_blank">
                <i class="fas fa-globe"></i> Website
              </a>
              <a href="wias.ym@gmail.com" class="member-link">
                <i class="fas fa-envelope"></i> Email
              </a>
              <a href="https://github.com/dandelionym" class="member-link" target="_blank">
                <i class="fab fa-github"></i> GitHub
              </a>
            </div>
          </div>
        </div>
      </div>
      



      <div class="col-md-4">
        <div class="member-card">
          <div class="member-avatar">
            <!-- If you have an image, use this line instead of the div below -->
            <!-- <img src="/assets/img/members/zheyuan-lai.jpg" alt="Ryan Zheyuan Lai"> -->
            <div class="member-initial">R</div>
          </div>
          <div class="member-info">
            <h3 class="member-name">Ryan Zheyuan Lai</h3>
            <div class="member-role">Core Member</div>
            <div class="member-bio">
              Research focus on multi-agent systems
            </div>
            <div class="member-links">
              <a href="https://zheyuanlai.github.io/" class="member-link" target="_blank">
                <i class="fas fa-globe"></i> Website
              </a>
              <a href="#" class="member-link">
                <i class="fas fa-envelope"></i> Email
              </a>
              <a href="https://github.com/zheyuanlai" class="member-link" target="_blank">
                <i class="fab fa-github"></i> GitHub
              </a>
            </div>
          </div>
        </div>
      </div>




      <!-- You can add more members by duplicating the col-md-4 div above -->
      <!-- For example: -->
      <!-- 
      <div class="col-md-4">
        <div class="member-card">
          ... Next member content ...
        </div>
      </div>
      -->
    </div>
  </div>
</div>

<!-- Optional JavaScript for additional interactions -->
<script>
  document.addEventListener('DOMContentLoaded', function() {
    // Additional JavaScript functionality can be added here if needed
  });
</script>
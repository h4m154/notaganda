---
layout: single
title: "About NotAGanda"
permalink: /about/
author_profile: false
toc: true
toc_sticky: true
---

<div class="about-page">
  <div class="about-header">
    <div class="profile-image">
      <!-- Replace with your actual profile image -->
      <div class="profile-image-placeholder">
        <i class="fas fa-user"></i>
      </div>
    </div>
    
    <div class="about-intro">
      <h1>Welcome to NotAGanda</h1>
      <p class="subtitle">Your central hub for content across multiple platforms</p>
    </div>
  </div>

  <div class="about-content">
    <div class="about-section">
      <h2>My Story</h2>
      <p>I created this hub as a central location to gather all my video content from across multiple platforms. Whether you're a longtime subscriber or just discovering my content, this site makes it easy to find all my videos in one place.</p>
      <p>My journey started in [year], and since then, I've been creating content that aims to [your content mission]. Through my videos, I strive to [what you aim to achieve with your content].</p>
    </div>

    <div class="about-section platforms-section">
      <h2>Where To Find My Content</h2>
      <div class="platform-grid">
        <div class="platform-card">
          <i class="fab fa-youtube"></i>
          <h3>YouTube</h3>
          <p>Long-form videos and detailed discussions on a variety of topics.</p>
          <a href="https://youtube.com/yourusername" target="_blank" class="platform-link">Visit Channel</a>
        </div>
        
        <div class="platform-card">
          <i class="fab fa-twitch"></i>
          <h3>Twitch</h3>
          <p>Live streams and interactive sessions where we can connect in real-time.</p>
          <a href="https://twitch.tv/yourusername" target="_blank" class="platform-link">Watch Streams</a>
        </div>
        
        <div class="platform-card">
          <i class="fab fa-tiktok"></i>
          <h3>TikTok</h3>
          <p>Short-form videos and quick updates for bite-sized content.</p>
          <a href="https://tiktok.com/@yourusername" target="_blank" class="platform-link">View TikToks</a>
        </div>
        
        <div class="platform-card">
          <i class="fab fa-twitter"></i>
          <h3>Twitter</h3>
          <p>News, updates, and conversations about the latest developments.</p>
          <a href="https://twitter.com/yourusername" target="_blank" class="platform-link">Follow Me</a>
        </div>
      </div>
    </div>
    
    <div class="about-section mission-section">
      <h2>My Mission</h2>
      <div class="mission-content">
        <div class="mission-text">
          <p>My goal is to create engaging, informative, and entertaining content that resonates with my audience. I believe in:</p>
          <ul>
            <li><strong>Quality Over Quantity</strong> - Creating content that adds value</li>
            <li><strong>Transparent Communication</strong> - Being honest with my audience</li>
            <li><strong>Community Building</strong> - Creating connections between viewers</li>
            <li><strong>Continuous Improvement</strong> - Always learning and evolving</li>
          </ul>
        </div>
        <div class="mission-graphic">
          <div class="mission-icon">
            <i class="fas fa-bullseye"></i>
          </div>
        </div>
      </div>
    </div>
    
    <div class="about-section skills-section">
      <h2>Content Focus</h2>
      <div class="skills-bars">
        <div class="skill-bar">
          <div class="skill-info">
            <span>Entertainment</span>
            <span>80%</span>
          </div>
          <div class="skill-progress">
            <div class="skill-progress-bar" style="width: 80%;"></div>
          </div>
        </div>
        
        <div class="skill-bar">
          <div class="skill-info">
            <span>Education</span>
            <span>75%</span>
          </div>
          <div class="skill-progress">
            <div class="skill-progress-bar" style="width: 75%;"></div>
          </div>
        </div>
        
        <div class="skill-bar">
          <div class="skill-info">
            <span>News & Commentary</span>
            <span>65%</span>
          </div>
          <div class="skill-progress">
            <div class="skill-progress-bar" style="width: 65%;"></div>
          </div>
        </div>
        
        <div class="skill-bar">
          <div class="skill-info">
            <span>Community Building</span>
            <span>90%</span>
          </div>
          <div class="skill-progress">
            <div class="skill-progress-bar" style="width: 90%;"></div>
          </div>
        </div>
      </div>
    </div>
    
    <div class="about-section cta-section">
      <h2>Get in Touch</h2>
      <p>I love hearing from viewers and am always open to collaboration opportunities, suggestions, or just a friendly hello.</p>
      <div class="cta-buttons">
        <a href="/contact/" class="btn btn-hero">Contact Me</a>
        <a href="/donate/" class="btn btn-secondary">Support My Work</a>
      </div>
    </div>
  </div>
</div>

<style>
  .about-page {
    max-width: 1000px;
    margin: 0 auto 5rem;
    padding: 0 1.5rem;
  }
  
  .about-header {
    display: flex;
    align-items: center;
    gap: 2.5rem;
    margin: 4rem 0 5rem;
    flex-wrap: wrap;
  }
  
  .profile-image {
    flex: 0 0 180px;
    height: 180px;
    border-radius: 50%;
    overflow: hidden;
    box-shadow: var(--shadow-md);
    border: 3px solid var(--color-bg-tertiary);
    position: relative;
  }
  
  .profile-image-placeholder {
    width: 100%;
    height: 100%;
    background: var(--gradient-secondary);
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  .profile-image-placeholder i {
    font-size: 80px;
    color: rgba(255, 255, 255, 0.8);
  }
  
  .about-intro {
    flex: 1;
  }
  
  .about-intro h1 {
    font-size: 2.8rem;
    margin: 0 0 1rem;
    color: var(--color-text-primary);
  }
  
  .about-intro .subtitle {
    font-size: 1.4rem;
    margin: 0;
    color: var(--color-text-secondary);
    font-weight: 300;
  }
  
  .about-content {
    display: flex;
    flex-direction: column;
    gap: 5rem;
  }
  
  .about-section {
    position: relative;
  }
  
  .about-section h2 {
    font-size: 2rem;
    margin-bottom: 1.5rem;
    color: var(--color-text-primary);
    position: relative;
    padding-bottom: 0.5rem;
  }
  
  .about-section h2::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 80px;
    height: 4px;
    background: var(--gradient-primary);
    border-radius: 2px;
  }
  
  .about-section p {
    font-size: 1.1rem;
    line-height: 1.7;
    color: var(--color-text-secondary);
    margin-bottom: 1.2rem;
  }
  
  /* Platforms Section */
  .platform-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
  }
  
  .platform-card {
    background-color: var(--color-bg-secondary);
    border-radius: 10px;
    padding: 2rem 1.5rem;
    text-align: center;
    transition: transform var(--transition-medium), box-shadow var(--transition-medium);
    position: relative;
    overflow: hidden;
    box-shadow: var(--shadow-sm);
  }
  
  .platform-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 5px;
    background: var(--gradient-primary);
    opacity: 0;
    transition: opacity var(--transition-medium);
  }
  
  .platform-card:hover {
    transform: translateY(-10px);
    box-shadow: var(--shadow-md);
  }
  
  .platform-card:hover::before {
    opacity: 1;
  }
  
  .platform-card i {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    color: var(--color-accent-primary);
  }
  
  .platform-card h3 {
    font-size: 1.3rem;
    margin-bottom: 0.8rem;
    color: var(--color-text-primary);
  }
  
  .platform-card p {
    font-size: 0.95rem;
    color: var(--color-text-secondary);
    margin-bottom: 1.5rem;
  }
  
  .platform-link {
    display: inline-flex;
    align-items: center;
    font-weight: 500;
    color: var(--color-accent-tertiary) !important;
    transition: all var(--transition-fast);
  }
  
  .platform-link::after {
    content: '→';
    opacity: 0;
    margin-left: 0;
    transition: opacity var(--transition-fast), margin-left var(--transition-fast);
  }
  
  .platform-card:hover .platform-link::after {
    opacity: 1;
    margin-left: 5px;
  }
  
  /* Mission Section */
  .mission-content {
    display: flex;
    gap: 3rem;
    align-items: center;
    flex-wrap: wrap;
  }
  
  .mission-text {
    flex: 2 1 400px;
  }
  
  .mission-text ul {
    padding-left: 1.5rem;
  }
  
  .mission-text li {
    margin-bottom: 0.8rem;
    color: var(--color-text-secondary);
  }
  
  .mission-text li strong {
    color: var(--color-text-primary);
  }
  
  .mission-graphic {
    flex: 1 1 200px;
    display: flex;
    justify-content: center;
  }
  
  .mission-icon {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    background: var(--gradient-secondary);
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  .mission-icon i {
    font-size: 70px;
    color: rgba(255, 255, 255, 0.9);
  }
  
  /* Skills Section */
  .skills-bars {
    margin-top: 2rem;
  }
  
  .skill-bar {
    margin-bottom: 1.5rem;
  }
  
  .skill-info {
    display: flex;
    justify-content: space-between;
    margin-bottom: 0.5rem;
  }
  
  .skill-info span {
    color: var(--color-text-secondary);
    font-weight: 500;
  }
  
  .skill-progress {
    height: 10px;
    background-color: var(--color-bg-tertiary);
    border-radius: 5px;
    overflow: hidden;
  }
  
  .skill-progress-bar {
    height: 100%;
    background: var(--gradient-primary);
    border-radius: 5px;
    animation: progress 1.5s ease-in-out;
  }
  
  @keyframes progress {
    0% {
      width: 0%;
    }
  }
  
  /* CTA Section */
  .cta-section {
    text-align: center;
    background-color: var(--color-bg-secondary);
    padding: 3rem;
    border-radius: 12px;
    margin-top: 2rem;
    box-shadow: var(--shadow-sm);
  }
  
  .cta-section h2 {
    text-align: center;
  }
  
  .cta-section h2::after {
    left: 50%;
    transform: translateX(-50%);
  }
  
  .cta-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    margin-top: 2rem;
  }
  
  @media (max-width: 768px) {
    .about-header {
      flex-direction: column;
      align-items: center;
      text-align: center;
      gap: 1.5rem;
    }
    
    .about-intro h1 {
      font-size: 2.2rem;
    }
    
    .about-section h2 {
      font-size: 1.8rem;
    }
    
    .about-section h2::after {
      left: 50%;
      transform: translateX(-50%);
    }
    
    .platform-grid {
      grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
    }
    
    .about-section {
      text-align: center;
    }
    
    .mission-content {
      flex-direction: column;
      gap: 2rem;
    }
    
    .mission-text ul {
      text-align: left;
    }
    
    .cta-buttons {
      flex-direction: column;
      gap: 1rem;
    }
    
    .cta-buttons .btn {
      width: 100%;
    }
  }
</style>

Thank you for being part of this journey! 
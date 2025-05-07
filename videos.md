---
layout: single
title: "Videos"
permalink: /videos/
---

<div class="video-section">
  <div class="video-section-inner">
    <div class="section-header">
      <h2>All Videos</h2>
    </div>
    
    <div class="platform-tabs">
      <button class="platform-tab active" data-platform="all">All</button>
      <button class="platform-tab" data-platform="YouTube">YouTube</button>
      <button class="platform-tab" data-platform="Twitch">Twitch</button>
      <button class="platform-tab" data-platform="TikTok">TikTok</button>
      <button class="platform-tab" data-platform="Other">Other</button>
    </div>
    
    <div class="video-grid">
      {% assign sorted_videos = site.data.videos | sort: 'date' | reverse %}
      {% for video in sorted_videos %}
        <div class="video-card" data-platform="{{ video.platform }}">
          <div class="video-container">
            <iframe src="{{ video.embed_url }}" frameborder="0" allowfullscreen></iframe>
          </div>
          <h3>{{ video.title }}</h3>
          <div class="video-meta">
            <span class="video-date">{{ video.date | date: "%B %d, %Y" }}</span>
            <span class="video-platform">{{ video.platform }}</span>
          </div>
          <p class="video-description">{{ video.description }}</p>
          <div class="video-platform">
            <a href="{{ video.url }}" class="platform-link" target="_blank">Watch on {{ video.platform }}</a>
          </div>
        </div>
      {% endfor %}
    </div>
  </div>
</div>

<style>
  .platform-tabs {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 10px;
    margin-bottom: 2rem;
  }
  
  .platform-tab {
    background-color: var(--color-bg-secondary);
    border: none;
    padding: 8px 16px;
    border-radius: 20px;
    cursor: pointer;
    transition: all 0.3s ease;
    color: var(--color-text-secondary);
  }
  
  .platform-tab.active, .platform-tab:hover {
    background-color: var(--color-accent-primary);
    color: var(--color-text-primary);
  }
  
  .video-meta {
    display: flex;
    justify-content: space-between;
    color: var(--color-text-muted);
    font-size: 0.9rem;
    margin: 0.5rem 1.2rem 1rem;
  }
  
  .video-description {
    padding: 0 1.2rem;
    margin-bottom: 1rem;
    color: var(--color-text-secondary);
  }
</style>

<script>
  document.addEventListener('DOMContentLoaded', function() {
    const tabs = document.querySelectorAll('.platform-tab');
    const videos = document.querySelectorAll('.video-card');
    
    tabs.forEach(tab => {
      tab.addEventListener('click', function() {
        // Remove active class from all tabs
        tabs.forEach(t => t.classList.remove('active'));
        
        // Add active class to clicked tab
        this.classList.add('active');
        
        // Get platform filter
        const platform = this.getAttribute('data-platform');
        
        // Filter videos
        videos.forEach(video => {
          if (platform === 'all' || video.getAttribute('data-platform') === platform) {
            video.style.display = 'block';
          } else {
            video.style.display = 'none';
          }
        });
      });
    });
  });
</script> 
---
layout: home
title: "Notaganda"
permalink: /
---

<section class="home-hero">
  <div class="hero-background">
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
  </div>
  <div class="container">
    <h1>Notaganda</h1>
    <p>Your central destination for all my video content across multiple platforms.</p>
    <div class="hero-buttons">
      <a class="btn btn-hero" href="#videos">Watch Videos</a>
      <a class="btn btn-secondary" href="/blog/">Read Blog</a>
    </div>
  </div>
</section>

<div class="home-sections">
  <section class="about-preview" id="about-preview">
    <h2>About</h2>
    <p>Learn more about who I am, my video creation journey, and the platforms where my content is available.</p>
    <a class="btn" href="/about/">Learn More</a>
  </section>

  <section class="blog-preview">
    <h2>Latest News</h2>
    <p>Check out my latest blog posts, updates, and announcements about new content releases.</p>
    <a class="btn" href="/blog/">View Blog</a>
  </section>

  <section class="support-preview">
    <h2><i class="fas fa-heart" style="color: var(--color-accent-primary); margin-right: 7px;"></i>Support</h2>
    <p>If you enjoy my content, consider supporting my work through various platforms and donations.</p>
    <a class="btn btn-hero" href="/donate/">Support Me</a>
  </section>
</div>

<section class="video-section" id="videos">
  <div class="video-section-inner">
    <div class="section-header">
      <h2>Featured Videos</h2>
    </div>
    <div class="video-grid">
      {% for video in site.data.videos limit:6 %}
        <div class="video-card">
          <div class="video-container">
            <iframe src="{{ video.embed_url }}" frameborder="0" allowfullscreen></iframe>
          </div>
          <h3>{{ video.title }}</h3>
          <div class="video-platform">
            <a href="{{ video.url }}" class="platform-link" target="_blank">Watch on {{ video.platform }}</a>
          </div>
        </div>
      {% endfor %}
    </div>
    <div class="section-footer">
      <a href="/videos/" class="btn btn-hero">View All Videos</a>
    </div>
  </div>
</section>

<section class="blog-section page-section">
  <div class="container">
    <div class="section-header">
      <h2>From The Blog</h2>
    </div>
    <div class="blog-grid">
      {% for post in site.posts limit:3 %}
        <div class="blog-card">
          <div class="post-date">{{ post.date | date: "%B %d, %Y" }}</div>
          <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
          <div class="post-excerpt">{{ post.content | strip_html | truncatewords: 30 }}</div>
          <a href="{{ post.url }}" class="read-more">Read More</a>
        </div>
      {% endfor %}
    </div>
    <div class="section-footer">
      <a href="/blog/" class="btn btn-secondary">View All Posts</a>
    </div>
  </div>
</section>

<section class="social-section page-section">
  <div class="container">
    <div class="section-header">
      <h2>Follow Me</h2>
    </div>
    <div class="social-links">
      {% if site.social.youtube %}
        <a href="{{ site.social.youtube }}" target="_blank" class="social-link youtube">
          <span class="sr-only">YouTube</span>
          <i class="fab fa-youtube"></i>
        </a>
      {% endif %}
      {% if site.social.twitter %}
        <a href="{{ site.social.twitter }}" target="_blank" class="social-link twitter">
          <span class="sr-only">Twitter</span>
          <i class="fab fa-twitter"></i>
        </a>
      {% endif %}
      {% if site.social.instagram %}
        <a href="{{ site.social.instagram }}" target="_blank" class="social-link instagram">
          <span class="sr-only">Instagram</span>
          <i class="fab fa-instagram"></i>
        </a>
      {% endif %}
      {% if site.social.twitch %}
        <a href="{{ site.social.twitch }}" target="_blank" class="social-link twitch">
          <span class="sr-only">Twitch</span>
          <i class="fab fa-twitch"></i>
        </a>
      {% endif %}
      {% if site.social.tiktok %}
        <a href="{{ site.social.tiktok }}" target="_blank" class="social-link tiktok">
          <span class="sr-only">TikTok</span>
          <i class="fab fa-tiktok"></i>
        </a>
      {% endif %}
    </div>
  </div>
</section>

{% include donate.html %} 
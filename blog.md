---
layout: single
title: "Blog"
permalink: /blog/
classes: wide
---

<div class="blog-hero">
  <h1>NotAGanda Blog</h1>
  <p>Updates, thoughts, and news about my video content across various platforms.</p>
</div>

<div class="blog-feed">
  {% for post in site.posts %}
    <article class="blog-entry">
      <div class="post-meta">
        <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
        {% if post.categories.size > 0 %}
          <span class="post-categories">
            {% for category in post.categories %}
              <a href="/categories/#{{ category | slugify }}" class="post-category">{{ category }}</a>
            {% endfor %}
          </span>
        {% endif %}
      </div>
      <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <div class="post-excerpt">
        {{ post.content | strip_html | truncatewords: 50 }}
      </div>
      <div class="post-footer">
        <a href="{{ post.url }}" class="read-more">Continue Reading</a>
      </div>
    </article>
  {% endfor %}
</div>

<style>
  .blog-hero {
    text-align: center;
    padding: 6rem 1rem 4rem;
    margin-bottom: 3rem;
    position: relative;
    background-color: var(--color-bg-primary);
    overflow: hidden;
  }
  
  .blog-hero::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: radial-gradient(circle at center, rgba(77, 201, 240, 0.1) 0%, rgba(10, 10, 10, 0) 70%);
    z-index: 0;
  }
  
  .blog-hero h1 {
    font-size: 3rem;
    font-weight: 700;
    margin-bottom: 1rem;
    color: var(--color-text-primary);
    position: relative;
    z-index: 1;
    background: var(--gradient-secondary);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    text-fill-color: transparent;
  }
  
  .blog-hero p {
    font-size: 1.25rem;
    max-width: 700px;
    margin: 0 auto;
    color: var(--color-text-secondary);
    position: relative;
    z-index: 1;
  }
  
  .blog-feed {
    max-width: 900px;
    margin: 0 auto 5rem;
    padding: 0 1.5rem;
  }
  
  .blog-entry {
    margin-bottom: 4rem;
    padding-bottom: 4rem;
    border-bottom: 1px solid var(--color-bg-tertiary);
    position: relative;
  }
  
  .blog-entry:last-child {
    border-bottom: none;
  }
  
  .post-meta {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    margin-bottom: 1rem;
    font-size: 0.9rem;
  }
  
  .post-date {
    color: var(--color-text-muted);
    display: flex;
    align-items: center;
  }
  
  .post-date::before {
    content: "";
    display: inline-block;
    width: 12px;
    height: 12px;
    margin-right: 8px;
    background-color: var(--color-accent-secondary);
    border-radius: 50%;
    opacity: 0.5;
  }
  
  .post-categories {
    display: flex;
    gap: 0.5rem;
  }
  
  .post-category {
    background-color: var(--color-bg-tertiary);
    padding: 0.2rem 0.6rem;
    border-radius: 4px;
    font-size: 0.8rem;
    text-transform: uppercase;
    font-weight: 500;
    letter-spacing: 0.5px;
    transition: background-color var(--transition-fast), color var(--transition-fast);
  }
  
  .post-category:hover {
    background-color: var(--color-accent-primary);
    color: white !important;
  }
  
  .post-title {
    margin-top: 0.5rem;
    margin-bottom: 1.2rem;
    font-size: 2rem;
    line-height: 1.3;
  }
  
  .post-title a {
    color: var(--color-text-primary) !important;
    text-decoration: none;
    transition: color var(--transition-fast);
    background-image: linear-gradient(transparent 0%, transparent calc(100% - 3px), var(--color-accent-tertiary) calc(100% - 3px), var(--color-accent-tertiary) 100%);
    background-size: 0 100%;
    background-repeat: no-repeat;
    transition: background-size var(--transition-medium);
  }
  
  .post-title a:hover {
    background-size: 100% 100%;
  }
  
  .post-excerpt {
    color: var(--color-text-secondary);
    font-size: 1.05rem;
    line-height: 1.7;
    margin-bottom: 1.5rem;
  }
  
  .post-footer {
    display: flex;
    justify-content: flex-start;
  }
  
  .read-more {
    display: inline-flex;
    align-items: center;
    font-weight: 500;
    color: var(--color-accent-tertiary) !important;
    position: relative;
    transition: all var(--transition-fast);
  }
  
  .read-more::after {
    content: '→';
    opacity: 0;
    margin-left: 0;
    transition: opacity var(--transition-fast), margin-left var(--transition-fast);
  }
  
  .read-more:hover::after {
    opacity: 1;
    margin-left: 5px;
  }
  
  @media (max-width: 768px) {
    .blog-hero h1 {
      font-size: 2.5rem;
    }
    
    .blog-hero p {
      font-size: 1.1rem;
    }
    
    .post-title {
      font-size: 1.8rem;
    }
  }
</style> 
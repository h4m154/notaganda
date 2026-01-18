---
layout: base
title: Home
---
<section class="hero">
  <div class="container">
    <div class="hero-content">
      <h1>Master Strategy Gaming</h1>
      <p>Level up your gameplay with expert-crafted courses. From beginner fundamentals to advanced tactics that will give you the edge.</p>
      <a href="/courses/" class="btn btn-primary">Browse Courses</a>
    </div>
  </div>
</section>

<section class="featured-courses">
  <div class="container">
    <h2>Featured Course</h2>
    <div class="course-grid">
      {% for course in site.courses %}
        {% include course-card.html course=course %}
      {% endfor %}
    </div>
  </div>
</section>

<section class="coming-soon">
  <div class="container">
    <h2>Coming Soon</h2>
    <div class="coming-soon-grid">
      <div class="coming-soon-card">
        <div class="coming-soon-icon">
          <svg width="48" height="48" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"/>
          </svg>
        </div>
        <h3>Supremacy 1914</h3>
        <p>Master the art of World War I grand strategy with comprehensive tactics and diplomatic strategies.</p>
        <span class="status-badge">In Development</span>
      </div>
      <div class="coming-soon-card">
        <div class="coming-soon-icon">
          <svg width="48" height="48" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"/>
          </svg>
        </div>
        <h3>Call of War</h3>
        <p>Dominate the World War II battlefield with advanced unit compositions and strategic planning.</p>
        <span class="status-badge">Planned</span>
      </div>
    </div>
  </div>
</section>

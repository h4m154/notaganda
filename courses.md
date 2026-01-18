---
layout: default
title: Courses
permalink: /courses/
---
<section class="page-header">
  <h1>All Courses</h1>
  <p>Comprehensive strategy guides to help you dominate your favorite games.</p>
</section>

<section class="courses-list">
  <div class="course-grid">
    {% for course in site.courses %}
      {% include course-card.html course=course %}
    {% endfor %}
  </div>
</section>

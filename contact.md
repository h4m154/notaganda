---
layout: single
title: "Contact Me"
permalink: /contact/
author_profile: false
---

<div class="contact-container">
  <div class="contact-info">
    <h2>Get in Touch</h2>
    <p>I'm always interested in hearing from viewers, fans, and potential collaborators. Feel free to reach out through any of the following methods:</p>
    
    <h3>Email</h3>
    <p><a href="mailto:your-email@example.com">your-email@example.com</a></p>
    
    <h3>Social Media</h3>
    <p>You can also reach me through direct messages on any of my social platforms:</p>
    <ul class="social-list">
      <li><a href="{{ site.social.youtube }}" target="_blank"><i class="fab fa-youtube"></i> YouTube</a></li>
      <li><a href="{{ site.social.twitter }}" target="_blank"><i class="fab fa-twitter"></i> Twitter</a></li>
      <li><a href="{{ site.social.instagram }}" target="_blank"><i class="fab fa-instagram"></i> Instagram</a></li>
      {% if site.social.twitch %}<li><a href="{{ site.social.twitch }}" target="_blank"><i class="fab fa-twitch"></i> Twitch</a></li>{% endif %}
      {% if site.social.tiktok %}<li><a href="{{ site.social.tiktok }}" target="_blank"><i class="fab fa-tiktok"></i> TikTok</a></li>{% endif %}
    </ul>
  </div>
  
  <div class="contact-form">
    <h2>Contact Form</h2>
    <p>Alternatively, fill out this form and I'll get back to you as soon as possible:</p>
    
    <form action="https://formspree.io/f/your-formspree-id" method="POST">
      <div class="form-group">
        <label for="name">Name</label>
        <input type="text" id="name" name="name" required>
      </div>
      
      <div class="form-group">
        <label for="email">Email</label>
        <input type="email" id="email" name="_replyto" required>
      </div>
      
      <div class="form-group">
        <label for="subject">Subject</label>
        <input type="text" id="subject" name="subject" required>
      </div>
      
      <div class="form-group">
        <label for="message">Message</label>
        <textarea id="message" name="message" rows="5" required></textarea>
      </div>
      
      <button type="submit" class="btn btn-hero">Send Message</button>
    </form>
  </div>
</div>

<style>
  .contact-container {
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    margin-bottom: 2rem;
  }
  
  .contact-info, .contact-form {
    flex: 1 1 400px;
  }
  
  .social-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }
  
  .social-list li {
    margin-bottom: 0.5rem;
  }
  
  .social-list a {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
  }
  
  .form-group {
    margin-bottom: 1.5rem;
  }
  
  label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: 500;
  }
  
  input, textarea {
    width: 100%;
    padding: 0.75rem;
    border: 1px solid var(--color-bg-tertiary);
    border-radius: 4px;
    background-color: var(--color-bg-primary);
    color: var(--color-text-primary);
  }
  
  input:focus, textarea:focus {
    outline: none;
    border-color: var(--color-accent-tertiary);
    box-shadow: 0 0 0 2px rgba(76, 201, 240, 0.25);
  }
</style> 
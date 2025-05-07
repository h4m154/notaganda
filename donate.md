---
layout: single
title: "Support My Work"
permalink: /donate/
author_profile: false
toc: false
classes: donate-page
---

<div class="donation-header">
  <h1>Support My Content Creation</h1>
  <p class="lead">If you enjoy my videos and would like to help me continue creating content, there are several ways you can contribute. Your support directly enables me to invest in better equipment, dedicate more time to creating, and improve the quality of content!</p>
</div>

<div class="donation-grid">
  <div class="donation-card">
    <div class="donation-icon">
      <i class="fas fa-coffee"></i>
    </div>
    <h2>Buy Me a Coffee</h2>
    <p>A quick and easy way to show your appreciation with a one-time donation. Every "coffee" helps fund new equipment, software, and time.</p>
    <a href="https://www.buymeacoffee.com/yourusername" class="btn btn-hero" target="_blank">Buy Me a Coffee</a>
  </div>
  
  <div class="donation-card">
    <div class="donation-icon">
      <i class="fab fa-patreon"></i>
    </div>
    <h2>Patreon</h2>
    <p>Become a patron for ongoing support with exclusive perks like behind-the-scenes content, early access to videos, exclusive Q&A sessions, and input on future topics.</p>
    <a href="https://www.patreon.com/yourusername" class="btn btn-hero" target="_blank">Join Patreon</a>
  </div>
  
  <div class="donation-card">
    <div class="donation-icon">
      <i class="fab fa-youtube"></i>
    </div>
    <h2>Channel Memberships</h2>
    <p>Join as a YouTube member to get custom badges next to your name, member-only emoji for comments and live chat, and access to members-only community posts.</p>
    <a href="https://www.youtube.com/channel/your-channel-id/join" class="btn btn-hero" target="_blank">Join YouTube Membership</a>
  </div>
  
  <div class="donation-card">
    <div class="donation-icon">
      <i class="far fa-heart"></i>
    </div>
    <h2>Free Support</h2>
    <p>The simplest way to support is to subscribe to my channels, like and comment on videos, and share my content with others who might enjoy it.</p>
    <div class="social-buttons">
      <a href="https://youtube.com/yourusername" class="social-button youtube" target="_blank"><i class="fab fa-youtube"></i></a>
      <a href="https://twitch.tv/yourusername" class="social-button twitch" target="_blank"><i class="fab fa-twitch"></i></a>
      <a href="https://tiktok.com/@yourusername" class="social-button tiktok" target="_blank"><i class="fab fa-tiktok"></i></a>
    </div>
  </div>
</div>

<div class="donation-message">
  <div class="message-icon">
    <i class="fas fa-heart"></i>
  </div>
  <p>Thank you for considering supporting my work. Every contribution, whether financial or just sharing my content, makes a significant difference and allows me to keep creating videos that you enjoy!</p>
</div>

<style>
  .donate-page {
    background-color: var(--color-bg-primary);
  }
  
  .donation-header {
    text-align: center;
    margin-bottom: 3rem;
    max-width: 800px;
    margin-left: auto;
    margin-right: auto;
  }
  
  .donation-header h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    background: var(--gradient-primary);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    display: inline-block;
  }
  
  .donation-header .lead {
    font-size: 1.2rem;
    color: var(--color-text-secondary);
    line-height: 1.6;
  }
  
  .donation-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 2rem;
    margin-bottom: 3rem;
  }
  
  .donation-card {
    background-color: var(--color-bg-secondary);
    border-radius: 10px;
    padding: 2rem;
    text-align: center;
    box-shadow: var(--shadow-sm);
    transition: transform var(--transition-medium), box-shadow var(--transition-medium);
    position: relative;
    overflow: hidden;
    height: 100%;
    display: flex;
    flex-direction: column;
  }
  
  .donation-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 4px;
    background: var(--gradient-primary);
    opacity: 0;
    transition: opacity var(--transition-medium);
  }
  
  .donation-card:hover {
    transform: translateY(-10px);
    box-shadow: var(--shadow-md);
  }
  
  .donation-card:hover::before {
    opacity: 1;
  }
  
  .donation-icon {
    font-size: 3rem;
    margin-bottom: 1.5rem;
    color: var(--color-accent-primary);
  }
  
  .donation-card h2 {
    margin-top: 0;
    margin-bottom: 1rem;
    font-size: 1.5rem;
  }
  
  .donation-card p {
    color: var(--color-text-secondary);
    margin-bottom: 1.5rem;
    flex-grow: 1;
  }
  
  .social-buttons {
    display: flex;
    justify-content: center;
    gap: 1rem;
  }
  
  .social-button {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 3rem;
    height: 3rem;
    border-radius: 50%;
    font-size: 1.5rem;
    transition: transform var(--transition-medium);
  }
  
  .social-button:hover {
    transform: translateY(-5px);
  }
  
  .social-button.youtube {
    background-color: #FF0000;
    color: white !important;
  }
  
  .social-button.twitch {
    background-color: #6441A4;
    color: white !important;
  }
  
  .social-button.tiktok {
    background-color: #000000;
    color: white !important;
  }
  
  .donation-message {
    background-color: var(--color-bg-secondary);
    border-radius: 10px;
    padding: 2rem;
    text-align: center;
    box-shadow: var(--shadow-sm);
    max-width: 800px;
    margin: 0 auto;
    margin-top: 3rem;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .message-icon {
    font-size: 2.5rem;
    color: var(--color-accent-primary);
    margin-bottom: 1.5rem;
    animation: pulse 2s infinite;
  }
  
  @keyframes pulse {
    0% {
      transform: scale(1);
    }
    50% {
      transform: scale(1.1);
    }
    100% {
      transform: scale(1);
    }
  }
  
  @media (max-width: 768px) {
    .donation-grid {
      grid-template-columns: 1fr;
    }
  }
</style> 
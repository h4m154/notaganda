# Notaganda

This is the GitHub repository for the [Notaganda](https://notaganda.com) website, a central hub for all my video content across multiple platforms.

## Development

This site is built with Jekyll and the Minimal Mistakes theme.

### Local Development

1. Clone this repository
2. Install dependencies: `bundle install`
3. Run the local server: `bundle exec jekyll serve`
4. View the site at http://localhost:4000

## Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the main branch.

## Custom Domain Setup

The site uses a custom domain from IONOS. The DNS settings are configured as follows:

1. A records pointing to GitHub Pages IP addresses:
   - 185.199.108.153
   - 185.199.109.153
   - 185.199.110.153
   - 185.199.111.153

2. CNAME record for www subdomain pointing to `notaganda.github.io`

## Content Management

- Posts go in the `_posts` directory
- Video data is managed in `_data/videos.yml`
- Pages are in the root directory or in `_pages` if you prefer

## Overview

This site provides:

- **Video Showcase**: Featured videos from multiple platforms (YouTube, Twitch, TikTok, etc.)
- **Blog/News**: Updates about new content and announcements
- **Platform Links**: Easy navigation to all your content platforms
- **Contact Form**: A way for viewers to get in touch
- **Support Options**: Methods for viewers to support your content creation

## Customization

### Site Configuration

Edit `_config.yml` to update:
- Site title and description
- Social media links
- Navigation structure

### Content Updates

- **Videos**: Add new videos in `_data/videos.yml`
- **Blog Posts**: Add new markdown files in `_posts/` directory
- **Pages**: Edit the markdown files in the root directory

### Styling

- Main styling is in `assets/css/custom.css`
- Additional styling overrides in `_includes/head-custom.html`

## Features

- Responsive design that works on all devices
- Dark theme with elegant color scheme
- Integration with multiple video platforms
- Blog with category and tag support
- Social media integration
- Contact form (using Formspree)
- Support/donation options

## License

This project is available as open source under the terms of the [MIT License](LICENSE). 
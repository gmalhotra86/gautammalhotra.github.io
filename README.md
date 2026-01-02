# Gautam Malhotra - Personal Website

Professional single-page resume site built with Jekyll and hosted on GitHub Pages.

## 🚀 Quick Start

### Prerequisites
- Ruby 2.7+ and Bundler installed
- Git configured
- GitHub account

### Local Development

1. **Install dependencies:**
   ```bash
   bundle install
   ```

2. **Run locally:**
   ```bash
   bundle exec jekyll serve
   ```

3. **View site:**
   Open `http://localhost:4000` in your browser

### Deployment

Site auto-deploys when you push to the `main` branch. Changes appear in ~1 minute.

## 📝 Updating Content

### Edit Resume
Edit `index.md` - all content is in markdown format.

### Add Images
- **Headshot:** Add to `assets/images/headshot.jpg` (max 200KB, 300x300px minimum)
- **Company logos:** Add to `assets/images/logos/` (40px height recommended)

### Update Config
Edit `_config.yml` for site-wide settings (email, analytics, etc.)

## 🔧 Setup Instructions

### 1. Domain Setup (Namecheap)

1. Buy `gautammalhotra.com` on [Namecheap](https://www.namecheap.com)
2. Go to Domain → Manage → Advanced DNS
3. Add these A records:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
4. Wait 24hrs for DNS propagation

### 2. GitHub Setup

1. Create repo named `gautammalhotra.github.io`
2. Push this code to the repo
3. Go to Settings → Pages
4. Source: Deploy from `main` branch
5. Custom domain: `gautammalhotra.com`
6. Enable "Enforce HTTPS"

### 3. Google Analytics Setup

1. Create account at [analytics.google.com](https://analytics.google.com)
2. Get your GA4 Measurement ID (format: `G-XXXXXXXXXX`)
3. Add to `_config.yml`: `google_analytics: G-XXXXXXXXXX`
4. Commit and push

## 📁 File Structure

```
gautammalhotra.github.io/
├── _config.yml          # Site configuration
├── _layouts/
│   └── default.html     # HTML template
├── index.md             # Resume content (EDIT THIS!)
├── assets/
│   ├── css/
│   │   └── custom.css   # Styling
│   └── images/
│       ├── headshot.jpg      # Your photo
│       └── logos/            # Company logos
├── CNAME                # Domain configuration
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```

## 🎨 Customization

### Colors
Edit CSS variables in `assets/css/custom.css`:
```css
:root {
  --navy: #1e3a8a;
  --light-gray: #f8fafc;
  --text-black: #0f172a;
}
```

### Layout
- Mobile-first responsive design
- Timeline visible on desktop (≥768px)
- Single-page scroll layout

## 📊 Success Metrics

**Target:** 10 quality inbound opportunities per month
- 3 recruiter outreach for VP/Director roles
- 7 advisory requests from VCs/executives

Track via Google Analytics + email responses.

## 🔒 Security

- HTTPS enforced by GitHub Pages
- No user input or forms
- Static site (no server vulnerabilities)

## ⚡ Performance

- Target load time: <2 seconds
- Optimize images: <200KB each
- Minimal dependencies

## 📮 Contact

- **Email:** gmalhotra86@gmail.com
- **LinkedIn:** [gautam-malhotra](https://linkedin.com/in/gautam-malhotra)

---

**Built with:** Jekyll + GitHub Pages  
**Last updated:** December 2025

# 🎉 Website Built! Next Steps to Launch

Your personal website is built and ready to deploy. Here's what to do next:

## ✅ What's Done

- Jekyll site structure created
- Resume content added (from your materials)
- Custom styling with timeline design
- Mobile-responsive layout
- Google Analytics integration (needs your ID)
- Git repo initialized with first commit

## 📋 Steps to Launch (in order)

### Step 1: Add Your Images (15-30 min)

**Headshot:**
1. Add your professional headshot to `assets/images/headshot.jpg`
2. Recommended: 300x300px minimum, <200KB
3. Use a professional photo with good lighting

**Company Logos:**
Add to `assets/images/logos/`:
- `adobe.png`
- `faire.png`
- `intuit.png`
- `accenture.png`
- `baml.png`

**Where to get logos:**
- Company press kits (Google "[Company] press kit")
- Brandfetch.com
- Company websites

### Step 2: Buy Domain (5 min)

1. Go to [Namecheap.com](https://www.namecheap.com)
2. Search for `gautammalhotra.com`
3. Purchase (~$10/year)
4. **Don't configure DNS yet** - we'll do that in Step 5

### Step 3: Create GitHub Repo (2 min)

1. Go to [github.com](https://github.com)
2. Click "New repository"
3. Name it **exactly:** `gautammalhotra.github.io`
4. Make it **Public**
5. **Don't** add README, .gitignore, or license (we already have them)
6. Click "Create repository"

### Step 4: Push Code to GitHub (2 min)

In your terminal, from the website directory:

```bash
cd /Users/gautamm/personal-os/gautammalhotra.github.io

# Add the GitHub remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/gautammalhotra.github.io.git

# Push the code
git branch -M main
git push -u origin main
```

### Step 5: Configure GitHub Pages (5 min)

1. In your GitHub repo, go to **Settings → Pages**
2. Under "Source": Select **Deploy from a branch**
3. Branch: Select **main** and **/ (root)**
4. Click **Save**
5. Under "Custom domain": Enter `gautammalhotra.com`
6. Click **Save** (don't check "Enforce HTTPS" yet)
7. Wait ~1 minute for GitHub to generate SSL certificate
8. Then check **"Enforce HTTPS"**

### Step 6: Point Domain to GitHub (10 min)

1. Go to Namecheap → Domain List → Manage `gautammalhotra.com`
2. Click **Advanced DNS**
3. Delete existing records
4. Add these **A Records** (Host: `@`, Value:):
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
5. Add **CNAME Record**:
   - Host: `www`
   - Value: `gautammalhotra.github.io`
6. Save changes

**⏰ Wait 2-24 hours for DNS propagation**

### Step 7: Set Up Google Analytics (10 min)

1. Go to [analytics.google.com](https://analytics.google.com)
2. Create account → New property
3. Property name: "Gautam Malhotra Website"
4. Choose "Web" stream
5. Copy your Measurement ID (format: `G-XXXXXXXXXX`)
6. Edit `_config.yml` and add:
   ```yaml
   google_analytics: G-XXXXXXXXXX
   ```
7. Commit and push:
   ```bash
   git add _config.yml
   git commit -m "Add Google Analytics"
   git push
   ```

## 🎯 Testing Checklist

After DNS propagates, test:

- [ ] Visit `https://gautammalhotra.com` - site loads
- [ ] Check mobile view (use phone or Chrome DevTools)
- [ ] Click email link - opens mail client
- [ ] Click LinkedIn link - goes to profile
- [ ] All images load correctly
- [ ] Timeline appears on desktop, hidden on mobile
- [ ] Google Analytics fires (check Real-time report)

## 🔄 How to Update Content

Whenever you want to update your resume:

1. Edit `index.md` in your preferred text editor
2. Commit and push:
   ```bash
   git add index.md
   git commit -m "Update experience section"
   git push
   ```
3. Site updates automatically in ~1 minute

## ⚡ Quick Commands Reference

```bash
# Navigate to site directory
cd /Users/gautamm/personal-os/gautammalhotra.github.io

# Test locally (requires Jekyll installed)
bundle install
bundle exec jekyll serve
# Then visit http://localhost:4000

# Update and deploy
git add .
git commit -m "Your change description"
git push

# Check git status
git status

# View commit history
git log --oneline
```

## 🆘 Troubleshooting

**Site not loading after 24hrs:**
- Check DNS settings in Namecheap match Step 6
- Run `dig gautammalhotra.com` to check DNS propagation
- Ensure CNAME file exists with `gautammalhotra.com`

**Images not showing:**
- Check file names match exactly (case-sensitive)
- Verify images are in correct folders
- Compress images if >200KB each

**Changes not appearing:**
- Check GitHub Actions tab - build should be successful
- Hard refresh browser (Cmd+Shift+R on Mac, Ctrl+Shift+R on Windows)
- Wait 2-3 minutes after pushing

## 💰 Costs

- **Domain:** ~$10/year (Namecheap)
- **Hosting:** FREE (GitHub Pages)
- **Analytics:** FREE (Google Analytics)
- **Total:** $10/year

## 📈 Success Metrics

**6-month target:**
- 10 quality inbound opportunities per month
  - 3 recruiter outreach for VP/Director roles
  - 7 advisory requests from VCs/executives

Track via Google Analytics + email responses.

## 🎉 You're Done!

Once DNS propagates and you've tested everything, you're live!

**Share your site:**
- Add to LinkedIn profile
- Include in email signature
- Share at conferences and networking events
- Use in warm intro follow-ups

---

**Questions?** Re-read the main README.md or reach out for help.

**Good luck! 🚀**

# GitHub Pages Deployment Guide

## Quick Setup

### Method 1: Using GitHub CLI (Recommended)
```bash
cd trudaism
gh repo create trudaism.github.io --public --remote=origin --push --description "Truth as Sacred - Official Trudaism Philosophy Site"
git push -u origin main
```

### Method 2: Manual Setup
1. Go to github.com/new
2. Repository name: `trudaism.github.io`
3. Make it public
4. Add files via upload or:
   ```bash
   git remote add origin https://github.com/YOURUSERNAME/trudaism.github.io.git
   git push -u origin main
   ```

### Method 3: Fork & Deploy
1. Fork this repository
2. Go to Settings → Pages
3. Select "Deploy from branch" → Source: main branch

## Post-Deployment
- **Live site**: `https://YOURUSERNAME.github.io/trudaism.github.io`
- **Updates**: Push to main → auto-deploy via GitHub Actions
- **Custom domain**: Add CNAME file for your own domain

## File Structure
```
site/
├── index.html           # Landing page
├── foundations.html     # Complete philosophy
├── practice.html        # Daily implementation
├── community.html       # Links and connections
├── style.css           # Dark theme + responsive
└── README.md           # This file
```
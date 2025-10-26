# Quick Deployment Guide

## 🚀 Fastest Way to Deploy

### 1. Netlify (Recommended - Easiest)
1. Go to https://app.netlify.com/drop
2. Drag the entire `static-site` folder
3. Done! Your site is live in seconds

### 2. Vercel
```bash
cd static-site
npx vercel
```

### 3. GitHub Pages
1. Create a new repository
2. Upload all files from `static-site` to the repository
3. Go to Settings > Pages
4. Select source: Deploy from a branch
5. Branch: main, folder: / (root)
6. Your site is live!

### 4. Surge.sh (CLI)
```bash
npm install -g surge
cd static-site
surge
```

## 📦 Option A: Direct Upload
Simply upload the entire `static-site` folder to your hosting provider via FTP, cPanel file manager, or AWS S3.

## 📦 Option B: Using Git
```bash
cd static-site
git init
git add .
git commit -m "Initial commit"
git remote add origin <your-repo-url>
git push -u origin main
```

## 🔧 For Different Hosting Providers

### AWS Amplify
1. Connect your GitHub repository
2. Use build command: (leave blank)
3. Use output directory: `static-site`

### Azure Static Web Apps
```bash
cd static-site
az staticwebapp deploy --name amt-site --resource-group <your-rg>
```

### Cloudflare Pages
1. Connect GitHub/GitLab
2. Build command: (none)
3. Publish directory: `static-site`

### Firebase
```bash
cd static-site
firebase init hosting
firebase deploy
```

## ✅ Pre-Deployment Checklist
- [ ] Update contact information (phone, email, address)
- [ ] Replace placeholder images with actual product images
- [ ] Replace client logo placeholders
- [ ] Update social media links
- [ ] Test all navigation links
- [ ] Test on mobile devices
- [ ] Verify form functionality (add backend if needed)

## 🎯 Post-Deployment
- Update DNS if using custom domain
- Enable HTTPS/SSL certificate
- Test contact form
- Monitor analytics
- Set up redirects if needed


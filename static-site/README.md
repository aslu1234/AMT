# AMT - Amigos Technology Static Website

This is a static version of the AMT (Amigos Technology) website, ready for deployment to any static hosting service.

## 📁 Directory Structure

```
static-site/
├── index.html          # Main landing page
├── css/                # Custom styles
├── js/                 # JavaScript files
├── lib/                # Bootstrap and other libraries
└── favicon.ico         # Site icon
```

## 🚀 Deployment Options

### Option 1: GitHub Pages
1. Push this `static-site` folder to a GitHub repository
2. Go to Settings > Pages
3. Select the branch and `/ (root)` directory
4. Your site will be live at `https://yourusername.github.io/repo-name`

### Option 2: Netlify
1. Sign up at https://www.netlify.com
2. Drag and drop the `static-site` folder
3. Your site will be deployed instantly

### Option 3: Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Navigate to the `static-site` folder
3. Run: `vercel`
4. Follow the prompts

### Option 4: AWS S3 + CloudFront
1. Create an S3 bucket
2. Upload all files from `static-site` to the bucket
3. Enable static website hosting
4. (Optional) Set up CloudFront distribution for CDN

### Option 5: Azure Static Web Apps
1. Install Azure CLI
2. Run: `az staticwebapp deploy --name amt-site --source static-site`
3. Follow authentication prompts

### Option 6: Firebase Hosting
1. Install Firebase CLI: `npm install -g firebase-tools`
2. Run: `firebase login`
3. Run: `firebase init hosting`
4. Deploy: `firebase deploy`

### Option 7: Traditional Web Hosting (cPanel, FTP, etc.)
1. Upload all files from `static-site` to your hosting's public_html directory
2. Ensure the main file is named `index.html`
3. Your site will be accessible via your domain

## 🧪 Local Testing

Before deploying, test the site locally:

### Using Python (recommended)
```bash
cd static-site
python -m http.server 8000
```
Then open http://localhost:8000 in your browser

### Using Node.js
```bash
cd static-site
npx http-server
```

### Using VS Code
Install the "Live Server" extension and right-click on `index.html` > "Open with Live Server"

## 📝 Features

- **Responsive Design**: Works on all devices (desktop, tablet, mobile)
- **Modern UI**: Dark theme with elegant styling
- **Bootstrap 5**: Latest Bootstrap framework for responsive layouts
- **Bootstrap Icons**: Beautiful icon set for better visual presentation
- **Smooth Scrolling**: Enhanced navigation experience
- **Contact Form**: Static contact form (no backend required for display)

## ⚠️ Important Notes

- The contact form is static and requires a backend service to actually send emails
- Replace placeholder images and client logos with actual content
- Update contact information (phone, email, address) as needed
- All external links (social media, product links) are currently placeholders

## 🛠️ Customization

### To Update Colors
Edit the CSS variables in the `<style>` section of `index.html`:
```css
:root {
    --color-primary-dark: #0a192f;
    --color-accent: #64ffda;
    /* ... etc */
}
```

### To Add Real Images
Replace placeholder URLs like:
```html
<img src="https://via.placeholder.com/400x200/...">
```
with actual image paths:
```html
<img src="images/smart-scale.jpg">
```

### To Update Content
Simply edit the HTML directly in `index.html` - no build process required!

## 📄 License

© 2025 AMT - Amigos Technology. All rights reserved.


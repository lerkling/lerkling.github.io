# Platform Link Website

Professional website for Platform Link - Strategic advisory for vertical SaaS and AI companies.

## Overview

This is a static website built with HTML, CSS, and vanilla JavaScript, designed to be hosted on GitHub Pages. The site features a professional but approachable design that reflects Platform Link's brand as a trusted operator-advisor.

## Project Structure

```
platformlink-website/
├── index.html          # Homepage
├── about.html          # About page
├── css/
│   └── styles.css     # All styles including responsive design
├── images/            # Images and assets (add your logo here)
├── js/                # JavaScript files (currently unused)
├── .gitignore         # Git ignore file
└── README.md          # This file
```

## Features

- **Responsive Design**: Mobile-first approach that works on all devices
- **Professional Branding**: Navy blue (#1a365d) and coral (#ff6b6b) color scheme
- **Fast Loading**: No heavy frameworks, optimized for performance
- **SEO-Friendly**: Semantic HTML with proper meta tags
- **Easy to Maintain**: Clean, well-documented code

## Deployment to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and log in with username: `lerkling`
2. Click the "+" icon in the top right and select "New repository"
3. Name your repository:
   - For user site: `lerkling.github.io` (will be available at https://lerkling.github.io)
   - For project site: `platformlink-website` (will be available at https://lerkling.github.io/platformlink-website)
4. Set visibility to "Public"
5. Do NOT initialize with README, .gitignore, or license (we already have these)
6. Click "Create repository"

### Step 2: Push Your Code to GitHub

```bash
# Navigate to your project directory
cd /Users/lerk-ling.chang/Desktop/platformlink-website

# Add all files to git
git add .

# Create your first commit
git commit -m "Initial commit: Platform Link website"

# Add your GitHub repository as remote
# For user site:
git remote add origin https://github.com/lerkling/lerkling.github.io.git

# OR for project site:
# git remote add origin https://github.com/lerkling/platformlink-website.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" in the repository menu
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click "Save"
6. Wait a few minutes for GitHub to build your site
7. Your site will be available at:
   - User site: `https://lerkling.github.io`
   - Project site: `https://lerkling.github.io/platformlink-website`

### Step 4: Configure Custom Domain (Optional)

To use your custom domain (platformlink.io):

1. In your repository settings under "Pages", find "Custom domain"
2. Enter: `www.platformlink.io`
3. Click "Save"
4. In your domain registrar (where you bought platformlink.io), add these DNS records:
   - Type: `CNAME`, Name: `www`, Value: `lerkling.github.io`
   - Type: `A`, Name: `@`, Value: `185.199.108.153`
   - Type: `A`, Name: `@`, Value: `185.199.109.153`
   - Type: `A`, Name: `@`, Value: `185.199.110.153`
   - Type: `A`, Name: `@`, Value: `185.199.111.153`
5. Wait for DNS propagation (can take up to 24 hours)
6. Enable "Enforce HTTPS" in GitHub Pages settings once DNS is configured

## Making Updates

### Update Content

1. Edit the HTML files (`index.html`, `about.html`) with your changes
2. Save the files
3. Commit and push:
   ```bash
   git add .
   git commit -m "Update content"
   git push
   ```
4. Changes will be live in a few minutes

### Update Styling

1. Edit `css/styles.css`
2. Save the file
3. Commit and push (same as above)

### Add Images/Logo

1. Add your image files to the `images/` folder
2. Update the HTML to reference them:
   ```html
   <img src="images/your-logo.png" alt="Platform Link Logo">
   ```
3. Commit and push

## Customization Guide

### Colors

Edit the CSS variables in `css/styles.css`:

```css
:root {
    --primary-navy: #1a365d;      /* Main brand color */
    --accent-coral: #ff6b6b;      /* Accent/CTA color */
    --text-dark: #1a202c;         /* Main text */
    --text-gray: #4a5568;         /* Secondary text */
}
```

### Content

- **Homepage**: Edit `index.html`
  - Hero section: Lines 28-35
  - Services: Lines 52-77
  - Differentiator: Lines 82-107

- **About Page**: Edit `about.html`
  - Replace placeholder content with your actual background and experience

### Logo

Replace the text-based logo with your actual logo:

1. Add logo file to `images/` folder
2. In both HTML files, replace:
   ```html
   <div class="logo">PLATFORM LINK</div>
   ```
   with:
   ```html
   <div class="logo"><img src="images/logo.png" alt="Platform Link"></div>
   ```

## Local Development

To preview your site locally:

1. Open `index.html` directly in your web browser, or
2. Use a local server:
   ```bash
   # With Python 3
   python3 -m http.server 8000

   # Then visit http://localhost:8000 in your browser
   ```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Contact

For questions or support, contact: contact@platformlink.io

## License

© 2024 Platform Link. All rights reserved.

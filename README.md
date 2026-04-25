# Naar Nederland - Dutch Learning App

A mobile-responsive web application for learning Dutch vocabulary with flashcards, search, and practice modes.

## Features

- **15-Day Learning Plan**: Structured curriculum from Les 21-65
- **Interactive Flashcards**: Flip cards for practice mode
- **Smart Search**: Search in both Dutch and Turkish
- **Voice Pronunciation**: Text-to-speech for Dutch words
- **Mobile Optimized**: Perfect for phone/tablet usage
- **Progress Tracking**: Visual progress indicators

## Deployment to Cloudflare Pages

### Step 1: Create GitHub Repository
1. Go to [GitHub](https://github.com) and create a new repository
2. Name it: `naar-nederland-app`
3. Keep it public or private (your choice)
4. Don't initialize with README (we already have one)

### Step 2: Push to GitHub
```bash
# Add your GitHub repository as remote (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/naar-nederland-app.git
git branch -M main
git push -u origin main
```

### Step 3: Deploy to Cloudflare Pages
1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com)
2. Navigate to **Pages** section
3. Click **"Create a project"**
4. Choose **"Connect to Git"**
5. Select GitHub and authorize if needed
6. Choose your `naar-nederland-app` repository
7. **Build Settings**:
   - **Framework preset**: None
   - **Build command**: Leave empty
   - **Build output directory**: Leave empty (root)
8. Click **"Save and Deploy"**

### Step 4: Get Your URL
After deployment, Cloudflare will give you:
- **Preview URL**: For testing
- **Production URL**: Your live site (usually `your-project.pages.dev`)

## Custom Domain (Optional)
1. In Cloudflare Pages project settings
2. Go to **"Custom domains"**
3. Add your domain (e.g., `naar-nederland.com`)
4. Update DNS records as instructed

## Project Structure
```
leren/
├── index.html          # Main application file
└── README.md          # This file
```

## Technologies Used
- **HTML5** with semantic markup
- **Tailwind CSS** via CDN for styling
- **Font Awesome** for icons
- **Vanilla JavaScript** for functionality
- **Web Speech API** for pronunciation

## Notes
- No build process required - static HTML file
- All dependencies loaded via CDN
- Fully responsive design
- Works offline once loaded

# InvestWise Deployment Guide

## Quick Deploy to Vercel

### Option 1: Deploy via GitHub (Recommended)

#### Step 1: Create GitHub Repository

1. Go to [https://github.com](https://github.com) and log in
2. Click the **+** icon → **New repository**
3. Name it `investwise`
4. Select **Public**
5. Click **Create repository**

#### Step 2: Push Code to GitHub

Run these commands in your terminal:

```bash
cd investwise
git remote add origin https://github.com/anxuanqi690/investwise.git
git push -u origin main
```

#### Step 3: Deploy on Vercel

1. Go to [https://vercel.com](https://vercel.com)
2. Click **Add New** → **Project**
3. Import your `investwise` repository from GitHub
4. Click **Deploy**
5. Your site will be live at: `https://investwise.vercel.app`

### Option 2: Deploy Directly (No GitHub)

1. Download the `investwise` folder
2. Go to [https://vercel.com](https://vercel.com)
3. Click **Add New** → **Project**
4. Click **Import Third-Party** → **Import Git Repository**
5. Or drag and drop the folder
6. Deploy!

### Option 3: Deploy via CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Navigate to project
cd investwise

# Login to Vercel
vercel login

# Deploy
vercel

# Deploy to production
vercel --prod
```

## Post-Deployment Setup

### 1. Update Domain (Optional)

After deploying, you can add a custom domain:
1. Go to Vercel Dashboard → Your Project → **Settings**
2. Click **Domains**
3. Add your custom domain (e.g., `investwise.com`)
4. Update DNS records as instructed

### 2. Update sitemap.xml URLs

Replace `https://investwise.vercel.app` with your actual domain in:
- `sitemap.xml`
- `robots.txt` (Sitemap directive)

### 3. Enable HTTPS

Vercel automatically provides SSL certificates. No action needed.

## AdSense Integration (For Revenue)

To monetize with Google AdSense:

1. Apply for [AdSense](https://www.google.com/adsense)
2. Once approved, add your AdSense code to each page
3. Place ad units strategically (sidebar, in-content, footer)
4. Monitor performance and optimize placement

### AdSense Approval Tips for Finance Sites:
- Ensure comprehensive disclaimer page
- Add clear privacy policy
- Include contact information
- Publish original, valuable content (you have 12+ articles!)
- Wait for indexing before applying (2-4 weeks)

## Troubleshooting

### Deployment Failed
- Check that all files are committed
- Verify `vercel.json` configuration
- Check build logs in Vercel dashboard

### 404 on Pages
- Ensure file paths are correct
- Check that `index.html` is in root directory

### CSS/JS Not Loading
- Verify `css/style.css` path in HTML
- Clear browser cache
- Check browser console for errors

## Project Structure

```
investwise/
├── index.html              # Homepage
├── about.html              # About page
├── contact.html            # Contact page
├── disclaimer.html         # Investment disclaimer
├── privacy.html           # Privacy policy
├── terms.html             # Terms of service
├── css/
│   └── style.css          # Custom styles
├── articles/              # Article pages (12 total)
│   ├── stock-market-basics.html
│   ├── how-to-read-candlestick.html
│   ├── dividend-investing-guide.html
│   ├── technical-analysis-101.html
│   ├── fundamental-analysis.html
│   ├── risk-management.html
│   ├── etf-investing-guide.html
│   ├── stock-screening-guide.html
│   ├── market-orders-explained.html
│   ├── portfolio-diversification.html
│   ├── value-investing.html
│   └── growth-stocks-guide.html
├── sitemap.xml            # XML sitemap
├── robots.txt             # Robots directive
├── package.json           # npm config
├── vercel.json            # Vercel config
└── README.md              # Project documentation
```

## AdSense CPC Optimization Tips

Finance content typically earns $2-5 per click. To maximize:

1. **Target high CPC keywords**: investing, stock trading, forex, crypto
2. **Create long-form content**: 1500+ words per article (done!)
3. **Internal linking**: Connect related articles (done!)
4. **Mobile optimization**: Ensure responsive design (done!)
5. **Page speed**: Static HTML is already optimized
6. **Strategic ad placement**: Above fold, in-content, sidebar

---

*Last Updated: 2025*

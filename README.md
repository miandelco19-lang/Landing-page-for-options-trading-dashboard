# Options Trading Dashboard Landing Page

A high-converting landing page for an AI-powered options strategy scanner built for retail traders.

## What's Included

* `landing.html` - Main landing page (ready to deploy)
* `.gitignore` - Git configuration
* `README.md` - This file

## Features

✨ **Converting Landing Page**

* Hero section with clear value prop
* Feature cards explaining benefits
* Social proof (user testimonials \& stats)
* Email signup form
* Mobile responsive design
* Fast loading (single HTML file)

## Quick Start

### Deploy to Vercel (Recommended - 2 minutes)

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Click "Add New" → "Project"
4. Select this GitHub repo
5. Click "Deploy"
6. Your site is live! 🎉

### Deploy to Netlify

1. Push this repo to GitHub
2. Go to [netlify.com](https://netlify.com)
3. Click "Add new site" → "Import an existing project"
4. Select GitHub \& your repo
5. Deploy!

### Local Testing

Simply open `landing.html` in your browser to test locally.

## File Structure

```
├── landing.html          # Main landing page
├── README.md             # This file
└── .gitignore            # Files to ignore in git
```

## Customization

Edit `landing.html` to:

* Change the title and meta description (in the `<head>`)
* Update the app name (search for "Options Scanner")
* Add your actual app screenshot (replace the demo placeholder)
* Update testimonials with real user quotes
* Add your email collection endpoint

## Email Signup

Currently the form shows a popup. To collect emails:

### Option A: Airtable

1. Create Airtable base with "Email" field
2. Get your API key
3. Update the JavaScript form handler

### Option B: Google Forms

1. Create Google Form
2. Point the form to Google Forms action URL

### Option C: Your Backend

Point the form to your own API endpoint that saves emails.

## Next Steps

1. **Deploy to Vercel** → Get a live URL
2. **Set up email collection** → Start capturing signups
3. **Customize content** → Add your screenshots and testimonials
4. **Add analytics** → Track visitors
5. **Promote it** → Share on Reddit, Twitter, Discord

## Analytics

Add Google Analytics by inserting this in the `<head>`:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA\_ID"></script>
<script>
  window.dataLayer = window.dataLayer || \[];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA\_ID');
</script>
```

Replace `GA\_ID` with your Google Analytics tracking ID.

## Support

Questions? Issues? Feel free to reach out!

\---

Built with ❤️ for retail options traders


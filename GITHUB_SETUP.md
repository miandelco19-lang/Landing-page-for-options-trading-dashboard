# GitHub Setup Guide - Step by Step

Follow these steps to create your GitHub repository and push your code.

## Prerequisites

- GitHub account (free at github.com)
- Git installed on your computer (github.com/git-guides/install-git)
- Your landing page files ready

## Step 1: Create GitHub Repository

1. **Go to GitHub**
   - Visit https://github.com
   - Sign in to your account

2. **Create a new repository**
   - Click the "+" icon in top right
   - Select "New repository"
   - Or go directly to: https://github.com/new

3. **Fill in repository details**
   ```
   Repository name: options-trading-dashboard
   Description: Landing page for options strategy finder
   Public: ✓ (yes, public)
   Initialize with README: ✗ (no, we have our own)
   ```

4. **Click "Create repository"**
   - You'll see instructions on next screen
   - Copy the repository URL (looks like: `https://github.com/YOUR_USERNAME/options-trading-dashboard.git`)

---

## Step 2: Set Up Locally (Using Command Line)

**Open Terminal/Command Prompt and run these commands:**

```bash
# Navigate to your project folder
cd path/to/your/project

# Initialize git
git init

# Add your files to git
git add .

# Create first commit
git commit -m "Initial commit: landing page"

# Connect to GitHub repository (replace YOUR_REPO_URL)
git remote add origin https://github.com/YOUR_USERNAME/options-trading-dashboard.git

# Push to GitHub (this sends your files to GitHub)
git branch -M main
git push -u origin main
```

**That's it!** Your code is now on GitHub.

---

## Step 3: Verify on GitHub

1. Go to your repository URL
2. Refresh the page
3. You should see:
   - `landing.html`
   - `README.md`
   - `.gitignore`

All files uploaded successfully! ✓

---

## Step 4: Deploy to Vercel

Now that your code is on GitHub, deploying to Vercel is super easy:

1. **Go to Vercel**
   - Visit https://vercel.com
   - Click "Sign Up"
   - Select "Continue with GitHub"
   - Authorize Vercel

2. **Create a new project**
   - Click "Add New" → "Project"
   - Select your GitHub account
   - Search for "options-trading-dashboard"
   - Click "Import"

3. **Configure (optional)**
   - Framework: None (it's just HTML)
   - Root Directory: ./
   - Environment variables: (leave blank for now)

4. **Deploy**
   - Click "Deploy"
   - Wait 30 seconds...
   - Your site is LIVE! 🎉

5. **Get your live URL**
   - Vercel shows your new domain
   - Usually something like: `options-trading-dashboard.vercel.app`
   - Share this link everywhere!

---

## Step 5: Update Your Landing Page (Later)

When you want to make changes:

```bash
# Make edits to landing.html

# Check what changed
git status

# Add changes
git add .

# Commit with a message
git commit -m "Update landing page content"

# Push to GitHub
git push

# Vercel automatically deploys! (within 1 minute)
```

---

## Step 6: Set Up Custom Domain (Optional)

If you have a domain (like `optionscanner.com`):

1. In Vercel dashboard, go to your project
2. Click "Settings" → "Domains"
3. Add your domain
4. Follow instructions to update DNS settings
5. Wait 24 hours for it to propagate

---

## Troubleshooting

### "Permission denied" error?
```bash
# Generate SSH key instead of HTTPS
git remote set-url origin git@github.com:YOUR_USERNAME/options-trading-dashboard.git
```

### "Git not found" error?
- You need to install Git first
- Download from: https://git-scm.com/download

### Want a simpler way (No Command Line)?

Use **GitHub Desktop** (GUI instead of terminal):
1. Download GitHub Desktop: https://desktop.github.com
2. Sign in with GitHub account
3. Click "Create a New Repository"
4. Drag and drop your files into the folder
5. Commit and publish
6. Then deploy to Vercel as normal

---

## Next: Collect Emails

Once your site is live, you need to collect signups. Choose one:

### Option A: Airtable (Recommended)
- Free tier is generous
- Easy to set up
- Can see all signups in spreadsheet
- Takes 10 minutes

### Option B: Google Forms (Easiest)
- Total free
- Responses in Google Sheets
- Takes 5 minutes

### Option C: Your Backend (Later)
- When you build your backend, collect directly

---

## Questions?

Need help with any step? 
- GitHub docs: https://docs.github.com
- Vercel docs: https://vercel.com/docs
- Git cheat sheet: https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf

Good luck! 🚀

# GitHub Pages Deployment Guide for CSV Plumbing

## Step 1: Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon in the top right and select "New repository"
3. Name it: `csvplumbing.github.io` (this is important for GitHub Pages)
4. Add a description: "CSV Plumbing website"
5. Choose "Public" (required for free GitHub Pages)
6. Click "Create repository"

## Step 2: Push Your Files to GitHub

Using command line (Terminal/Command Prompt):

```bash
# Navigate to your project folder
cd "/Users/justin/Dev/CSV Plumbing"

# Initialize git
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial CSV Plumbing website"

# Add remote repository
git remote add origin https://github.com/YOUR_USERNAME/csvplumbing.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (gear icon)
3. Click **Pages** in the left sidebar
4. Under "Build and deployment", make sure:
   - Source is set to "Deploy from a branch"
   - Branch is set to "main" or "master"
5. Click **Save**

Your site will be live at: `https://YOUR_USERNAME.github.io`

## Step 4 (Optional): Use a Custom Domain

### If you have a custom domain (e.g., csvplumbing.com.au):

1. **In your repository:**
   - Create a file named `CNAME` (no extension)
   - Add your domain: `csvplumbing.com.au`
   - Push to GitHub

2. **With your domain registrar:**
   - Add an A record pointing to GitHub's IP: `185.199.108.153`
   - Or add a CNAME record pointing to: `YOUR_USERNAME.github.io`

## Step 5: Enable the Contact Form

1. Go to [formspree.io](https://formspree.io)
2. Sign up for a free account
3. Create a new form
4. You'll get a Form ID (looks like: `mnopqrst`)
5. Edit `index.html` and replace `YOUR_FORM_ID` with this ID:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
6. Push the change to GitHub

## Making Updates

After setup, updating the website is easy:

```bash
# Make your changes to the files
# Then:
git add .
git commit -m "Describe your changes"
git push
```

Your changes will be live in about 30 seconds to 1 minute.

## Troubleshooting

**Site not showing up?**
- Wait 5-10 minutes for GitHub to build and deploy
- Check that repository is public
- Verify branch is "main" in Pages settings

**Contact form not working?**
- Make sure you have the correct Form ID from Formspree
- Check the form action URL in index.html
- Test by submitting the form

**Custom domain not working?**
- Verify DNS records are pointing correctly
- Can take 24-48 hours to propagate
- Check GitHub Pages settings shows your custom domain

## Questions?

Contact Chris at: chris@csvplumbing.com or 0450 207 705

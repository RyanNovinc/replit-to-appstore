# App Course Landing Page

## Deploying to GitHub Pages

### Step 1: Create a GitHub Repository
1. Go to [github.com](https://github.com) and log in
2. Click the "+" icon in the top right and select "New repository"
3. Name your repository (e.g., `app-course-landing`)
4. Make it **Public**
5. **Do NOT** initialize with README
6. Click "Create repository"

### Step 2: Upload Your Files
After creating the repo, you'll see a page with instructions. Follow these steps:

**Option A: Upload via GitHub Website (Easiest)**
1. On your new repository page, click "uploading an existing file"
2. Drag and drop ALL files from this folder:
   - `index.html`
   - `images/` folder (with ryan.jpg inside)
   - This `README.md` (optional)
3. Scroll down and click "Commit changes"

**Option B: Using Git Command Line**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click "Settings" tab
3. Click "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"
6. Wait 1-2 minutes for deployment

### Step 4: Access Your Site
Your site will be available at:
```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

For example: `https://ryan-codes.github.io/app-course-landing/`

## File Structure
```
.
├── index.html          # Main landing page
├── images/
│   └── ryan.jpg       # Your profile photo
└── README.md          # This file
```

## Important Notes

- The image path is set to `images/ryan.jpg` - make sure this folder structure is maintained
- All files must be in the root of your repository
- Changes can take 1-2 minutes to appear after pushing
- The site uses a dark theme with cyan accents
- Mobile responsive design included

## Making Updates

After initial setup, to update your site:
1. Edit files locally or on GitHub directly
2. Commit changes
3. Push to main branch (or save on GitHub)
4. Wait 1-2 minutes for deployment

## Custom Domain (Optional)

If you want to use your own domain:
1. Buy a domain from Namecheap, Google Domains, etc.
2. In GitHub repo Settings > Pages, add your custom domain
3. Update your domain's DNS settings with your provider
4. Add CNAME record pointing to `YOUR-USERNAME.github.io`

## Troubleshooting

**Image not showing?**
- Check that `images/ryan.jpg` exists in your repository
- Verify the path is exactly `images/ryan.jpg` (case-sensitive)
- Clear browser cache and refresh

**Changes not appearing?**
- Wait 2-3 minutes after pushing
- Hard refresh browser (Ctrl+Shift+R or Cmd+Shift+R)
- Check GitHub Actions tab for deployment status

**404 Error?**
- Make sure GitHub Pages is enabled in Settings
- Verify you're using the correct URL format
- Check that index.html is in the repository root

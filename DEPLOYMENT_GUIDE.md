# GitHub Pages Deployment Guide for Gaurav's Portfolio

## Step-by-Step Guide to Deploy Your Portfolio

### Prerequisites
- GitHub account (free at https://github.com)
- Git installed on your computer
- All portfolio files ready

### Method 1: Using GitHub Pages with a New Repository (Recommended)

#### Step 1: Create a New GitHub Repository

1. Log in to your GitHub account
2. Click the **+** icon in the top right corner
3. Select **New repository**
4. Name it: `yourusername.github.io`
   - Replace `yourusername` with your actual GitHub username
   - Example: `imgauravs.github.io`
5. Add description: "Data Engineer Portfolio"
6. Keep it **Public** (required for GitHub Pages)
7. Click **Create repository**

#### Step 2: Prepare Files on Your Computer

1. Create a folder on your computer: `gaurav-portfolio`
2. Place these files in the folder:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `README.md`
   - `.gitignore`
   - `_config.yml`

#### Step 3: Initialize Git Repository Locally

Open PowerShell or Terminal in your portfolio folder and run:

```powershell
# Initialize Git repository
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial portfolio website commit"

# Add remote connection to GitHub
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

#### Step 4: Verify Deployment

1. Go to your repository on GitHub
2. Navigate to **Settings** > **Pages**
3. Under "Source", select **Deploy from a branch**
4. Branch: **main**
5. Folder: **/root**
6. Click **Save**

#### Step 5: Access Your Live Portfolio

- Your site will be live at: `https://yourusername.github.io`
- It may take 1-5 minutes for GitHub to build and deploy
- Refresh the page after a few minutes

---

### Method 2: Using gh-pages Branch (Alternative)

1. Follow steps 1 and 2 above
2. Instead of `main` branch, create a `gh-pages` branch:

```powershell
git checkout -b gh-pages
git push -u origin gh-pages
```

3. In GitHub Settings > Pages, select `gh-pages` branch
4. Your site will be available at the same URL

---

## Updating Your Portfolio

Whenever you want to update your portfolio:

```powershell
# Navigate to your portfolio folder
cd path\to\gaurav-portfolio

# Make your changes to files

# Stage all changes
git add .

# Commit with a message
git commit -m "Update project descriptions"

# Push to GitHub
git push origin main
```

Changes will be live within a few minutes.

---

## Domain Setup (Optional)

### Using a Custom Domain

1. **Register a domain** (e.g., gauravshukla.dev)
2. In GitHub repository:
   - Go to **Settings** > **Pages**
   - Under "Custom domain", enter your domain
   - Click **Save**
3. Create a `CNAME` file in your repository root with:
   ```
   yourdomain.com
   ```
4. Configure DNS at your domain registrar:
   - Add A records pointing to GitHub's IP addresses:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Or add CNAME record pointing to `yourusername.github.io`

---

## Troubleshooting

### Site Not Loading
- **Wait 5-10 minutes** for GitHub Pages to build
- Check repository is **Public**
- Verify files are in the root directory of `main` branch
- Check HTTPS is enabled in Settings > Pages

### Site Shows 404
- Ensure repository name is exactly `yourusername.github.io`
- Check that `index.html` is in the root folder
- Verify GitHub Pages is enabled in Settings

### Styles Not Loading
- Clear browser cache (Ctrl+Shift+Delete on Windows)
- Check that `styles.css` is in the root folder
- Verify CSS file path in HTML is correct

### JavaScript Not Working
- Check browser console for errors (F12)
- Verify `script.js` is in the root folder
- Check that script reference in HTML is correct

---

## Local Testing Before Publishing

Test your site locally before pushing to GitHub:

### Using Python (Windows/Mac/Linux):
```powershell
# Navigate to portfolio folder
cd path\to\gaurav-portfolio

# Start local server (Python 3)
python -m http.server 8000

# Open browser and visit
# http://localhost:8000
```

### Using Node.js:
```powershell
# Install http-server globally (first time only)
npm install -g http-server

# Run server
http-server

# Open browser and visit the URL shown
```

---

## File Structure

Your repository should look like this:

```
yourusername.github.io/
├── index.html
├── styles.css
├── script.js
├── README.md
├── .gitignore
├── _config.yml
└── CNAME (if using custom domain)
```

---

## Best Practices

1. **Regular Updates**: Update your portfolio regularly with new projects
2. **Test Before Publishing**: Always test locally first
3. **Commit Messages**: Use descriptive commit messages
4. **Version Control**: Don't delete old versions, use branches for experiments
5. **SEO**: Add meta tags for better search visibility
6. **Performance**: Optimize images if you add them
7. **Mobile Testing**: Always check on mobile devices

---

## Git Commands Reference

```powershell
# Clone repository
git clone https://github.com/yourusername/yourusername.github.io.git

# Check status
git status

# Add all files
git add .

# Add specific file
git add filename.html

# Commit changes
git commit -m "Your message here"

# Push changes
git push origin main

# Pull latest changes
git pull origin main

# Create new branch
git checkout -b branch-name

# Switch branch
git checkout branch-name

# View commit history
git log

# View differences
git diff
```

---

## Additional Resources

- [GitHub Pages Official Documentation](https://pages.github.com/)
- [Git Documentation](https://git-scm.com/doc)
- [HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [JavaScript Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

---

## Next Steps

1. ✅ Create GitHub account
2. ✅ Create repository named `yourusername.github.io`
3. ✅ Push all portfolio files
4. ✅ Wait for deployment
5. ✅ Share your portfolio URL with your network!

---

**Questions?** Feel free to check GitHub's official documentation or open an issue in your repository.

**Good luck with your portfolio launch!** 🚀

---

Last Updated: March 2026

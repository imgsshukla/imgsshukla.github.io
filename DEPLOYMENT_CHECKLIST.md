# 🚀 GitHub Pages Deployment Checklist

## Pre-Deployment Checklist

- [ ] All portfolio files are ready:
  - [ ] `index.html`
  - [ ] `styles.css`
  - [ ] `script.js`
  - [ ] `README.md`
  - [ ] `_config.yml`
  - [ ] `.gitignore`

- [ ] Tested locally (optional but recommended)
- [ ] All contact information is correct in `index.html`
- [ ] All project descriptions are accurate
- [ ] Experience timeline is up to date

## GitHub Account Setup

- [ ] GitHub account created at https://github.com
- [ ] Email verified
- [ ] Git installed on computer
- [ ] Configured git with your name and email:
  ```
  git config --global user.name "Your Name"
  git config --global user.email "your.email@gmail.com"
  ```

## Repository Creation

- [ ] Created new repository on GitHub
- [ ] Repository name: `yourusername.github.io`
  - [ ] (Replace `yourusername` with your actual GitHub username)
- [ ] Repository is set to **PUBLIC**
- [ ] Description added: "Data Engineer Portfolio"

## Deployment Steps

### Option A: Command Line (Windows PowerShell/Terminal)

- [ ] Navigate to portfolio folder:
  ```
  cd path\to\portfolio
  ```

- [ ] Initialize Git:
  ```
  git init
  ```

- [ ] Add all files:
  ```
  git add .
  ```

- [ ] Create first commit:
  ```
  git commit -m "Initial portfolio website"
  ```

- [ ] Set branch to main:
  ```
  git branch -M main
  ```

- [ ] Add remote (replace `yourusername`):
  ```
  git remote add origin https://github.com/yourusername/yourusername.github.io.git
  ```

- [ ] Push to GitHub:
  ```
  git push -u origin main
  ```

### Option B: GitHub Desktop (Graphical Interface)

- [ ] Downloaded GitHub Desktop from https://desktop.github.com
- [ ] Logged in with GitHub account
- [ ] Created new repository locally
- [ ] Added all portfolio files to repository folder
- [ ] Committed changes with message "Initial portfolio"
- [ ] Connected to remote GitHub repository
- [ ] Published to GitHub

## Post-Deployment Verification

- [ ] Waited 2-5 minutes for GitHub Pages to build
- [ ] Checked GitHub repository Settings > Pages
  - [ ] Source is set to "main" branch
  - [ ] Custom domain is NOT set (unless intentional)
- [ ] Visited `https://yourusername.github.io` in browser
- [ ] Portfolio loads successfully
- [ ] All sections are visible:
  - [ ] Hero section
  - [ ] Projects
  - [ ] Experience
  - [ ] Skills
  - [ ] About
  - [ ] Contact
- [ ] Styles are applied (colors, fonts, layout)
- [ ] JavaScript is working (menu, animations)
- [ ] Links are working (social, email, navigation)

## Content Verification

- [ ] Your name appears correctly
- [ ] Job title/subtitle is accurate
- [ ] Contact email is correct
- [ ] Phone number is correct
- [ ] Location is correct
- [ ] All project details are accurate
- [ ] Experience timeline is correct
- [ ] Skills list is complete
- [ ] Social media links work correctly
- [ ] LinkedIn URL is correct

## Browser Testing

Test on multiple browsers and devices:

- [ ] Google Chrome (Desktop)
- [ ] Mozilla Firefox (Desktop)
- [ ] Safari (Desktop, if Mac user)
- [ ] Edge (Desktop)
- [ ] Chrome (Mobile/Tablet)
- [ ] Safari (Mobile/Tablet)

Check on each:
- [ ] Page loads quickly
- [ ] Layout is responsive
- [ ] Navigation menu works
- [ ] Mobile menu works (hamburger)
- [ ] All links are clickable
- [ ] Text is readable
- [ ] Images/gradients look good

## SEO & Meta Information

- [ ] Verified in page source:
  - [ ] Title tag: "Gaurav Shukla - Data Engineer Portfolio"
  - [ ] Meta description is set
  - [ ] Viewport tag for responsive design

## Troubleshooting Checks

If site doesn't load:
- [ ] GitHub Pages enabled in Settings
- [ ] Repository is PUBLIC
- [ ] Repository name is exactly `yourusername.github.io`
- [ ] `index.html` is in root directory
- [ ] No errors in GitHub repository

If styles don't load:
- [ ] Browser cache cleared
- [ ] `styles.css` is in root directory
- [ ] File names are exact case match
- [ ] Files successfully pushed to GitHub

If JavaScript doesn't work:
- [ ] `script.js` is in root directory
- [ ] Browser console has no errors (F12)
- [ ] Files pushed successfully

## First Update Process

After verifying everything works:

- [ ] Made desired changes to files
- [ ] Tested changes locally
- [ ] Staged changes:
  ```
  git add .
  ```
- [ ] Committed changes:
  ```
  git commit -m "Describe your changes"
  ```
- [ ] Pushed to GitHub:
  ```
  git push
  ```
- [ ] Waited 1-3 minutes for update
- [ ] Verified changes on live site

## Optimization Checklist

- [ ] Portfolio loads in under 3 seconds
- [ ] Images (if any) are optimized
- [ ] CSS is minified (consider for future)
- [ ] JavaScript is minified (consider for future)
- [ ] No console errors when viewing site

## Custom Domain Setup (Optional)

If adding custom domain:
- [ ] Domain registered with registrar
- [ ] CNAME file created with domain name
- [ ] Created CNAME file in repository and pushed
- [ ] DNS records updated at registrar
  - [ ] A records (if using A records)
  - [ ] CNAME record (if using CNAME)
- [ ] Waited for DNS propagation (up to 48 hours)
- [ ] Custom domain verified in GitHub Settings
- [ ] HTTPS enabled automatically

## Ongoing Maintenance

- [ ] Bookmark your portfolio URL
- [ ] Share URL on:
  - [ ] LinkedIn profile
  - [ ] Twitter/X
  - [ ] GitHub bio
  - [ ] Email signature
  - [ ] Resume/CV
- [ ] Set reminder to update portfolio annually
- [ ] Plan to add new projects
- [ ] Update experience as roles change
- [ ] Monitor portfolio performance

## Final Sign-Off

- [ ] Portfolio is live and accessible
- [ ] All content is accurate and current
- [ ] Shared with network/connections
- [ ] Ready for job applications/networking!

---

## Useful Links to Keep Handy

- GitHub Pages Help: https://pages.github.com/
- Your Repository: https://github.com/yourusername/yourusername.github.io
- Your Live Site: https://yourusername.github.io
- GitHub Documentation: https://docs.github.com/
- Git Cheat Sheet: https://git-scm.com/docs

---

## Quick Command Reference

```bash
# Daily/Weekly Updates
git status              # Check what's changed
git add .              # Stage all changes
git commit -m "msg"    # Commit with message
git push               # Push to GitHub

# Check status
git log                # View commit history
git diff               # View changes

# If you need to undo
git reset HEAD~1       # Undo last commit
git revert HEAD        # Create reverse commit
```

---

**You've got this!** 🎉

Your portfolio is now ready to showcase your skills to the world.

---

Last Updated: March 2026

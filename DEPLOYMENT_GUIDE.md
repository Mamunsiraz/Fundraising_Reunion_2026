# 🚀 GitHub Pages Deployment Guide

## Step-by-Step Instructions to Host Your Donation System

### Option 1: Using GitHub Web Interface (Easiest)

#### Step 1: Create a New Repository
1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **"+"** icon in the top right corner
3. Select **"New repository"**
4. Name your repository (e.g., `donation-system` or `charity-dashboard`)
5. Choose **"Public"** (required for free GitHub Pages)
6. Click **"Create repository"**

#### Step 2: Upload Your Files
1. On your new repository page, click **"uploading an existing file"**
2. Drag and drop these 4 files:
   - `index.html`
   - `funding.html`
   - `expenditure.html`
   - `README.md`
3. Click **"Commit changes"**

#### Step 3: Enable GitHub Pages
1. Go to your repository's **Settings** (top menu)
2. Scroll down and click **"Pages"** in the left sidebar
3. Under **"Source"**, select:
   - Branch: **main** (or **master**)
   - Folder: **/ (root)**
4. Click **"Save"**
5. Wait 1-2 minutes for deployment

#### Step 4: Access Your Website
Your site will be live at:
```
https://YOUR-USERNAME.github.io/REPOSITORY-NAME/
```

Example: `https://johndoe.github.io/donation-system/`

---

### Option 2: Using Git Command Line (Advanced)

#### Prerequisites
- Install Git on your computer
- Have a GitHub account

#### Step 1: Initialize Git Repository
```bash
# Navigate to your project folder
cd path/to/your/donation-system

# Initialize git
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit: Donation management system"
```

#### Step 2: Create GitHub Repository
1. Go to GitHub.com and create a new repository
2. **Do not** initialize with README (we already have one)
3. Copy the repository URL

#### Step 3: Push to GitHub
```bash
# Add remote repository
git remote add origin https://github.com/YOUR-USERNAME/REPOSITORY-NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

#### Step 4: Enable GitHub Pages
Follow **Step 3** from Option 1 above

---

## 🎯 Custom Domain (Optional)

### Using Your Own Domain

1. Buy a domain from any registrar (GoDaddy, Namecheap, etc.)
2. In your repository, create a file named `CNAME`
3. Add your domain to the CNAME file:
   ```
   www.yourdonationsite.com
   ```
4. In your domain registrar's DNS settings, add:
   - Type: **CNAME**
   - Name: **www**
   - Value: **YOUR-USERNAME.github.io**

---

## 🔧 Updating Your Website

### Via Web Interface
1. Go to your repository on GitHub
2. Click on the file you want to edit
3. Click the pencil icon (Edit)
4. Make changes
5. Click **"Commit changes"**
6. Wait 1-2 minutes for the site to update

### Via Git Command Line
```bash
# Make changes to your files locally

# Stage changes
git add .

# Commit changes
git commit -m "Updated donation amounts"

# Push to GitHub
git push origin main
```

---

## 📊 Common Customizations

### Update Organization Name
Edit the logo in all three HTML files:
```html
<div class="logo">Your Charity Name</div>
```

### Update Donor Information (funding.html)
Find the donor sections and update:
```html
<div class="donor-name">New Donor Name</div>
<div class="donation-amount">$XX,XXX</div>
```

### Update Expense Data (expenditure.html)
Find the category sections and update:
```html
<div class="category-name">New Category</div>
<div class="category-amount">$XX,XXX</div>
```

### Change Color Scheme
In each HTML file's `<style>` section, find and replace gradient colors:
```css
/* Funding page - Blue gradient */
background: linear-gradient(135deg, #3b82f6 0%, #06b6d4 100%);

/* Expenditure page - Red gradient */
background: linear-gradient(135deg, #ef4444 0%, #f97316 100%);

/* Homepage - Purple gradient */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

---

## ✅ Verification Checklist

- [ ] All 4 files uploaded to GitHub
- [ ] GitHub Pages enabled in Settings
- [ ] Website accessible via GitHub Pages URL
- [ ] Navigation menu works between pages
- [ ] Responsive design works on mobile
- [ ] All data displays correctly

---

## 🐛 Troubleshooting

### Site Not Loading?
1. Wait 2-3 minutes after enabling Pages
2. Check that repository is **Public**
3. Verify files are in root directory (not in a subfolder)
4. Clear browser cache and try again

### Navigation Links Not Working?
- Make sure all `.html` files are in the same directory
- Check file names match exactly (case-sensitive)

### Images Not Showing?
- Profile images use Pravatar.cc (requires internet)
- Replace with your own images if needed

### 404 Error?
- Check GitHub Pages settings
- Ensure branch is set to `main` or `master`
- Verify URL format: `username.github.io/repo-name/`

---

## 📚 Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Tutorial](https://git-scm.com/docs/gittutorial)
- [Markdown Guide](https://www.markdownguide.org/)

---

## 🎉 Success!

Once deployed, share your website URL with donors and stakeholders!

```
🌐 Your Live Site: https://YOUR-USERNAME.github.io/REPOSITORY-NAME/
```

---

**Need Help?** Open an issue on your GitHub repository or contact support.

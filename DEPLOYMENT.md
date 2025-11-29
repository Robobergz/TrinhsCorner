# Quick Deployment Guide

## 🚀 Deploy to GitHub Pages (5 minutes)

### Step 1: Create GitHub Repository
1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon → **New repository**
3. Name it: `restaurant-menu` (or any name you like)
4. Make it **Public**
5. Click **Create repository**

### Step 2: Upload Your Files
Two options:

#### Option A: Using GitHub Web Interface (Easiest)
1. On your new repository page, click **uploading an existing file**
2. Drag and drop all files from the unzipped folder
3. Write commit message: "Initial menu website"
4. Click **Commit changes**

#### Option B: Using Git Command Line
```bash
# In your terminal, navigate to the unzipped folder
cd restaurant-menu-site

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial menu website"

# Connect to GitHub (replace USERNAME and REPO)
git remote add origin https://github.com/USERNAME/REPO.git

# Push
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (in left sidebar)
3. Under "Source", select **main** branch
4. Click **Save**
5. Wait 1-2 minutes
6. Your site will be live at: `https://USERNAME.github.io/REPO-NAME/`

## 🎨 Adding Your Images

### Quick Method:
1. Upload your images to `assets/images/` folder on GitHub
2. Edit `index.html` directly on GitHub
3. Click the pencil icon to edit
4. Find placeholder lines like:
   ```html
   <div class="item-image-placeholder pho-bg">🍜</div>
   ```
5. Replace with:
   ```html
   <img src="assets/images/your-photo.jpg" alt="Description" class="item-image">
   ```
6. Commit changes
7. Changes will be live in ~1 minute

### Better Method:
1. Clone your repository locally:
   ```bash
   git clone https://github.com/USERNAME/REPO.git
   ```
2. Add images to `assets/images/` folder
3. Edit `index.html` in your favorite code editor
4. Commit and push:
   ```bash
   git add .
   git commit -m "Added food images"
   git push
   ```

## 🔗 Custom Domain (Optional)

Want to use your own domain like `menu.myrestaurant.com`?

1. Buy a domain from [Namecheap](https://namecheap.com) or [Google Domains](https://domains.google)
2. In GitHub Settings → Pages, add your custom domain
3. Update your domain's DNS settings with GitHub's IPs
4. Full guide: [GitHub Docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## 📱 QR Code for Customers

Once live, create a QR code for your URL:
1. Visit [qr-code-generator.com](https://www.qr-code-generator.com)
2. Enter your GitHub Pages URL
3. Download QR code
4. Print and display at tables!

## 🆘 Need Help?

- GitHub Pages not working? Check repository is **Public**
- Images not showing? Check file paths are correct
- Changes not appearing? Wait 1-2 minutes or do a hard refresh (Ctrl+Shift+R)

---

**Your menu is ready to go live! 🎉**

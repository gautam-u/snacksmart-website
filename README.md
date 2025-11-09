# SnackSmart Website

**Official website for SnackSmart iOS app - REQUIRED for App Store submission**

This Jekyll website provides the **mandatory** Privacy Policy and Support pages required by Apple App Store, plus a landing page to showcase your app.

## 🚨 Why This Website is REQUIRED

Apple App Store **requires** two URLs before you can submit your app:
1. **Privacy Policy URL** (mandatory) - shows how you handle user data
2. **Support URL** (mandatory) - provides customer support contact

Without these URLs publicly accessible, **your app will be rejected**.

---

## 📋 Website Structure

```
SnackSmartWebsite/
├── _config.yml          # Site configuration
├── _layouts/
│   └── default.html     # Page layout template
├── index.md             # Landing page with app features
├── privacy-policy.md    # REQUIRED - Privacy policy (Apple mandate)
├── support.md           # REQUIRED - Support/FAQ page (Apple mandate)
├── terms.md             # Terms of Service (recommended)
├── assets/
│   └── screenshots/     # Place app screenshots here
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```

---

## 🚀 Quick Deployment (GitHub Pages - FREE)

### Option 1: Deploy to GitHub Pages (Recommended - FREE)

**Step 1: Create GitHub Repository**
```bash
cd /Users/gauti/Developer/projects/ios/SnackSmartWebsite
git init
git add .
git commit -m "Initial commit - SnackSmart website"
```

**Step 2: Create Repository on GitHub**
1. Go to https://github.com/new
2. Repository name: `snacksmart-website`
3. Make it **Public** (required for GitHub Pages free tier)
4. Click "Create repository"

**Step 3: Push to GitHub**
```bash
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/snacksmart-website.git
git push -u origin main
```

**Step 4: Enable GitHub Pages**
1. Go to repository Settings → Pages
2. Source: Deploy from a branch
3. Branch: `main` → `/ (root)` → Save
4. Wait 2-5 minutes for deployment

**Your website will be live at:**
```
https://YOUR-USERNAME.github.io/snacksmart-website/
```

**URLs for App Store Connect:**
- **Privacy Policy:** `https://YOUR-USERNAME.github.io/snacksmart-website/privacy-policy/`
- **Support URL:** `https://YOUR-USERNAME.github.io/snacksmart-website/support/`
- **Landing Page:** `https://YOUR-USERNAME.github.io/snacksmart-website/`

---

### Option 2: Test Locally First

**Install Jekyll (one-time setup):**
```bash
# macOS with Homebrew
brew install ruby
gem install bundler jekyll

# Install dependencies
cd /Users/gauti/Developer/projects/ios/SnackSmartWebsite
bundle install
```

**Run Local Server:**
```bash
bundle exec jekyll serve
```

**Open in browser:**
```
http://localhost:4000/snacksmart-website/
```

---

## 📸 Adding App Screenshots

### Step 1: Capture Screenshots

**On iPhone Simulator:**
```bash
# Run your app in Xcode simulator (iPhone 6.7" - iPhone 14 Pro Max or similar)
# Press ⌘S to save screenshot
```

Screenshots are saved to: `~/Desktop/`

**Required Size:** 1290 x 2796 pixels (iPhone 6.7")

### Step 2: Add Screenshots to Website

```bash
# Copy screenshots to website
cp ~/Desktop/screenshot1.png /Users/gauti/Developer/projects/ios/SnackSmartWebsite/assets/screenshots/dashboard.png
cp ~/Desktop/screenshot2.png /Users/gauti/Developer/projects/ios/SnackSmartWebsite/assets/screenshots/camera.png
cp ~/Desktop/screenshot3.png /Users/gauti/Developer/projects/ios/SnackSmartWebsite/assets/screenshots/healthkit.png
cp ~/Desktop/screenshot4.png /Users/gauti/Developer/projects/ios/SnackSmartWebsite/assets/screenshots/premium.png
cp ~/Desktop/screenshot5.png /Users/gauti/Developer/projects/ios/SnackSmartWebsite/assets/screenshots/analytics.png
cp ~/Desktop/screenshot6.png /Users/gauti/Developer/projects/ios/SnackSmartWebsite/assets/screenshots/history.png
```

### Step 3: Update and Deploy

```bash
git add assets/screenshots/
git commit -m "Add app screenshots"
git push
```

---

## ⚙️ Configuration

### Update Your Information

Edit `_config.yml`:

```yaml
# Update these fields
email_address: your-email@example.com  # Your support email
appstore_link: https://apps.apple.com/us/app/snacksmart/idXXXXXXXXXX  # After app is live
github_username: your-github-username

# Keep baseurl and url for GitHub Pages
baseurl: "/snacksmart-website"
url: "https://your-github-username.github.io"
```

---

## 📝 Customization

### Modify Privacy Policy

Edit `privacy-policy.md` to match your exact data practices:
- Update email address in contact section
- Adjust data collection details if you change features
- Keep sections that match your actual implementation

### Modify Support Page

Edit `support.md`:
- Update FAQ based on common user questions
- Add/remove questions as your app evolves
- Update email address

### Modify Landing Page

Edit `index.md`:
- Update app description
- Modify features list
- Update pricing if you change subscription costs

---

## 🔄 Deployment Workflow

### Making Changes

```bash
# Edit files locally
nano privacy-policy.md

# Test changes
bundle exec jekyll serve

# Commit and push
git add .
git commit -m "Update privacy policy"
git push

# GitHub Pages will auto-deploy in 2-5 minutes
```

---

## 📱 App Store Connect Integration

### Step 1: Get Your URLs

After deploying to GitHub Pages, your URLs are:
- **Privacy:** `https://YOUR-USERNAME.github.io/snacksmart-website/privacy-policy/`
- **Support:** `https://YOUR-USERNAME.github.io/snacksmart-website/support/`

### Step 2: Add to App Store Connect

1. Go to https://appstoreconnect.apple.com
2. Select your app (SnackSmart)
3. Navigate to "App Information"
4. Enter URLs:
   - **Privacy Policy URL:** (paste privacy policy URL)
   - **Support URL:** (paste support URL)
5. Click "Save"

**✅ You can now submit your app!**

---

## 🌐 Alternative Hosting Options

### Cloudflare Pages (Free)
- Fastest performance globally
- Built-in SSL
- Deploy from GitHub
- https://pages.cloudflare.com

### Netlify (Free)
- Easy drag-and-drop deployment
- Custom domains
- Auto-deploy from Git
- https://www.netlify.com

### Vercel (Free)
- Fast deployment
- Great for static sites
- Git integration
- https://vercel.com

### Custom Domain

If you want a custom domain (e.g., `snacksmart.com`):
1. Buy domain from Namecheap, GoDaddy, or Google Domains
2. Point DNS to your hosting provider
3. Update `_config.yml`:
   ```yaml
   url: "https://snacksmart.com"
   baseurl: ""
   ```

---

## ✅ Pre-Launch Checklist

Before submitting to App Store:

- [ ] Website deployed and accessible
- [ ] Privacy Policy URL works: `https://yoursite.com/privacy-policy/`
- [ ] Support URL works: `https://yoursite.com/support/`
- [ ] Terms of Service URL works: `https://yoursite.com/terms/`
- [ ] Email address is correct in all pages
- [ ] App screenshots uploaded to `assets/screenshots/`
- [ ] Landing page reflects current app features
- [ ] Privacy policy matches actual data collection
- [ ] Support page has accurate information

---

## 📞 Support

If you need help with the website:
- Email: {{ site.email_address }}
- GitHub Issues: Create issue in repository

---

## 📜 License

This website template is based on the FitJournal/HomeWorkout website structure.

---

**🎉 Your website is now ready for App Store submission!**

**Next Steps:**
1. Deploy website to GitHub Pages
2. Add URLs to App Store Connect
3. Submit your app for review
4. Celebrate when approved! 🚀

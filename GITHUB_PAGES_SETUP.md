# 🚀 GitHub Pages Setup Guide - Step by Step

## 📋 Your Current Status
✅ Repository created: naveenkumar.github.io
✅ index.html uploaded

## 🎯 Complete Setup Steps

---

## STEP 1: Verify Your Repository Name

Your repository name should be EXACTLY:
```
YOUR-GITHUB-USERNAME.github.io
```

For example:
- If username is `naveenkumar2024`, repo should be `naveenkumar2024.github.io`
- If username is `naveen-kumar`, repo should be `naveen-kumar.github.io`

⚠️ **IMPORTANT**: The username in the repository name must match your actual GitHub username exactly!

---

## STEP 2: Check Your Repository Settings

1. Go to your repository: `https://github.com/YOUR-USERNAME/naveenkumar.github.io`

2. Click on **"Settings"** tab (top right of the repository)

3. Scroll down and look for **"GitHub Pages"** section in the left sidebar
   - Click on **"Pages"**

4. Under **"Source"**, you should see:
   - Branch: **main** (or **master**)
   - Folder: **/ (root)**

5. Click **"Save"** if you made any changes

---

## STEP 3: Wait for Deployment (1-2 minutes)

After saving:
1. You'll see a blue box saying: "Your site is ready to be published at..."
2. Wait 1-2 minutes
3. The box will turn **green** and say: "Your site is published at..."

---

## STEP 4: Access Your Website

Your live website URL will be:
```
https://YOUR-USERNAME.github.io/
```

Example:
- If your username is `naveenkumar2024`, your URL is:
  `https://naveenkumar2024.github.io/`

---

## 🔧 TROUBLESHOOTING

### Problem 1: "404 - There isn't a GitHub Pages site here"

**Solutions:**
1. **Check repository name**
   - Go to repository Settings → scroll to bottom
   - Look for "Repository name"
   - It MUST be `your-username.github.io` (all lowercase)
   - If wrong, rename it: Settings → scroll to bottom → "Rename repository"

2. **Check file name**
   - Your file MUST be named `index.html` (not `index_fixed.html`)
   - Go to your repository
   - Click on the file
   - If it's named wrong, click the pencil icon (Edit)
   - Change filename at top to `index.html`
   - Scroll down and click "Commit changes"

3. **Check if repository is Public**
   - Go to Settings
   - Scroll to bottom to "Danger Zone"
   - If it says "Make public", click it
   - GitHub Pages only works with public repos (on free plan)

### Problem 2: Repository name mismatch

If your repository is named `naveenkumar.github.io` but your actual username is different:

**Fix it:**
1. Go to repository **Settings**
2. Scroll to bottom ("Danger Zone")
3. Click **"Rename repository"**
4. Change to: `YOUR-ACTUAL-USERNAME.github.io`
5. Click "I understand, rename repository"

### Problem 3: Website shows but book data doesn't load

**This is normal!** The Google Sheets URL is already configured, but:
1. Make sure your Google Sheet is **published to web**
2. The CSV URL should end with `pub?output=csv`
3. Clear browser cache (Ctrl + F5 / Cmd + Shift + R)
4. Wait 30 seconds and refresh again

---

## 📝 STEP-BY-STEP: Repository Rename (If Needed)

If your GitHub username is different from "naveenkumar":

### Find Your Actual Username:
1. Go to https://github.com
2. Click your profile picture (top right)
3. Your username is shown below your name
   - Example: @naveenkumar2024

### Rename Repository:
1. Go to your repository
2. Click **"Settings"** (top menu)
3. Scroll all the way down to **"Danger Zone"** section
4. Click **"Rename repository"**
5. In the box, type: `your-actual-username.github.io`
   - If your username is `naveenkumar2024`, type: `naveenkumar2024.github.io`
6. Click **"I understand, rename repository"**

### Enable GitHub Pages:
1. Still in Settings, click **"Pages"** (left sidebar)
2. Under "Source":
   - Branch: Select **main** (or **master**)
   - Folder: Select **/ (root)**
3. Click **"Save"**
4. Wait 1-2 minutes
5. Refresh the page
6. You'll see: "Your site is published at https://your-username.github.io/"

---

## ✅ FINAL CHECKLIST

Before your site works, verify:

- [ ] Repository name matches your username exactly
  - Format: `username.github.io` (all lowercase)

- [ ] Repository is **Public** (not Private)

- [ ] File is named `index.html` (not `index_fixed.html`)

- [ ] GitHub Pages is enabled in Settings → Pages

- [ ] Source is set to "main" branch and "/ (root)" folder

- [ ] Waited 2-3 minutes after enabling Pages

- [ ] Your Google Sheets CSV URL is configured in the HTML file

---

## 🌐 WHAT YOUR URL WILL BE

Based on your GitHub username:

| GitHub Username | Your Website URL |
|----------------|------------------|
| naveenkumar | https://naveenkumar.github.io/ |
| naveenkumar2024 | https://naveenkumar2024.github.io/ |
| naveen-kumar | https://naveen-kumar.github.io/ |

The URL ALWAYS follows this pattern:
```
https://YOUR-GITHUB-USERNAME.github.io/
```

---

## 📱 TEST YOUR WEBSITE

Once deployed, test these features:

1. **Basic Load**: Does the website show?
2. **Book Data**: Do you see all 39 sections and books?
3. **Statistics**: Are the numbers correct at the top?
4. **Navigation**: Click on a section - does it scroll?
5. **Filters**: Try "Available Only" filter
6. **Mobile**: Open on your phone - is it responsive?

---

## 🔄 UPDATE WORKFLOW (After Initial Setup)

To update book availability in the future:

1. **Edit Google Sheet**
   - Add "(UNAVAILABLE)" to book names
   - Example: "Bible Study Source Book (UNAVAILABLE)"

2. **Wait 5 minutes** (or refresh the website)

3. **Check website** - book should show in red

**No need to touch GitHub!** Just edit Google Sheets.

---

## 🆘 STILL NOT WORKING?

### Check Browser Console:
1. Open your website
2. Press **F12** (or right-click → Inspect)
3. Click **"Console"** tab
4. Look for red error messages
5. Share the error message for help

### Common Error Messages:

**"Failed to fetch"**
- Solution: Check Google Sheets URL in index.html
- Make sure sheet is published to web

**"404 Not Found"**
- Solution: Repository name or file name is wrong
- Follow "Problem 1" above

**"Access Denied"**
- Solution: Repository must be Public
- Go to Settings → scroll down → "Change visibility"

---

## 📧 QUICK SUMMARY

Your website setup is almost done! Just verify:

1. ✅ Repository name: `your-username.github.io`
2. ✅ File name: `index.html`
3. ✅ Repository: Public
4. ✅ GitHub Pages: Enabled (Settings → Pages)
5. ✅ Wait 2-3 minutes
6. ✅ Visit: `https://your-username.github.io/`

That's it! Your book library will be live! 🎉

---

## 🎓 EXAMPLE: Complete Setup

Let's say your GitHub username is `naveenkumar2024`:

1. **Repository**: `naveenkumar2024.github.io`
2. **File**: `index.html` (in root folder)
3. **Settings → Pages**: Enable with main branch
4. **Wait**: 2 minutes
5. **Visit**: `https://naveenkumar2024.github.io/`
6. **Share**: Send this URL to users!

✅ Done! Books are live and update from Google Sheets automatically!

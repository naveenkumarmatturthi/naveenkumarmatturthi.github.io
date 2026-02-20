# 📚 Book Library - Google Sheets + GitHub Pages Setup Guide

## 🎯 Overview
This solution allows you to:
- Update book availability in **Google Sheets** (easy to edit)
- Automatically update the **live website** (hosted free on GitHub Pages)
- Mark unavailable books in red (just highlight them in Google Sheets)
- No coding required for updates!

---

## 📝 Step-by-Step Setup

### STEP 1: Upload Excel to Google Sheets

1. **Go to Google Sheets**: https://sheets.google.com
2. **Create a new sheet** or click "File" → "Open"
3. **Upload your Excel file** (Grace-Section.xlsx)
   - Click "File" → "Import" → "Upload"
   - Select your Excel file
   - Choose "Replace spreadsheet" or "Create new spreadsheet"

### STEP 2: Mark Unavailable Books (IMPORTANT!)

To mark books as unavailable (they will show in red on the website):

**Method 1: Add "(UNAVAILABLE)" to book name**
- In the "Name" column, add " (UNAVAILABLE)" after the book name
- Example: "Bible Study Source Book (UNAVAILABLE)"

**Method 2: Highlight cells in red**
- Select the book row
- Click on text color or fill color
- Choose red color

### STEP 3: Publish Google Sheet as CSV

1. In Google Sheets, click **"File"** → **"Share"** → **"Publish to web"**
2. In the dialog:
   - **First dropdown**: Select your sheet (usually "Sheet1")
   - **Second dropdown**: Select "Comma-separated values (.csv)"
3. Click **"Publish"**
4. **Copy the URL** that appears (it looks like):
   ```
   https://docs.google.com/spreadsheets/d/e/2PACX-1vXXXXXX.../pub?output=csv
   ```
5. **Keep this URL safe** - you'll need it in the next step!

### STEP 4: Configure the Website

1. **Open the `index.html` file** in a text editor (Notepad, VS Code, etc.)
2. **Find this line** (around line 450):
   ```javascript
   const GOOGLE_SHEETS_CSV_URL = 'YOUR_GOOGLE_SHEETS_CSV_URL_HERE';
   ```
3. **Replace** `'YOUR_GOOGLE_SHEETS_CSV_URL_HERE'` with your actual CSV URL:
   ```javascript
   const GOOGLE_SHEETS_CSV_URL = 'https://docs.google.com/spreadsheets/d/e/2PACX-1vXXXXXX.../pub?output=csv';
   ```
4. **Save the file**

### STEP 5: Deploy to GitHub Pages (FREE Hosting!)

#### Option A: Using GitHub Website (Easiest)

1. **Create a GitHub account** (if you don't have one): https://github.com/signup
2. **Create a new repository**:
   - Go to https://github.com/new
   - Repository name: `book-library` (or any name you want)
   - Make it **Public**
   - Click "Create repository"

3. **Upload your file**:
   - Click "uploading an existing file"
   - Drag and drop your `index.html` file
   - Click "Commit changes"

4. **Enable GitHub Pages**:
   - Go to repository "Settings"
   - Scroll down to "Pages" section (left sidebar)
   - Under "Source", select "main" branch
   - Click "Save"

5. **Get your website URL**:
   - Wait 1-2 minutes
   - Your site will be live at: `https://YOUR-USERNAME.github.io/book-library/`

#### Option B: Using GitHub Desktop (For Regular Updates)

1. **Download GitHub Desktop**: https://desktop.github.com
2. **Create a new repository** in GitHub Desktop
3. **Add your `index.html` file** to the repository folder
4. **Publish** to GitHub
5. **Enable GitHub Pages** (same as Option A, step 4)

---

## 🔄 How to Update Books (Daily Workflow)

### To Mark a Book as Unavailable:
1. Open your Google Sheet
2. Find the book
3. Add " (UNAVAILABLE)" to the book name
   - OR highlight the row in red color
4. **That's it!** The website updates automatically (within 5 minutes)

### To Mark a Book as Available Again:
1. Open your Google Sheet
2. Remove " (UNAVAILABLE)" from the book name
   - OR remove the red highlight
3. Website updates automatically

### Tips:
- Changes take effect immediately (browser cache refresh)
- Website auto-refreshes every 5 minutes
- No need to republish anything!

---

## 🎨 Features of the Website

✅ **Live Status Updates** from Google Sheets
✅ **Red highlighting** for unavailable books
✅ **Status badges** (Available/Unavailable)
✅ **Statistics dashboard** (Total, Available, Unavailable counts)
✅ **Filter buttons** (All / Available Only / Unavailable Only)
✅ **Mobile responsive** (works on phones, tablets, desktops)
✅ **Search-friendly** table of contents
✅ **Print to PDF** support
✅ **Auto-refresh** every 5 minutes

---

## 🆓 Cost Breakdown

| Service | Cost | Purpose |
|---------|------|---------|
| Google Sheets | **FREE** | Edit and update book data |
| GitHub Pages | **FREE** | Host the website (unlimited bandwidth) |
| **TOTAL** | **$0/month** | 100% Free Solution! |

---

## 🔧 Troubleshooting

### Website shows "Unable to Load Data"
**Solution**: Make sure you:
1. Published the Google Sheet to web as CSV
2. Copied the correct CSV URL (should end with `pub?output=csv`)
3. Replaced the URL in `index.html` correctly

### Books not updating
**Solution**:
1. Check if Google Sheet is published (File → Share → Publish to web)
2. Clear browser cache (Ctrl + F5 / Cmd + Shift + R)
3. Wait 5 minutes for auto-refresh

### Can't access GitHub Pages URL
**Solution**:
1. Make sure repository is **Public** (not Private)
2. Wait 2-3 minutes after enabling GitHub Pages
3. Check Settings → Pages to see if it's deployed

---

## 📱 Alternative Free Hosting Options

If you prefer not to use GitHub Pages, here are alternatives:

1. **Netlify** (https://netlify.com)
   - Drag and drop `index.html`
   - Instant deployment
   - Free SSL certificate

2. **Vercel** (https://vercel.com)
   - Import from GitHub
   - Auto-deploy on changes
   - Fast CDN

3. **Cloudflare Pages** (https://pages.cloudflare.com)
   - Similar to GitHub Pages
   - Better performance in some regions

All are 100% FREE for static sites!

---

## 📧 Need Help?

If you get stuck:
1. Check the Google Sheets URL format
2. Verify the file is published to web
3. Test the CSV URL in your browser (should download a CSV file)
4. Check browser console for errors (F12 → Console tab)

---

## 🎉 You're All Set!

Your book library is now:
- ✅ Live on the internet (free!)
- ✅ Easy to update (just edit Google Sheets)
- ✅ Automatically shows unavailable books in red
- ✅ Mobile-friendly and professional-looking

Share your GitHub Pages URL with users and they'll always see the latest book availability!

Example URL: `https://your-username.github.io/book-library/`

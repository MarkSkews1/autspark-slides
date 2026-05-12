# 🎯 AutSpark Slides - Quick Reference

## 📍 Local Preview

Your presentation is currently running at:  
**http://localhost:3456**

Open this in your browser to preview the slides!

---

## 🎬 Presentation Preview

**Slide Count:** 12 slides  
**Theme:** Clean white professional theme  
**Framework:** Reveal.js

### Slide Flow:
1. **Opening** - Smarter Laundry Operations
2. **The Problem** - Operational data trapped
3. **Hidden Costs** - Where efficiency is lost
4. **Market Shift** - From reactive to intelligent
5. **Introducing AutSpark** - Operational intelligence
6. **How It Works** - 4 phases to results
7. **Key Benefits** - What you'll actually see
8. **Early Adopter Advantage** - Why partner with AutSpark
9. **3-Month Pilot** - Proof of concept
10. **Timeline** - Getting started
11. **Core Truth** - You can't manage what you can't see
12. **Call to Action** - Let's build this together

---

## 🎨 Visual Features

✓ Professional color scheme (dark blue headers, red highlights)  
✓ Clean tables and lists  
✓ Grid layouts for benefits  
✓ Speaker notes on first slide  
✓ Mobile responsive design  

---

## 🚀 Deploy to Railway - Quick Steps

### 1️⃣ Create GitHub Repo

On GitHub.com, create a new repository called `autspark-slides`

### 2️⃣ Push Code

```bash
cd /home/mark-skews/Dev/LinCore/autspark-slides
git remote add origin https://github.com/YOUR_USERNAME/autspark-slides.git
git branch -M main
git push -u origin main
```

### 3️⃣ Deploy on Railway

1. Go to https://railway.app
2. Click **"New Project"**
3. Select **"Deploy from GitHub repo"**
4. Choose **autspark-slides**
5. Click **"Deploy"**
6. Wait 2-3 minutes for build

### 4️⃣ Get Public URL

1. In Railway dashboard, click your service
2. Go to **Settings** → **Domains**
3. Click **"Generate Domain"**
4. Copy the URL (e.g., `autspark-slides.up.railway.app`)

### 5️⃣ Share with Prospects! 🎉

Send them the URL - that's it!

---

## 🔧 Making Updates

**To update slides:**

1. Edit `public/index.html` in your project
2. Commit and push:
   ```bash
   git add .
   git commit -m "Update slide content"
   git push
   ```
3. Railway auto-deploys in 2-3 minutes!

---

## 💡 Pro Tips

### For Presenters:
- **Press 's'** during presentation to open speaker notes
- **Press 'f'** for fullscreen mode
- **Press Esc** to see all slides at once (overview mode)
- **Use arrow keys** to navigate smoothly

### For Sharing:
- Add `?print-pdf` to URL to get PDF export mode
- Example: `https://your-url.up.railway.app/?print-pdf`
- Then print to PDF from Chrome

### For Analytics (Optional):
- Add Google Analytics to `public/index.html` before `</head>`
- Track how many prospects view your slides

---

## 🎯 Expected Result After Deployment

**Before:** Markdown file on your computer  
**After:** Professional web presentation accessible worldwide

**URL Structure:**
- Development: `http://localhost:3456`
- Production: `https://autspark-slides.up.railway.app`

**Features Unlocked:**
- ✅ Share link with anyone
- ✅ Mobile/tablet friendly
- ✅ Presenter mode with notes
- ✅ Professional appearance
- ✅ Always available
- ✅ No downloads required for viewers

---

## 📞 Support

If you need help:
1. Check `README.md` for general info
2. Check `RAILWAY_DEPLOY.md` for deployment details
3. Check Railway logs if deployment fails
4. Verify `Dockerfile` and `package.json` are unchanged

---

**Status:** ✅ Ready to deploy!  
**Next:** Push to GitHub → Deploy to Railway → Share with prospects


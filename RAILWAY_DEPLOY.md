# Railway Deployment Guide for AutSpark Slides

## Quick Deploy to Railway

### Option 1: Deploy from GitHub (Recommended)

1. **Initialize Git Repository**
   ```bash
   cd autspark-slides
   git init
   git add .
   git commit -m "Initial commit: AutSpark Nordic presentation"
   ```

2. **Push to GitHub**
   ```bash
   # Create a new repo on GitHub first, then:
   git remote add origin https://github.com/YOUR_USERNAME/autspark-slides.git
   git branch -M main
   git push -u origin main
   ```

3. **Deploy on Railway**
   - Go to https://railway.app
   - Click "New Project"
   - Select "Deploy from GitHub repo"
   - Choose your `autspark-slides` repository
   - Railway will auto-detect the Dockerfile
   - Click "Deploy"

4. **Set Custom Domain (Optional)**
   - In Railway dashboard, go to your service
   - Click "Settings" → "Domains"
   - Click "Generate Domain" (gets something like `autspark-slides.up.railway.app`)
   - Or add your custom domain

### Option 2: Deploy with Railway CLI

```bash
# Install Railway CLI
npm i -g @railway/cli

# Login
railway login

# Initialize project
cd autspark-slides
railway init

# Deploy
railway up

# Generate public URL
railway domain
```

## Environment Variables

No environment variables needed! The app works out of the box.

## Port Configuration

Railway automatically sets the `PORT` environment variable. The app is already configured to use `process.env.PORT || 3000`.

## Expected URLs

After deployment, you'll get a URL like:
- `https://autspark-slides-production.up.railway.app`
- `https://autspark-slides.up.railway.app`

## Updating the Presentation

1. Edit `public/index.html`
2. Commit and push changes:
   ```bash
   git add .
   git commit -m "Update presentation content"
   git push
   ```
3. Railway will automatically redeploy!

## Sharing with Prospects

Share the Railway URL directly:
- Clean, professional URL
- Always available
- Fast loading
- Mobile-friendly
- No authentication required

## Troubleshooting

### Build Fails
- Check Railway logs for errors
- Verify `package.json` is present
- Ensure `Dockerfile` is in root directory

### App Crashes
- Check Railway logs
- Verify port binding: app must listen on `process.env.PORT`

### Slides Don't Display
- Check browser console for errors
- Verify CDN links for Reveal.js are accessible
- View page source to confirm HTML is served

## Cost

Railway free tier includes:
- 500 hours/month of usage
- $5 credit/month
- Perfect for a presentation site!

This presentation site uses minimal resources and will easily fit in the free tier.


# GitHub Pages Deployment Guide

## ✅ What's Been Set Up

Your repository now includes a GitHub Actions workflow (`.github/workflows/deploy.yml`) that automatically deploys your site to GitHub Pages whenever you push to the `main` branch.

## 🚀 Enable GitHub Pages with Actions

Follow these steps to enable deployment:

### Step 1: Configure GitHub Pages Settings

1. Go to your repository: https://github.com/m-global/web
2. Click on **Settings** (top right)
3. In the left sidebar, click **Pages**
4. Under **"Source"**, select **"GitHub Actions"** (not "Deploy from a branch")
5. Save (it should auto-save)

### Step 2: Workflow Will Auto-Run

Once you set the source to "GitHub Actions", the workflow will automatically:
- Trigger on every push to `main` branch
- Build and upload the site files
- Deploy to GitHub Pages

You can also manually trigger the workflow:
- Go to **Actions** tab in your repository
- Select "Deploy to GitHub Pages" workflow
- Click "Run workflow" button

### Step 3: Access Your Sites

After deployment completes (usually 1-2 minutes), your sites will be live at:

- **Landing Page**: https://m-global.github.io/web/
- **FunkTechnik**: https://m-global.github.io/web/funk-technik/
- **TEKNIK**: https://m-global.github.io/web/tekniks-pro-audio/

## 📊 Monitor Deployment

- View deployment status: https://github.com/m-global/web/actions
- Each push triggers a new deployment automatically
- Green checkmark ✅ = successful deployment
- Red X ❌ = deployment failed (check logs)

## 🔄 Future Updates

To update your sites:
1. Make changes to your files
2. Commit: `git commit -m "Your update message"`
3. Push: `git push origin main`
4. GitHub Actions will automatically redeploy

## ⚙️ Workflow Features

- **Auto-deploy**: Triggers on push to main branch
- **Manual trigger**: Can be run manually from Actions tab
- **Concurrent protection**: Only one deployment at a time
- **Proper permissions**: Configured for secure deployment

## 🛠️ Troubleshooting

If deployment fails:
1. Check the Actions tab for error logs
2. Ensure GitHub Pages is set to "GitHub Actions" source
3. Verify the workflow file is in `.github/workflows/deploy.yml`
4. Check repository permissions allow Pages deployment

---

**Repository**: https://github.com/m-global/web
**Status**: Ready for deployment ✅


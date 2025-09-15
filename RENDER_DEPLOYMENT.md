
# 🚀 Deploy to Render.com (Free Tier)

## Quick Setup Instructions

### Step 1: Create Render Service
1. Go to [Render Dashboard](https://dashboard.render.com/)
2. Click "New +" → "Web Service"
3. Select "Build and deploy from a Git repository"
4. Connect to GitHub and select this repository: https://github.com/HarshilSiyani/sheet-app-daily-profits-app-0117-1757945976399
5. Use branch: **main**

### Step 2: Configure Service Settings
- **Name**: daily-profits-app
- **Build Command**: `npm install && npm run build`
- **Publish Directory**: `dist` (Vite build output directory)
- **Instance Type**: Free
- **Environment**: Static Site

**Note**: No start command needed for static sites - Render serves files directly from the build output.

### Step 3: Environment Variables
Add these environment variables in Render service settings:

```
NODE_ENV=production
NEXT_PUBLIC_SHEETAPPS_API_URL=http://localhost:3000/api/v1
NEXT_PUBLIC_SHEETAPPS_API_KEY=sk_b6b7f3764ef3401bb4d8d58123f30b61
NEXT_PUBLIC_SHEET_ID=1lq5RkslA1IkPRqgGHQDnhFJ3z1JOfXbHwRGs4VguBB0
NEXT_PUBLIC_SHEET_HEADERS=["StoreName","Date","Profit"]
NEXT_PUBLIC_SHEET_DATA_TYPES=["text","date","number"]
NEXT_PUBLIC_APP_NAME=Daily Profits App
NEXT_PUBLIC_APP_DESCRIPTION=Manage and track Daily Profits data with real-time Google Sheets integration
```

### Step 4: Deploy
- Click "Create Web Service"
- Wait for build and deployment (5-10 minutes)
- Your app will be live at: `https://your-service-name.onrender.com`

## 🔄 Auto-Deploy Setup (Optional)
Render automatically redeploys when you push to the **main** branch.

## 📞 Support
- Repository: https://github.com/HarshilSiyani/sheet-app-daily-profits-app-0117-1757945976399
- Generated: 9/16/2025
- SheetApps Support: [Contact Us](mailto:support@sheetapps.com)

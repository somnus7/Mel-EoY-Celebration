# Melbourne Branch End of Year Celebration

A Progressive Web App (PWA) for navigating the Melbourne Branch End of Year Celebration on the Lady Cutler cruise.

## Features

- 📱 **Works offline** - Cache all content for offline access
- 🏠 **Add to Home Screen** - Install as a native-like app on iOS & Android
- 🌙 **Light/Dark theme** - Toggle between themes
- 🌐 **Bilingual** - English and Chinese support
- ✅ **Checklist** - Track your packing items (saved to localStorage)
- ⏱️ **Countdown** - Live countdown to departure
- 📍 **Location** - Map link and transport info
- 🛡️ **Safety** - Important safety reminders

## Deployment to GitHub Pages

### Option 1: Quick Deploy

1. Create a new GitHub repository
2. Upload all files from this folder:
   - `EoY Party.html` (rename to `index.html` for easier access)
   - `manifest.json`
   - `sw.js`
   - `icons/` folder
   - `README.md`
3. Go to **Settings** → **Pages**
4. Under "Source", select **Deploy from a branch**
5. Select `main` branch and `/ (root)` folder
6. Click **Save**
7. Your site will be live at: `https://[username].github.io/[repo-name]/`

### Option 2: Using Git

```bash
# Initialize git in the EoY Party folder
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - EoY Party PWA"

# Add your GitHub repo as remote
git remote add origin https://github.com/[username]/[repo-name].git

# Push to main branch
git push -u origin main
```

Then enable GitHub Pages in repository Settings.

## File Structure

```
EoY Party/
├── EoY Party.html    # Main app (rename to index.html for GitHub Pages)
├── manifest.json     # PWA manifest
├── sw.js             # Service Worker for offline caching
├── README.md         # This file
└── icons/
    └── icon.svg      # App icon
```

## For Best Experience

Tell your colleagues to:

1. **iPhone users**: Open in Safari → Tap Share → "Add to Home Screen"
2. **Android users**: Open in Chrome → Tap menu → "Add to Home screen" or "Install app"

The app will show an install banner automatically on mobile devices.

## Local Storage

The app uses localStorage to persist:
- `partyLang` - Selected language (en/zh)
- `partyTheme` - Selected theme (light/dark)
- `partyChecklist` - Checked items
- `installBannerDismissed` - Whether install banner was dismissed

## Compatibility

- ✅ iPhone (Safari)
- ✅ Android (Chrome, Samsung Internet)
- ✅ Desktop browsers (Chrome, Edge, Firefox, Safari)

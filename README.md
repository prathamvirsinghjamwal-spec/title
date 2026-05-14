# 📓 TITLE STOCK

A Progressive Web App for notebook cover inventory management.

Track stock by seller and MRP, calculate stock value at landing cost, and get low-stock alerts — all offline, all on your device.

## Features

- 📝 **Stock entry** — Seller name, cover type (Notebook / A4), MRP, nags × notebooks-per-nag, landing cost
- 💰 **Stock value** — Auto-calculated from landing cost
- ⚠️ **Low stock alerts** — Separate thresholds for Notebook & A4 covers
- 🔍 **Search & filter** — By seller, MRP, type, or low-stock status
- 📤 **Export / Import CSV** — Backup your data anytime
- 📱 **Installable** — Works like a native app on Android & iOS
- 🌐 **Offline-first** — Works without internet after first load
- 🌓 **Dark mode** — Auto-switches with system theme

## Deploy to GitHub Pages

### Step 1 — Create a GitHub repo

1. Go to [github.com](https://github.com) and click **New repository**
2. Name it `title-stock` (or anything you like)
3. Make it **Public**
4. Click **Create repository**

### Step 2 — Upload these files

Easiest way (using the web UI):

1. On your new repo page, click **uploading an existing file**
2. Drag and drop ALL files from this folder (including the `icons` folder)
3. Click **Commit changes**

Or using Git from your computer:

```bash
git clone https://github.com/YOUR_USERNAME/title-stock.git
cd title-stock
# Copy all files from this folder into the repo
git add .
git commit -m "Initial commit"
git push
```

### Step 3 — Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, select **Deploy from a branch**
3. Select branch: **main** and folder: **/ (root)**
4. Click **Save**
5. Wait 1-2 minutes — your app will be live at:
   ```
   https://YOUR_USERNAME.github.io/title-stock/
   ```

## Install on Your Phone

### Android (Chrome)

1. Open the live URL on your phone
2. You should see an **"Install TITLE STOCK"** banner — tap **Install**
3. Or tap the **⋮** menu → **Install app** / **Add to Home screen**
4. Open it like any app from your home screen

### iPhone / iPad (Safari)

1. Open the live URL in Safari (not Chrome — must be Safari on iOS)
2. Tap the **Share** button (square with up-arrow)
3. Scroll down and tap **Add to Home Screen**
4. Tap **Add** in the top-right
5. Open it from your home screen

## Install on Desktop

1. Open the live URL in Chrome, Edge, or Brave
2. Click the install icon (⊕) in the address bar
3. Click **Install**

## How to Use

### Adding stock
1. Tap **+ New entry**
2. Enter seller, cover type, MRP
3. Enter nags received × notebooks made per nag
4. Enter landing cost per cover
5. Tap **Add to stock**

### Setting alert thresholds
1. Go to **Settings**
2. Set low-stock threshold (in nags) for Notebook & A4 covers separately
3. Tap **Save settings**

When any MRP-group falls at or below threshold, a red banner appears at the top.

### Backup
Tap **Settings → Export CSV** regularly to back up your data. You can re-import the CSV later or open it in Excel.

## Data Storage

All data is stored locally in your browser's **IndexedDB**. Nothing is sent to any server. Your inventory is private to your device.

⚠️ Clearing your browser data or uninstalling the app will erase your stock records — **export to CSV regularly**.

## File Structure

```
title-stock/
├── index.html           # Main app
├── styles.css           # Styling
├── app.js               # Application logic
├── service-worker.js    # Offline support
├── manifest.json        # PWA manifest
├── icons/
│   ├── icon-192.png
│   ├── icon-512.png
│   ├── icon-maskable-512.png
│   └── favicon.png
└── README.md
```

## License

Free to use, modify, and distribute.

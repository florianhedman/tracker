# 💪 Workout Tracker PWA

A personal workout tracker for bodyweight & weight training.  
No subscriptions. No accounts. Runs offline. Installable on Android.

---

## 🚀 Deploy to GitHub Pages (Step-by-Step)

### Step 1 — Create a GitHub repository

1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click the **+** button → **New repository**
3. Name it: `workout-tracker` (or anything you like)
4. Set it to **Public**
5. Click **Create repository**

---

### Step 2 — Upload the files

On your new repo page, click **uploading an existing file** (or drag & drop):

Upload **all** these files, keeping the folder structure:
```
index.html
manifest.json
sw.js
icons/
  icon-192.png
  icon-512.png
```

Click **Commit changes**.

---

### Step 3 — Enable GitHub Pages

1. Go to your repo → **Settings** tab
2. Scroll to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Choose branch: **main** — folder: **/ (root)**
5. Click **Save**

Wait ~60 seconds, then your app is live at:
```
https://YOUR-USERNAME.github.io/workout-tracker/
```

---

### Step 4 — Update the manifest (important!)

Edit `manifest.json` and update the `start_url` and `scope` to match your GitHub Pages path:

```json
"start_url": "/workout-tracker/",
"scope": "/workout-tracker/",
```

Also update `sw.js` — change the ASSETS list root path from `"/"` to `"/workout-tracker/"` and `"/index.html"` to `"/workout-tracker/index.html"`.

Commit and push the change.

---

### Step 5 — Install on Android

1. Open Chrome on your Android phone
2. Navigate to your GitHub Pages URL
3. Tap the **three-dot menu (⋮)** in the top right
4. Tap **"Add to Home screen"**
5. Tap **Add** — done! 🎉

The app icon appears on your home screen and opens fullscreen like a native app. It also works **offline** after the first load.

---

## 📱 Features

- **Log tab** — Add exercises, log sets with weight & reps, see your previous best
- **History tab** — Browse all past sessions, expand to see details, delete sessions
- **Progress tab** — Charts for any exercise: max weight, reps, or volume over time
- **Custom exercises** — Add your own exercises with the ★ button
- **Offline support** — Works without internet after first load
- **Data persists** — Stored locally on your device via localStorage

## 🏋️ Exercise Library

Includes 16 weight training + 16 bodyweight/calisthenics exercises out of the box.
Bodyweight exercises automatically hide the weight field.

---

*Built with React 18, no build tools required.*

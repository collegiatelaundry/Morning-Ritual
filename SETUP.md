# Get the Morning Ritual app onto your iPhone

The folder `morning-ritual-app` contains 6 files: `index.html`, `manifest.webmanifest`, `sw.js`, and three icon PNGs. Here's how to turn them into an app on your home screen — about 3 minutes.

## Step 1 — Put it on GitHub Pages

1. Go to [github.com/new](https://github.com/new) (sign in if needed).
2. Repository name: `morning-ritual` · set it to **Public** · click **Create repository**.
3. On the new repo page, click **uploading an existing file** (link in the quick-setup box).
4. Drag all 6 files from the `morning-ritual-app` folder into the upload area, then click **Commit changes**.
5. Go to **Settings → Pages** (left sidebar). Under *Build and deployment*, set **Source: Deploy from a branch**, **Branch: main / (root)**, click **Save**.
6. Wait ~1 minute, refresh the page — GitHub shows your site URL:
   `https://<your-username>.github.io/morning-ritual/`

## Step 2 — Install it on your iPhone

1. Open that URL in **Safari** on your iPhone (it must be Safari).
2. Tap the **Share** button (square with arrow).
3. Scroll down, tap **Add to Home Screen**, then **Add**.

Done. You'll get a sunrise icon on your home screen; it opens full-screen like a native app, works offline, remembers your check-marks for the day, resets fresh each morning, and quietly counts your streak of completed mornings.

## Notes

- Progress is stored on the device itself — iPhone and iPad each keep their own.
- Want to change a step later? Just ask me — I'll update `index.html` and you re-upload that one file (GitHub → open the file → pencil icon → paste → commit). The app updates on next launch or two.
- The same URL works on your iPad, desktop, anywhere.

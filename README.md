# AuraFlow OS 3.1 — 100% Offline Mind & Body Optimization Sanctuary

This bundle contains a **100% offline-ready**, zero-CDN web application with built-in **Screen Wake Lock**, **PWA Service Worker**, **7-Chakra Tibetan Singing Bowls**, **Formant Bija Vocal Chants**, and the **Global Instant Ambience Quick-Switcher**.

## Bundle Contents
- `index.html` — Complete application with Web Audio API synthesizers and Screen Wake Lock
- `styles.css` — Local offline stylesheet (zero external CDN requests)
- `manifest.json` — Android / PWA app manifest
- `sw.js` — Offline Service Worker cache
- `icon.svg` — Scalable vector app icon

---

## Step 1: Host on GitHub Pages
1. Create a new public repository on GitHub (e.g., `auraflow-os`).
2. Upload all 6 files (`index.html`, `styles.css`, `manifest.json`, `sw.js`, `icon.svg`, `README.md`) to the root of the repository.
3. Go to **Settings → Pages → Build and deployment**:
   - **Source:** Deploy from a branch
   - **Branch:** `main` / `/ (root)` → Click **Save**.
4. Wait ~60 seconds for your live HTTPS URL (e.g., `https://<username>.github.io/auraflow-os/`).

---

## Step 2: Generate the Android `.apk`

### Option A: PWABuilder (Recommended for GitHub Pages — Zero Coding)
1. Copy your live GitHub Pages URL (`https://<username>.github.io/auraflow-os/`).
2. Open **[pwabuilder.com](https://www.pwabuilder.com/)**, paste the URL, and click **Start**.
3. Click **Package for Stores → Android → Generate Package**.
4. Download the `.zip` containing your signed `.apk` (and `.aab` for Google Play).

### Option B: WebIntoApp / Capacitor (Direct Local Zip)
- **WebIntoApp:** Upload this exact `.zip` archive directly to `webintoapp.com` to build an offline `.apk`.
- **Capacitor:** Copy these files into Capacitor's `www/` directory and run `npx cap add android && npx cap sync && npx cap open android`.

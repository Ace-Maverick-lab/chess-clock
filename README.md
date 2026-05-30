# Chess Clock — Install Guide

## What's in this folder
- `index.html` — the app itself
- `manifest.json` — lets Android treat it as a real app
- `sw.js` — makes it work offline

## How to install on Android (no app store needed)

### Option A — Host on GitHub Pages (free, easiest)
1. Go to https://github.com and create a free account
2. Click **+** → **New repository** → name it `chess-clock` → **Public** → Create
3. Upload all 3 files (index.html, manifest.json, sw.js)
4. Go to **Settings → Pages** → Source: **main branch / root** → Save
5. After ~1 minute your URL will be: `https://YOUR-USERNAME.github.io/chess-clock`
6. Open that URL in Chrome on your Android phone
7. Tap the **⋮ menu → Add to Home Screen**
8. It installs like a real app and works fully offline!

### Option B — Use any web host
Upload the 3 files to any static web host (Netlify, Vercel, etc.)
and open the URL in Chrome on Android → Add to Home Screen.

### Option C — Local file (no internet needed after first load)
Copy the files to your phone and open `index.html` with Chrome.
Note: offline service worker won't work from file://, but the app itself will.

## How to play
- **First tap**: tap either panel to start — the opponent's clock begins
- **Your turn**: tap YOUR panel when you've made your move — starts the opponent's clock
- **Pause**: tap the Pause button in the middle bar
- **Reset**: tap Reset to start over
- **Settings**: change time control (bullet, blitz, rapid, custom + increment)

## Time controls included
| Name    | Time      |
|---------|-----------|
| Bullet  | 1 min     |
| Bullet  | 2 min + 1 sec |
| Blitz   | 3 min + 2 sec |
| Blitz   | 5 min     |
| Rapid   | 10 min ✓ default |
| Rapid   | 15 min + 10 sec |
| Classic | 30 min    |
| Long    | 60 min    |
| Long    | 90 min + 30 sec |
| Custom  | any minutes + increment |

## Features
- ✅ Full screen, one half per player
- ✅ White = white background, black text; Black = black background, white text
- ✅ Low-time warning (pulsing red at 30 seconds)
- ✅ Fischer increment support
- ✅ Screen stays awake during play
- ✅ 100% offline after first load

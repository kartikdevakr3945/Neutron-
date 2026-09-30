# Neutron by K.D App Developer (free, standalone)

A separate app that runs by itself. No Claude link and no server. The AI part uses Google's free Gemini API with YOUR free key.

## Files
- index.html : the whole app
- manifest.json, sw.js, icon-192.png, icon-512.png : make it installable like a real app

## Step 1: get a free key (no card needed)
1. Open https://aistudio.google.com/apikey and sign in with Google.
2. Create an API key and copy it. Keep it private.

## Step 2: put the app online for free (needed to install it on a phone)
Upload the 5 files (keep them together in one folder) to a free static host, for example Netlify (drag and drop), GitHub Pages, or Cloudflare Pages. You get an https link.
Do NOT type your key into any file. You enter it inside the app.

## Step 3: install on your phone
1. Open your link in Chrome.
2. Chrome menu (three dots) > Install app (or Add to Home screen).
3. Open Neutron from your home screen, tap the gear, paste your key, tap Save.
4. Tap a starter like "Business website" and build.

## Free limits (as of September 2026)
Google adjusts these often. Fast mode (gemini-3.5-flash-lite) allowed about 500 requests per day and Smart mode (gemini-3.6-flash) about 20 per day on the free tier. Check AI Studio for your live numbers. If you hit the limit, wait or use Fast.
Model names can change. If you see a "model not found" error, type the current name from ai.google.dev/gemini-api/docs/models into the Fast/Smart model ID boxes in Settings.

## Privacy and safety
- Your key is stored only in this browser on this device. Anyone who uses your phone or opens your browser data could read it. Don't enter it on shared devices.
- Every person who uses the link must use their OWN free key. Never publish a link with your key inside.
- On Google's free tier, your prompts may be used to improve Google's products. Don't put private or secret information in your prompts.
- If your key leaks, delete it in AI Studio and make a new one.

## Real APK (optional)
This installs as a home-screen app already. A Play Store style APK needs extra tools (for example the free PWABuilder website, or Android Studio on a computer).

## Status
Built and checked against a simulated Gemini service (streaming, cut-off detection, error handling). NOT yet tested with a real key, on a real host, or on your phone. Google's browser access rules could also block direct calls; if the first build fails, send me the exact message.

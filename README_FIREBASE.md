Short instructions — Firebase integration

- To keep Firebase credentials out of source control, create `env.js` from `env.js.example` and fill your real values.
- `env.js` is ignored by `.gitignore` and should define `window.__FIREBASE_CONFIG__`.
- The app will automatically use `window.__FIREBASE_CONFIG__` when present; otherwise it falls back to the inline config in `dashboard.html` so the site keeps working.

Steps:
1. Copy `env.js.example` → `env.js`.
2. Fill in your Firebase values.
3. Include `<script src="env.js"></script>` in your HTML before the app scripts.

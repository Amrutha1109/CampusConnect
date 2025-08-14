# CampusConnect — Frontend Starter (No Login, Safe, Student‑Friendly)

This is a **front‑end only** React + Tailwind starter for the CampusConnect idea:
- Pinterest/Instagram‑style feed (images, videos, text)
- Substack‑like writing (use Text post type)
- Anonymous **guest handles** via `localStorage` (no login)
- **Cross‑campus DMs** (local only, mock data)
- **Safety** placeholder: text keyword filter + media check stub

> Ready to push to GitHub and deploy to **Vercel**. No backend required.

## Running locally

```bash
# Node.js 18+
npm install
npm run dev
```

## Build & Deploy
- **Vercel**: Import the repo → it auto‑detects Vite → Deploy.
- **Netlify**: Build command `npm run build`, publish directory `dist`.

## Folder structure
```
/src
  /components       # UI pieces (Feed, Compose, DMs)
  /lib              # guest handle, moderation placeholders, mock data
  App.jsx           # Routes and pages
  main.jsx          # App entry
  styles.css        # Tailwind
index.html
package.json
tailwind.config.js
postcss.config.js
vite.config.js
```

## Safety / Moderation
This starter ships with very basic checks:
- `isTextSafe()` + `sanitizeText()` scrub offensive words
- `isMediaSafe()` always returns true (replace with Google Vision / Microsoft Content Moderator)

## Next steps (to make it production‑ready)
- Replace local DMs + posts with **Firebase / Supabase**
- Add **report/block** UI and moderator dashboard
- Replace media safety stub with real API calls
- Add image/video upload to cloud storage (Firebase Storage / S3)
- Add rate limits for posting & DMing
- Optional: campus‑verified roles (still without collecting personal info)

---

Made for rapid prototyping. Keep it kind, creative, and student‑friendly ✨

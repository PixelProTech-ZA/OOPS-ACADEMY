# OOPS ACADEMY

Funny disasters. Clever kids. Real learning. A PWA for Grade R to Grade 2 (English), by PixelProTech Solutions (Pty) Ltd.

## Files (all flat, no build step)
index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png, icon-maskable-512.png, apple-touch-icon.png, favicon.png

## Run / deploy
- Local: `python3 -m http.server 8080` then open http://localhost:8080 (service workers need http(s), not file://).
- GitHub Pages / Netlify / any static host: upload the folder as is. Paths are relative, so a repo sub-path works.
- Update: change `V` in sw.js (e.g. oops-academy-v2) so devices refresh the cache.

## Notes
- Child's name and grade are stored in localStorage on the device only. No accounts, no tracking.
- Voice uses the browser's speech synthesis (en-ZA if installed). Voice answers need SpeechRecognition (Chrome/Edge).
- More languages: add a UI and CONTENT block per language in index.html.
- Safety content should be reviewed by a child-safety professional before release. Childline SA: 116.

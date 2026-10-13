# OOPS ACADEMY

Funny disasters. Clever kids. Real learning. A PWA for Grade R to Grade 2 (English), by PixelProTech Solutions (Pty) Ltd.

## Files (all flat, no build step)
index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png, icon-maskable-512.png, apple-touch-icon.png, favicon.png

## Run / deploy
- Local: `python3 -m http.server 8080` then open http://localhost:8080 (service workers need http(s), not file://).
- GitHub Pages / Netlify / any static host: upload the folder as is. Paths are relative, so a repo sub-path works.
- Update: change `V` in sw.js (e.g. oops-academy-v2) so devices refresh the cache.

## Notes
- Child's first name and grade are stored in localStorage on the device only. No accounts, no tracking, nothing sent to PixelProTech.
- The "Say it" mic button uses the browser's speech recognition; Chrome sends that audio to Google. The in-app parent note says so.
- Class cheers are synthesized with the Web Audio API (no audio files). Parents can switch them off with the Cheers toggle.
- Each character has its own voice (pitch/rate in CHARS); Teacher Thandi reads questions and feedback.
- Microphone: one "Turn on microphone" prompt (the browser remembers Allow), then Auto-listen starts after each question is read; toggle on the home screen. Blocked or unsupported browsers get a plain explanation instead of a silent failure.
- No auto-advance timers: the child taps Next, so speech is never cut off and Back always works.
- Voice uses the browser's speech synthesis (en-ZA if installed). Voice answers need SpeechRecognition (Chrome/Edge).
- More languages: add a UI and CONTENT block per language in index.html.
- Safety content should be reviewed by a child-safety professional before release. Childline SA: 116.

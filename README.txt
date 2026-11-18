AUDIO LAB — OFFLINE ANALYZER PWA v0.1

Files:
- index.html: app screen
- styles.css: responsive mobile UI
- app.js: local file inspection, browser decoding, waveform, WAV export
- manifest.json: installable PWA metadata
- sw.js: offline app-shell cache
- icon.svg: app icon

IMPORTANT
A service worker and PWA installation generally require HTTPS (or localhost). Opening index.html directly from a file manager may allow basic analysis, but PWA installation/offline app-shell caching will not work reliably from file://.

EASIEST PHONE-ONLY DEPLOYMENT
1. Extract the ZIP on your phone.
2. Create a GitHub repository from the GitHub mobile website (or use an existing repository).
3. Upload all six app files to the repository root.
4. In repository Settings > Pages, deploy from the main branch and root folder.
5. Open the published HTTPS page in Chrome, wait for it to load once, then Chrome menu > Add to Home screen / Install app.
6. Open it once while online so the app shell is cached. Then test airplane mode.

Audio is processed in the browser. The app does not send selected audio to a server. WAV export is uncompressed PCM and may be much larger than the source file. Browser decoding support varies by device and codec.

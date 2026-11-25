# Agrichar website — app update

Replace index.html in the repository with this one, and add the six new files BESIDE it
(same folder as index.html, not inside assets/):

- index.html            (replaces the old one)
- manifest.webmanifest  (new)
- sw.js                 (new)
- icon-192.png          (new)
- icon-512.png          (new)
- icon-maskable-512.png (new)
- apple-touch-icon.png  (new)

The assets/ folder is unchanged — keep yours as it is. Nothing in the design changed.

## What is new
1. Installable app. Over https (GitHub Pages is https) Chrome and Edge show an "Install app"
   button in the header; Android also offers "Add to home screen". On iPhone/iPad the button
   opens a short sheet explaining Share -> Add to Home Screen, which is the only way Safari
   allows. It opens full screen with the Agrichar logo as its icon, rotates freely, and the
   pages still open when the signal drops.
2. The site now starts in ENGLISH, in the browser and inside the installed app. The ع button
   switches to Arabic and the choice is remembered in the browser. index.html?lang=ar opens
   straight in Arabic.

If you replace index.html later and an installed app still shows the old page, open it once
with an internet connection: pages are fetched from the network first and fall back to the
cache only when offline.

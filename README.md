# Twitch Chat Reactive Overlay

This repository hosts a simple Twitch chat reactive PNG swapper overlay you can use in OBS.

## How to use

1. Upload your PNG images somewhere accessible online (e.g., Imgur, Cloudinary).

2. Open the URL with query parameters for your Twitch channel and image URLs, for example:

https://yourusername.github.io/chat-reactive-overlay/chat_reactive.html?channel=YourTwitchName&idle=https://i.imgur.com/abc.png&reacting=https://i.imgur.com/xyz.png&duration=1500

https://nuckolpunch.github.io/twitch-chat-reactive/chat_reactive.html?channel=jonbrimstone&idle=https://i.imgur.com/WryOIK9.png&reacting=https://i.imgur.com/v6c7Ext.png&duration=2000


- `channel` — Your Twitch channel name (no `#`)
- `idle` — URL to your idle PNG image
- `reacting` — URL to your reacting PNG image
- `duration` — Optional. How long to show the reacting image in milliseconds (default 1500)

3. Add this URL as a **Browser Source** in OBS.

## Notes

- This overlay connects anonymously to Twitch chat.
- No backend server required; this is fully client-side.
- Make sure your images are publicly accessible via HTTPS.

---

Made for easy Twitch overlays. Enjoy!

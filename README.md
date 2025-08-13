# Chat Reactive Overlay for Twitch
A lightweight browser-based Twitch chat reactive PNG overlay for OBS.  
Switches between an idle image and talking animation when chat messages arrive.
---
## Available Overlay Versions
### 1) Original (chat_react.html)
Supports only `idle` and one `reacting` image with the inclusion of `duration` and `speed`
### 2) Full Featured (chat_reactive_advanced.html)  
Supports all parameters including special question/exclaim reactions, animation speed, random mode, talk delay, etc.  
Best for advanced customization.
### 3) Simple (chat_reactive_simple.html)  
Supports: `idle`, `reacting`, `duration`, `speed`, `random`  
No special reactions (`question` or `exclaim`). Easier URLs and setup.
### 4) Minimal (chat_reactive_minimal.html)  
Supports only `idle` and one `reacting` image (no animation, no timing params).  
Good for beginners or quick testing.
---
## How to Use
Upload your PNG images somewhere with direct URLs (e.g., Imgur) and build a URL like this to use in OBS as a Browser Source.
```
https://nuckolpunch.github.io/twitch-chat-reactive/chat_reactive.html?channel=MyTwitchName&idle=IDLE_URL&reacting=eacting=REACT_URL&duration=2000
```
```
https://nuckolpunch.github.io/twitch-chat-reactive/chat_reactive.html?channel=nuckolpunch&idle=https://i.imgur.com/WryOIK9.png&reacting=https://i.imgur.com/v6c7Ext.png&duration=2000
```
### Full Featured Example URL
```
https://nuckolpunch.github.io/twitch-chat-reactive/chat_reactive_advanced.html?channel=MyTwitchName&idle=IDLE_URL&reacting=TALK1,TALK2&question=QUES1,QUES2&exclaim=EXCL1,EXCL2&duration=1500&speed=150&random=true&talkdelay=3000
```
### Simple Example URL
```
https://nuckolpunch.github.io/twitch-chat-reactive/chat_reactive_simple.html?channel=MyTwitchName&idle=IDLE_URL&reacting=TALK1,TALK2&duration=1500&speed=150&random=true
```
### Minimal Example URL
```
https://nuckolpunch.github.io/twitch-chat-reactive/chat_reactive_minimal.html?channel=MyTwitchName&idle=IDLE_URL&reacting=REACT_URL
```
---
## Notes on Image URLs
- Use direct PNG links (ending in `.png`).  
- Imgur example: right-click image → Copy Image Address (not page URL).  
- Users should host and supply their own images to customize fully.
---
## OBS Setup
1. Add a Browser Source in OBS.  
2. Paste your overlay URL with your images and parameters.  
3. Set the size to your PNG resolution or your desired layout size.  
4. Enable *Shutdown source when not visible* and *Refresh browser when scene becomes active* (recommended).  
5. Enjoy your chat reactive avatar!
---
## License

MIT License

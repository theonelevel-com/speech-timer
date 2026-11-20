# Speech Timer

**Toastmasters Speech Timing Tool — by Westlake Toastmasters**

A web-based speech timer for Toastmasters meetings. Works in any browser, installs as a standalone app on your phone, and runs offline.

🌐 **Live app:** [https://theonelevel-com.github.io/speech-timer/](https://theonelevel-com.github.io/speech-timer/)

📖 **Help Guide:** [HELP.md](./HELP.md), covering how to use the timer, install it as an app, and more

🎥 **Timing on Zoom:** [Zoom Speech Timer Background](./ZOOM-BACKGROUND.md)

---

## Version

**v1.5.3** — Westlake Toastmasters

---

## Features

- **Colour-coded timing** — screen changes from White → Green → Yellow → Red as the speaker progresses
- **Preset speech types** — Standard (5–7 min), Ice Breaker (4–6 min), Table Topics (1–2 min), Evaluation (2–3 min)
- **Custom timing** — set your own Green / Yellow / Red thresholds in m:ss format
- **Count down to red** — optional setting; counts down to the red time, then shows overtime as -0:01, -0:02…
- **Competition mode** — colour only, with the time hidden from the speaker
- **Demonstration mode** — cycles through all colours in 20 seconds for testing
- **Overtime alarm** — optional repeating audio alarm 30 seconds after red (every 15s)
- **Overtime flashing** — red/white screen flash 1 minute past red (epilepsy-safe 1 Hz frequency, can be disabled)
- **Speech log** — records speaker name, type, time, and over/within status with editable fields
- **Start / Pause / Finish / Reset** controls with confirmation dialog
- **Fully offline** — works without an internet connection once installed

---

## Install as an App

The timer installs on iPhone, iPad, Android and desktop, and works offline once installed. Step-by-step instructions are in the **[Help Guide → Install as an App](./HELP.md#install-as-an-app)**.

---

## Host It Yourself (GitHub Pages)

1. Fork or clone this repository
2. Go to **Settings → Pages**
3. Under "Source", select **Deploy from a branch**
4. Choose **main** branch, root folder `/`
5. Click **Save**
6. Your timer will be live at `https://YOUR-USERNAME.github.io/speech-timer/`

---

## Files

| File | Purpose |
|------|---------|
| `index.html` | The complete timer app (single HTML file, no build step) |
| `HELP.md` | Help Guide (also opened by the Help button in the app) |
| `ZOOM-BACKGROUND.md` | Using the timer as a Zoom camera or background with Meld Studio (Mac and Windows) |
| `manifest.json` | PWA manifest — tells browsers this is an installable app |
| `sw.js` | Service worker — caches everything for offline use |
| `icons/` | App icons for home screen (192px, 512px, 180px) |

---

*Powered by The Club with Heart*
♥️
*[www.westlaketoastmasters.co.za](https://www.westlaketoastmasters.co.za)*

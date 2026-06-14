# RepTimer 🏋️

A free, no-install workout interval timer that runs in any browser. No ads, no subscriptions, no account needed — just open the file and go.

---

## 📱 Add to your iPhone home screen (looks and feels like an app)

RepTimer is designed to live on your iPhone home screen with its own icon — no App Store required.

1. Open the RepTimer link in **Safari** (must be Safari — Chrome and Firefox won't work)
2. Tap the **Share button** at the bottom of the screen (the box with an arrow pointing up)
3. Scroll down in the share sheet and tap **"Add to Home Screen"**
4. The name will already say **RepTimer** — tap **Add** in the top right corner

It will appear on your home screen with a green clock icon, just like any other app. Tapping it opens RepTimer full screen with no browser address bar.

> **Tips for the best experience:**
> - Keep your screen on while the timer is running — iOS pauses browser timers when the screen locks
> - Make sure your iPhone's mute switch is off (no orange dot) so you can hear the audio cues
> - If you update the app and want the new icon, delete the shortcut and re-add it

---

## What it does

You set three things:

- **Reps** — how many work intervals you want
- **Work interval** — how long each rep lasts (hours, minutes, or seconds)
- **Rest period** — how long to rest between reps (hours, minutes, or seconds)

RepTimer calculates the total session length automatically, then counts you through every rep with distinct audio cues so you can keep your eyes off the screen while you train.

## Audio cues

Each event has a unique sound so you always know what's happening:

| Event | Sound |
|---|---|
| Work starts | Three sharp ascending beeps (punchy, high energy) |
| Rest starts | Two long descending tones (calm, relaxed) |
| During rest | Gentle looping pentatonic melody — plays until the next rep begins |
| Session complete | Rising fanfare arpeggio |

## How to use

### Option 1 — Open locally
1. Download `index.html`
2. Open it in any browser (Chrome, Safari, Firefox, Edge)
3. Set your reps, work interval, and rest period
4. Tap **Start**

### Option 2 — Host on GitHub Pages (share a link with anyone)
1. Fork this repo
2. Go to **Settings → Pages**
3. Set source to the `main` branch, root folder
4. Your timer will be live at `https://<your-username>.github.io/<repo-name>/`

## Features

- Works on desktop, tablet, and mobile
- Dark mode support (follows your system setting)
- Session log with timestamps
- Pause and resume mid-session
- Total session duration shown before you start
- No internet connection required after the page loads (except for the icon font)

## Limitations

- Browser timers pause when the screen locks on iOS — keep your screen on while using it, or use Low Power Mode off
- Audio requires a tap/click to start (browser autoplay policy) — the Start button handles this automatically

## Tech

Plain HTML, CSS, and JavaScript. No frameworks, no build step, no dependencies beyond a Tabler Icons CDN link for the button icons. The audio is generated entirely with the Web Audio API — no audio files to download.

## Contributing

Issues and pull requests welcome. Planned improvements:

- [ ] Save last-used settings in localStorage
- [ ] Named workout presets
- [ ] Spoken countdown ("3… 2… 1… Go!")
- [ ] Apple Watch / wearable vibration support via PWA

## License

MIT — free to use, modify, and share.

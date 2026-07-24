# Deep Focus — Pomodoro + Music Player

A single tab you can leave open while you study: a configurable Pomodoro timer paired with a music player that plays files straight from your own computer. No need to build anything, just one `HTML` file that runs entirely in the browser.

Orignally started as a way to learn web development, now it has been remade!

---

## Features

- **Configurable Pomodoro timer** - You can change focus length, short break, long break, cycles before a long break, auto-start next session, and an optional end-of-session chime, all saved between visits.
- **Your own music, locally** - The previous version used to be that you need to have your `MP3s` be in the root folder of the project, now you can choose a folder or drag one onto the page. `.mp3` files are found automatically, including in subfolders.
- **Daily focus progress** - Stats is key, so I made them persists across reloads (and resets automatically at midnight).
- **Keyboard shortcuts** - Everything is easier with shortcuts! `Space` play/pause, `←` / `→` skip 10 seconds.
- **Works offline** - The `HTML` file can work on its own once the page has loaded. Zero reliance on API calls or external fonts.
- Tokyo Night color theme. The **GOAT** of all color themes

---

## Running it locally

Just open `index.html` in a browser. That's it. There is no need to install or build. You don't need to re-enact that one famous quote.

If you'd rather serve it over `http://`, any static server works:

```bash
python3 -m http.server
# then visit http://localhost:8000
```

---

## GitHub Pages

There is a GitHub Pages version of this if you would rather have it ready to use without any hinderance. Click the link that is below the description of this repository or check it out [here](https://xia-qi2450.github.io/Deep-Focus/).

---

## Project structure

```file
.
├── index.html   # the entire app: markup, styles, and logic in one file
└── README.md
```

---

## Browser support

Just any modern browser should work (recent Chrome, Firefox, Safari, or Edge) for the File API (folder picking), the native `<dialog>` element (settings panel), and the Web Audio API (end-of-session chime). Of course if there are unsupported elements, they will be handled by using alternatives.

---

## Privacy

Dude, its a normal `HTML` file, there will definitely be no data collection of any kind. All settings are stored in your browser's `LocalStorage` so there is no need to collect any info.

---

## License

MIT because open-source and free to use is the best way forward.

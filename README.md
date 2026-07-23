# A Special Delivery 💌

Night sky with shooting stars → postman walks in → lilies handed over →
envelope opens with a sparkle burst → typewriter letter (music plays once,
right as it opens) → live "since we met" timer → Spotify/TikTok/Final Note
→ ending.

Everything — including your song — lives inside **one self-contained
`index.html`**. There's no `assets/` folder, no separate `music.mp3` to
misplace: the audio is embedded directly in the page. Just three files:

```
A-Special-Delivery/
├── index.html   all scenes + your song, embedded
├── style.css    every color and animation
└── script.js    EDIT THIS — your letter, date, and links live here
```

## 1. Edit your content

Open `script.js`. Everything personal is in one block at the very top:

```js
const LETTER_TEXT = `...`;   // <-- your real letter goes here
const START_DATE = new Date('2023-04-19T00:00:00');   // already set
const SPOTIFY_URL = '...';   // already set to your playlist
const TIKTOK_URL = '...';    // already set
const FINAL_NOTE = `...`;    // <-- short note shown by the "Final Note" button
```

The only thing left to do is replace `LETTER_TEXT` and `FINAL_NOTE` with
your real words.

## 2. Publish on GitHub Pages

1. Create a new **public** repo.
2. Upload all three files — `index.html`, `style.css`, `script.js` —
   straight into the repo root.
3. Settings → Pages → Source: `Deploy from a branch`, branch `main`,
   folder `/ (root)`. Save.
4. Your site is live at `https://<your-username>.github.io/<repo>/`

## Notes

- Music plays once, starting the instant the envelope opens, and fades
  out when you leave the letter or open the Final Note.
- A small music note button (top-right) lets her replay the song anytime.
- Tested end-to-end with no console errors.

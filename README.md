# Three Questions — Leo Tolstoy
### A Realm of English (B) Selection | Interactive Educational PWA

A complete offline-first Progressive Web App for Bengali-medium Class IX–XII students studying Leo Tolstoy’s short story **Three Questions**.

## Features

- **Complete textbook text** (Pages 168–172) with original footnotes
- **Clickable vocabulary** with Bengali meaning, pronunciation & part of speech
- **Paragraph-level Bengali translations** (toggleable)
- **Human-like reading** via Web Speech API (browser TTS) + ready structure for future human MP3 + word timings
- **Synchronized paragraph highlighting** while listening
- **Three modes**: Read · Listen · Learn
- **Vocabulary panel** with search, favourites, learned status (localStorage)
- **Interactive Quiz** (story comprehension + vocabulary)
- **Progress dashboard** (words learned, paragraphs read, quiz score, streak)
- **Settings**: font size, line spacing, light/dark/sepia/high-contrast, reduced motion
- **Bookmarks**, global search, print-friendly styles
- **PWA**: installable, works offline after first visit
- **Mobile-first** with sticky bottom player and hamburger nav

## Files

| File | Purpose |
|------|---------|
| `index.html` | Complete single-file application |
| `manifest.json` | PWA manifest |
| `sw.js` | Service worker (cache-first) |
| `README.md` | This file |

## How to Deploy (GitHub Pages)

1. Go to **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / **root**
4. Save

Then visit: `https://pbwsantu-collab.github.io/three-questions-tolstoy-pwa/`

## Adding Human Narration Later

The reading engine already supports:

```js
const audioLessons = {
  "p001": "audio/three-questions/p001.mp3",
  // ...
};

const timings = {
  "p001": [
    { word: "It", start: 0.00, end: 0.20 },
    // ...
  ]
};
```

If an MP3 is missing the app automatically falls back to browser TTS.

## Target Learners

Bengali-medium students (Class IX–XII) learning English literature.

**Core loop:** SEE → HEAR → CLICK → UNDERSTAND → REPEAT → PRACTISE → MASTER

---

Built as a self-contained educational digital textbook.

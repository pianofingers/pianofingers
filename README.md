# Piano Fingers

**A free, interactive piano scale & chord fingering tool.**

Piano Fingers helps you learn the correct left- and right-hand fingering for piano scales and chords, right on a playable, visual keyboard. No sign-up, no install, just open it and play.

🔗 **Live app:** [pianofingers.github.io](https://pianofingers.github.io/)
📦 **Repo:** [github.com/pianofingers/pianofingers.github.io](https://github.com/pianofingers/pianofingers.github.io)

---

## What it does

- **Scales**: every key, major and minor scales, pentatonic scales, blues, modal and exotic scales, with hand-verified fingering (cross-checked against published fingering charts) and heuristic fingering for the more unusual scales.
- **Chords**: triads, 6ths, 7ths, sus2/sus4, diminished, augmented and more, with every inversion, in Chord mode.
- **Interactive keyboard**: highlights the notes and finger numbers for the current key, scale, or chord, with circled numbers showing exactly where the thumb tucks under or crosses over.
- **Left / Right / Both hands**: see and hear either hand on its own, or both together at the correct relative pitch.
- **Audio playback**: hear the scale or chord played back with real-time synthesis, adjustable tempo (20 to 260 BPM), and an optional "Increase" mode that gradually speeds up each time it loops, a simple built-in speed trainer.
- **Quick Scales / Quick Chords**: a fast-access grid to jump straight to a scale or chord type.
- Fully responsive: desktop, tablet, and mobile landscape (portrait is intentionally blocked with a rotate prompt, since the keyboard needs the width).

## Tech

Piano Fingers is a **single self-contained HTML file**. No build step, no dependencies, no backend.

- Vanilla HTML / CSS / JavaScript
- Audio generated live with the Web Audio API (no sample files)
- All UI (keyboard, hand diagrams, controls) rendered as inline SVG / DOM, built at runtime from a plain data model of scale and chord formulas

## Running it locally

Since it's one file, there's nothing to install:

1. Download `index.html`
2. Open it directly in any modern browser

That's it. To host it, just deploy `index.html` as-is (GitHub Pages, Netlify, Cloudflare Pages, or any static host).

## Project structure

```
index.html   # everything: markup, styles, and app logic in one file
```

Everything is organised in clearly commented sections inside the file:
- Scale and chord data (offset formulas relative to the root)
- Fingering tables and heuristics
- Keyboard rendering (SVG)
- Audio engine (Web Audio API)
- UI wiring (controls, panels, modal)

## Known limitations

- Chord fingering is simplified (root-position style fingering applied across inversions), not a fully worked-out fingering for every possible voicing.
- Exotic/heuristic scale fingerings are generated from a consistent rule set rather than individually verified against a teaching source, unlike the major/minor scale tables.

## Support

Piano Fingers is free to use and built independently. If you find it useful, consider [supporting the project](https://donate.stripe.com/00w8wQbZr6Wk3jxaS24sE0d) or reaching out at **pianofingersapp@gmail.com** with feedback, bug reports, or feature requests.

## License

_Add your chosen license here (e.g. MIT); none specified yet._

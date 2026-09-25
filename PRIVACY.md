# Privacy — Ink Clock (Chrome)

**Last updated:** 2026-09-24

Ink Clock is a Chrome extension that tells the time with a copyright-free line from a book, or an original voice line written for this clock. It does not require an account and does not ask for your name, email, or address.

## What the extension uses

- **Settings you choose**, saved with Chrome’s `storage` API on this device only: paper look, text size, quote source, date and time formats, time zone, page-turn interval, layout and colors, read-aloud options, and sound options. The current page (minute and line) may also be saved so the next open can keep the same passage until the schedule turns.
- **The current time**, taken from this device (or from the time zone you pick).
- **Bundled text** for the copyright-free books file (`books/pd-times.txt`) and the original voice files (`voices/`). Those files ship inside the extension and are not uploaded anywhere.
- **Text-to-speech**, using Chrome’s built-in `tts` API when you tap Read or when automatic read-aloud is on. Speech stays on the device.
- **Sound effects**, synthesized in the page with the Web Audio API. No sound files are downloaded.

## What the extension does not do

- No advertising.
- No sale of data.
- No account or sign-in.
- No purchases.
- No tracking or analytics SDKs.
- **No network requests for quotes.** The extension does not contact literature-clock hosts or other quote APIs.

## Quotes

- **Books:** lines gathered for use under Canada’s public-domain rules (authors who died in 1971 or earlier, and related checks used by this project). An empty minute may show the nearest earlier line.
- **Voices (Yoda, Pirate, Teacher, and the rest):** original lines written for this clock. They are not quotations from films or books.

## Contact

[Markus van Kempen](https://markusvankempen.github.io/) · [markus.van.kempen@gmail.com](mailto:markus.van.kempen@gmail.com) · [github.com/markusvankempen](https://github.com/markusvankempen)

No bug too small, no syntax too weird.

Published privacy policy for the Chrome Web Store:

```
https://raw.githubusercontent.com/markusvankempen/ink-clock/main/PRIVACY.md
```

Docs home: https://github.com/markusvankempen/ink-clock

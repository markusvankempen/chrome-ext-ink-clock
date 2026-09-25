# Chrome Web Store — Ink Clock

Paste-ready listing text and a checklist for submission. Package only this `chrome` folder (`manifest.json` at the zip root).

## Listing fields

### Name

```
Ink Clock
```

### Summary (≤ 132 characters)

```
A copyright-free clock of books. Every new tab tells the time with a public-domain line — or an original voice.
```

### Detailed description

```
Ink Clock tells the time with a sentence from a book that mentions that exact minute.

Open a new tab (or the toolbar popup) and you get a cream page with the date, the time, the line, and the credit. Tap Another line for a different passage. Tap Read to hear the sentence, then the title and author. The clock phrase stays on the page and is not spoken.

All book quotations are copyright-free in Canada (bundled with the extension). There is no live feed of modern novels.

Quote sources
• Books — public-domain and Canada-clear lines; an empty minute shows the nearest earlier line
• Surprise me — mixes those books with original voices
• Voices — Yoda, Pirate, Teacher, and more (original pastiche, not film or book quotations)

Customize the page
• Paper looks: Paper, Snow, Sepia, Midnight, and others
• Text size, layout, and colors
• Date and time formats, 12- or 24-hour, and time zone
• Page turn every 1, 5, 10, 15, 30, or 60 minutes (default 5)

Sound (optional)
• Read aloud when you tap Read, or automatically when the page turns
• Optional page-turn or themed sound effects, and an hour chime

Ink Clock does not require an account, does not show ads, and does not sell your data. Settings stay on this device. Quotes are bundled — the extension does not call remote quote servers. See the privacy policy linked on this listing.

Related: the Alexa skill Ink O’Clock (say “ink clock”) is a separate product.
```

### Category

**Productivity**

### Language

English

### Single purpose

```
Provides a literature clock: the new tab and toolbar popup display the current time as a copyright-free literary quotation (or an original themed line) for that minute, with optional read-aloud and sound.
```

### Permission justifications

**storage**  
```
Saves the user’s theme, quote source, schedule, time zone, read-aloud, and sound preferences on this device.
```

**tts**  
```
Reads the quote aloud when the user taps Read or enables automatic read-aloud. Uses Chrome’s built-in text-to-speech.
```

No host permissions are requested.

### Privacy policy URL

```
https://raw.githubusercontent.com/markusvankempen/ink-clock/main/PRIVACY.md
```

Public docs repo: https://github.com/markusvankempen/ink-clock

## Screenshots

Capture at least one (1280×800 or 640×400):

1. New tab — Page with a clear book quote  
2. Theme tab — Quote sources and paper looks  
3. Sound tab — read-aloud and sound effects  
4. Optional: popup and Midnight look  

## Package

From the literature-clock project root:

```bash
python3 scripts/package_chrome.py
```

That syncs `voices/` and `books/`, then writes:

```
dist/ink-clock-chrome.zip
```

Upload that zip in the Chrome Web Store developer dashboard (**Package** → upload a new package). The zip root contains `manifest.json` (not a nested `chrome/` folder).

Manual alternative:

```bash
python3 scripts/sync_chrome_quotes.py
cd chrome
zip -r ../dist/ink-clock-chrome.zip . -x "*.DS_Store"
```

## Checklist

- [ ] Version bumped in `manifest.json` for each upload  
- [ ] Icons 16 / 48 / 128 present  
- [ ] Privacy policy URL live  
- [ ] Permission justifications filled  
- [ ] Screenshots uploaded  
- [ ] Smoke-test: new tab, Another line, Read, Surprise me, Sound → Try the sound  
- [ ] Contact email on the developer dashboard monitored  

## Version

Current package version: see `manifest.json` (`1.1.0` = copyright-free only, no remote quote hosts).

## Author

[Markus van Kempen](https://markusvankempen.github.io/) · [markus.van.kempen@gmail.com](mailto:markus.van.kempen@gmail.com)

No bug too small, no syntax too weird.

# Chrome Web Store — fill-in guide for Ink Clock

Use this document while completing **Store listing → Product details**.  
Assets live in `dist/store-listing/` (also copied under this folder’s sibling paths below).

**Privacy policy URL (required):**  
https://raw.githubusercontent.com/markusvankempen/ink-clock/main/PRIVACY.md  

**Docs / homepage:**  
https://github.com/markusvankempen/ink-clock  

**Support URL (same as homepage is fine):**  
https://github.com/markusvankempen/ink-clock/issues  

**Author:** [Markus van Kempen](https://markusvankempen.github.io/) · [markus.van.kempen@gmail.com](mailto:markus.van.kempen@gmail.com)

No bug too small, no syntax too weird.

---

## Product details (all languages — English)

### Title from package

```
Ink Clock
```

*(Comes from `manifest.json` → `name`. Do not change in the form.)*

### Summary from package

```
A new-tab clock that tells the time with a line from a book.
```

*(Comes from `manifest.json` → `description`. Under 132 characters. Rebuild the zip after changing it.)*

### Description

Paste this into the **Description** box (focus on what it does and why install it):

```
Ink Clock turns every new tab into a quiet page from a book.

Instead of a blank tab or a busy dashboard, you see the date, the time, and a sentence that mentions that exact minute—then the title and author underneath. Tap Another line for a different passage. Tap Read to hear it aloud. The clock phrase stays on the screen; only the literary line is spoken.

Why install it
• A calmer new tab—cream paper, clear type, no ads or feeds
• Works offline for quotes (everything ships inside the extension)
• Twelve paper looks, from Paper and Sepia to Midnight and Ocean
• Optional read-aloud with your Chrome voices, and soft page-turn or themed sounds
• Pick a voice for the hour: Pirate, Teacher, Detective, and more (original lines written for this clock)
• Surprise me mixes classic book lines with those voices
• Set how often the page turns (1 to 60 minutes), 12- or 24-hour time, and your time zone

How it works
Open a new tab or click the Ink Clock icon. The footer has Page, Theme, Quote, Time, and Sound. Theme chooses the paper look and the quote source. Sound controls reading and optional effects.

Book lines are drawn from works that are free to use in Canada. The extension does not pull a live feed of modern novels and does not need an account.

Related: the Alexa skill Ink O’Clock (say “ink clock”) is a separate product.
```

Character count: well under 16,000.

### Category

```
Productivity
```

*(Alternative if the dashboard suggests it: Lifestyle.)*

### Language

```
English
```

---

## Graphic assets — what to upload

All files are **JPEG or 24-bit PNG (no alpha)**. Paths relative to the literature-clock project:

| Form field | Size | File |
|---|---|---|
| **Store icon** | 128 × 128 | `dist/store-listing/store-icon-128.png` |
| **Screenshot 1** (required) | 1280 × 800 | `dist/store-listing/screenshot-1-page.png` |
| **Screenshot 2** | 1280 × 800 | `dist/store-listing/screenshot-2-theme.png` |
| **Screenshot 3** | 1280 × 800 | `dist/store-listing/screenshot-3-sound.png` |
| **Screenshot 4** | 1280 × 800 | `dist/store-listing/screenshot-4-midnight.png` |
| **Screenshot 5** | 1280 × 800 | `dist/store-listing/screenshot-5-pirate.png` |
| **Small promo tile** | 440 × 280 | `dist/store-listing/promo-small-440x280.png` |
| **Marquee promo tile** | 1400 × 560 | `dist/store-listing/promo-marquee-1400x560.png` |

Screenshot order suggestion:

1. Page — main quote view (best first impression)  
2. Theme — paper looks and quote sources  
3. Sound — read-aloud and effects  
4. Midnight — dark look  
5. Pirate — original voice example  

**Global promo video:** leave blank (optional).

---

## Additional fields

### Official URL

```
None
```

Or add `github.com/markusvankempen/ink-clock` in Search Console later if you want “Official URL”.

### Homepage URL

```
https://github.com/markusvankempen/ink-clock
```

### Support URL

```
https://github.com/markusvankempen/ink-clock/issues
```

### Mature content

```
No
```

*(Unless the store asks you to confirm otherwise—this item is not mature-directed.)*

---

## Test instructions (Chrome Web Store review)

**Credentials:** leave Username and Password **blank**. No account or login is required.

**Additional instructions** (paste below):

```
No login or test account is needed.

1. Install the extension from the uploaded package.
2. Open a new tab. The page should show the current time as a highlighted passage from a book (or a themed voice line), with title and author below.
3. Click the Ink Clock toolbar icon to open the popup — it shows the same clock in a compact view.
4. On the new-tab page, open Settings (gear). Try:
   - Theme: switch paper look and a voice (e.g. Books, Yoda, Pirate).
   - Quote source: Books vs a themed voice; confirm the line style changes.
   - “Another line” / refresh: a different line for the same minute appears.
   - Read: Chrome TTS reads the quote aloud.
   - Optional: enable automatic read-aloud or sound effects and wait for a page turn.
5. Change schedule or time zone if desired; settings persist after closing and reopening the tab.

Expected: works offline for quotes (bundled files only); no sign-in; no remote quote API.
```

---

## Data usage (Privacy practices form)

**Leave every box unchecked.** Ink Clock does not collect any of the listed user data now or in future plans described in the privacy policy.

| Category | Select? | Why |
|---|---|---|
| Personally identifiable information | **No** | No name, email, age, or ID |
| Health information | **No** | Not used |
| Financial and payment information | **No** | No purchases or payments |
| Authentication information | **No** | No account, password, or PIN |
| Personal communications | **No** | No email/chat access |
| Location | **No** | Time zone is a setting the user picks (or “this device”); it is not collected or sent as location data |
| Web history | **No** | No history permission; does not read browsing history |
| User activity | **No** | No analytics, click tracking, or keylogging |
| Website content | **No** | Does not read other sites’ pages |

Settings (theme, schedule, quote source, sound) stay in Chrome’s **local storage on the device**. They are not uploaded to your servers (there are none for this extension).

If the form also asks these follow-ups (wording varies):

| Question | Answer |
|---|---|
| Do you sell user data to third parties? | **No** |
| Do you use or transfer user data for purposes unrelated to the item’s single purpose? | **No** |
| Do you use or transfer user data to determine creditworthiness or for lending? | **No** |
| Is all user data encrypted in transit? | **Not applicable** (no user data is transmitted) — if forced to choose and “N/A” is missing, pick the option that matches “we don’t collect / don’t transfer” |
| Do you collect remote code? | **No** |

Certify that the disclosures match the privacy policy:  
https://raw.githubusercontent.com/markusvankempen/ink-clock/main/PRIVACY.md

---

## Privacy (Distribution / Privacy practices)

When the dashboard asks for a privacy policy:

```
https://raw.githubusercontent.com/markusvankempen/ink-clock/main/PRIVACY.md
```

**Single purpose (if asked):**  
Provides a literature clock: the new tab and toolbar popup show the current time as a line from a book (or an original themed voice), with optional read-aloud and sound.

**Permission justifications:**

- **storage** — Saves theme, quote source, schedule, time zone, read-aloud, and sound preferences on this device.  
- **tts** — Reads the quote when the user taps Read or enables automatic read-aloud (Chrome built-in speech).  

No host permissions.

---

## Package to upload

```bash
python3 scripts/package_chrome.py
```

Upload: `dist/ink-clock-chrome.zip`  

Current package version: see `chrome/manifest.json` (bump for every new upload).

---

## Quick checklist

- [ ] Title / summary match the package (reload zip after editing `manifest.json`)  
- [ ] Description pasted  
- [ ] Category = Productivity, Language = English  
- [ ] Store icon 128×128  
- [ ] At least one screenshot (prefer all five)  
- [ ] Small + marquee promo tiles  
- [ ] Homepage + Support URLs  
- [ ] Privacy policy URL  
- [ ] **Data usage — all collection boxes unchecked**  
- [ ] **Test instructions pasted; credentials blank**  
- [ ] Mature content = No  
- [ ] Package zip uploaded  

# Riverbend Yoga Studio – Touchstone 3

Student project for **Introduction to Web Development – Touchstone 3: Visual Design and Responsive Layout**.
Client: **Client B – Riverbend Yoga Studio**. Author: Ahmed Yousif.

This project builds on my Touchstone 2 site. The four pages keep all of their Task 2 content and features:
the weekly schedule table, class descriptions, pricing table, instructor biographies, accessibility information,
studio policies, workshop list, the full request form, the responsive `<picture>` element and the audio player.
Touchstone 3 adds one external stylesheet (`css/styles.css`) and a few class names and wrapper `<div>`s
so the CSS can lay the pages out with Flexbox.

## Media files

All seven media files from Touchstone 2 are included and load correctly:

| File | Folder | Used on |
|---|---|---|
| `yoga-logo_c.png` | `images/` | every page (header logo) |
| `yoga-studio_c.png` | `images/` | index.html (Our mission) |
| `yoga-feature-large_c.png` | `images/` | index.html (featured class, screens 800px and wider) |
| `yoga-feature-small_c.png` | `images/` | index.html (featured class, smaller screens) |
| `yoga-instructor_c.png` | `images/` | about.html (Maya Collins) |
| `yoga-workshop_c.png` | `images/` | events.html (workshop figure) |
| `yoga-breathing_c.mp3` | `audio/` | index.html (breathing exercise, 22 seconds) |

The logo file has a white background, so the CSS uses `mix-blend-mode: multiply` to let the cream header show through it.

## How to run it locally

1. Keep all files and folders together.
2. Double-click `index.html` to open it in a modern browser (Chrome, Edge, Firefox or Safari).
3. Use the menu to move between the four pages.

To test the responsive layout, press F12 to open the developer tools and turn on the device toolbar,
or make the browser window narrower.

## Publishing with GitHub Pages (optional)

1. Create a GitHub repository and upload every file and folder in this project.
2. Open **Settings → Pages**, choose the `main` branch and `/ (root)`, then click **Save**.
3. After a minute GitHub shows your live link, for example `https://<your-username>.github.io/<repository-name>/`.
4. Paste the repository link and the live link into Section 1 of the Touchstone 3 document.

## Project structure

```
Riverbend-Yoga/
├── index.html
├── services.html
├── about.html
├── events.html
├── css/
│   └── styles.css
├── images/          (the six PNG images)
├── audio/           (yoga-breathing_c.mp3)
├── fonts/           (Lora and Nunito Sans, stored locally)
├── screenshots/     (screenshots used in the Touchstone 3 document)
└── README.md
```

## Design summary

- **Colors (4):** cream `#F7F3EC`, sage green `#4F6F5A`, sand `#D9B99B`, charcoal `#2E3532`.
  Every text and background pair meets the WCAG AA contrast level (lowest: sage on cream, 5.06:1).
- **Fonts (2):** Lora (headings, legends, tagline) and Nunito Sans (body text, menu, buttons, form).
  Body text is 18px to make reading easier for older adults.
- **Flexbox:** header, main menu, "On this page" links, photo-and-text rows, card sections, buttons,
  form choices and footer.
- **Media queries:** 900px (tablet) and 600px (phone).
- All paths are relative.

## Testing done

- All four pages open and load `css/styles.css`.
- Every link and in-page anchor (for example `about.html#accessibility-heading`) points to a page and id that exist.
- No horizontal scrolling at 1366px, 820px and 390px wide.
- HTML checked with html-validate: no errors.
- All six images and the MP3 load on every page that uses them, and the `<picture>` element shows the large photo on desktop and the small one on phones.

## Notes

- The request form has no backend (`action="#"`), as in Touchstone 2. The browser checks the
  required fields and formats, but the form does not send a real request.
- Lora and Nunito Sans are free fonts under the SIL Open Font License (license files are in `fonts/`).

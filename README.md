# Riverbend Yoga Studio (Touchstone 3)

This is my Touchstone 3 project for Introduction to Web Development (Visual Design and Responsive Layout). My client is Client B, Riverbend Yoga Studio.

Live site: https://iseido.github.io/Riverbend-Yoga/

I built this on top of my Touchstone 2 site, so all the Task 2 content is still here: the schedule and pricing tables, class descriptions, instructor bios, accessibility info, studio policies, the workshop list and the request form. For Task 3 I added one stylesheet, `css/styles.css`, plus some class names and a few wrapper `<div>`s so I could lay the pages out with Flexbox.

## Running it locally

Download or clone the repo and open `index.html` in a browser. There is nothing to install. Keep the folders together, because the pages load the CSS, images, fonts and audio with relative paths.

To check the responsive layout, open the developer tools (F12), turn on the device toolbar and try a phone size and a tablet size.

## Files

```
index.html, services.html, about.html, events.html
css/styles.css     the only stylesheet, linked from all four pages
images/            the logo and photos from Task 2
audio/             the guided breathing MP3
fonts/             Lora and Nunito Sans, saved locally
screenshots/       screenshots I used in my Touchstone 3 document
```

## Design

I kept the palette to four colors: cream (#F7F3EC) for the background, sage green (#4F6F5A) for headings and buttons, sand (#D9B99B) for borders and highlight boxes, and charcoal (#2E3532) for body text and the footer. Every text and background pair passes the WCAG AA contrast check. The lowest one is sage on cream at 5.06:1.

Headings use Lora and everything else uses Nunito Sans. I set the body text to 18px because the studio wants older adults to feel welcome, and bigger text is easier for them to read.

The header, menu, cards, photo rows, form and footer all use Flexbox. There are two media queries. At 900px the photos move above their text, and at 600px the menu turns into a list of full-width buttons.

The logo PNG has a white background, so I used `mix-blend-mode: multiply` to blend it into the cream header instead of showing a white box.

## Testing

I opened every page at 1366px, 820px and 390px wide and checked that none of them scroll sideways. All the links and section links go to pages and ids that exist, all the images and the MP3 load, and html-validate found no errors in the HTML.

## Notes

The request form doesn't have a backend (`action="#"`), same as in Task 2. The browser checks the required fields, but nothing actually gets sent.

Lora and Nunito Sans are free under the SIL Open Font License. The license files are in `fonts/`.

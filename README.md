# FF Name Style generator

Source files for the [FF Name Style tool on FF Bio Code](https://ffbiocodes.com/ff-name-style/). The live page lets players turn a base name into copyable Unicode text, explore symbols, and assemble a custom nickname. This repository documents the page components and makes them easier to review and maintain.

## What is here

| File | Purpose |
| --- | --- |
| [`source/ff name style.html`](source/ff%20name%20style.html) | Generator markup, styles, metadata, structured data, and browser logic |
| [`source/FFNAMESTYLE-BODY.HTML`](source/FFNAMESTYLE-BODY.HTML) | Usage guide, examples, accessibility details, and FAQ |
| [`source/ffnamestyle-author bio.html`](source/ffnamestyle-author%20bio.html) | About-the-creator section |
| [`source/preview.html`](source/preview.html) | Separate Free Fire bio preview gallery component |

These files are page components intended for the existing FF Bio Code website. They are not a complete standalone website or an official Garena project. The bio preview gallery is included for source reference; it is not part of the nickname generator.

## Use the generator

1. Open the [live FF Name Style page](https://ffbiocodes.com/ff-name-style/).
2. Enter a short base name and compare the available text styles.
3. Copy a result, or send it to the custom nickname builder to add a symbol or frame.
4. Paste the final text into the destination app and check its appearance and acceptance before confirming a name change.

The generated output uses Unicode characters, not an installed font. Appearance and acceptance can vary by device and app. The generator's input limits are editing limits; they do not override the game's current naming rules. Never enter a game password into a nickname tool.

## Working with the source

The main tool is plain HTML, CSS, and JavaScript. Its optional Google Fonts request affects presentation; the nickname conversion runs in the browser. When integrating the source, retain a single page title, canonical URL, and primary heading on the published page. Review structured data against visible page content before deployment. Keep the existing site's navigation, other tools, and theme integration intact.

This repository does not enable GitHub Pages because the canonical live experience is the website linked above.

## Project status

Maintained as a source and documentation repository for FF Bio Code. This is a fan-made nickname formatting tool and is not affiliated with or endorsed by Garena or Free Fire.


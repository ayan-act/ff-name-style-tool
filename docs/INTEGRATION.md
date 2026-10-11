# Integration and release notes

The files in `source/` are website components, not a buildable application. The production target is the existing [FF Name Style page](https://ffbiocodes.com/ff-name-style/). Integrate only the component being changed; preserve the site's navigation, bio tools, preview gallery, analytics consent, and other working features.

## Component boundaries

- `ff name style.html` contains the primary generator, its styles and scripts, and page-level metadata. Do not insert duplicate `<title>`, description, canonical, Open Graph, or structured-data tags if the site theme or SEO plugin already generates them.
- `FFNAMESTYLE-BODY.HTML` belongs below the generator. It provides explanatory content and FAQ markup. Keep its FAQ structured data aligned with the visible answers.
- `ffnamestyle-author bio.html` is an author section. Keep author claims and links accurate.
- `preview.html` is a separate bio preview gallery. Its external images and module dependency should be reviewed before use; it is not required by the nickname generator.

## Release checklist

1. Confirm the page's canonical URL is `https://ffbiocodes.com/ff-name-style/` and there is one primary heading.
2. Test the font and builder tabs with keyboard and touch input. Verify the selected tab, focus movement, and announcements.
3. Test copy, customize, saved styles, symbols, frames, and the empty-input state in current mobile and desktop browsers.
4. Check that a long or unusual Unicode sequence does not break the layout and that the tool describes its limits accurately.
5. Confirm the supporting guide and FAQ still match the actual controls and limits.
6. Inspect the live page in light and dark system modes where applicable; check narrow screens and browser zoom.
7. Verify outbound resource links and disclaimers. Check the live page after deployment rather than assuming this repository reflects production immediately.

## Privacy and content integrity

Nickname generation takes place in the browser. Do not request a player's game password or imply that this tool can validate a name against a game server. If adding telemetry or external services, update the site's privacy notice to match the behavior. Avoid publishing credentials, analytics secrets, or private user data in this public repository.


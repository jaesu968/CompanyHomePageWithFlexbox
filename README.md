# Imagination Company — Flexbox Homepage

This project is a responsive company homepage built using CSS Flexbox. It demonstrates practical layout techniques (header, navbar, hero, products, team) while keeping content centered and images displayed full-bleed where appropriate.

## Live preview
- Open the site locally by opening [index.html](index.html) in your browser, or serve the folder with a simple static server.

## Files
- [index.html](index.html) — page markup
- [resources/styles.css](resources/styles.css) — primary stylesheet
- resources/images/ — project images used for hero, products, and team

## Project goals
- Use Flexbox to build a clean, responsive homepage layout.
- Keep the main content centered while allowing decorative images to span the full viewport horizontally.
- Maintain accessibility and responsive behavior on small screens.

## Notable layout decisions
- Header: `display: flex` with the site title centered and the logo positioned absolutely on the right so the title remains visually centered across the page.
- Navbar: an inline flex row centered beneath the title (`.navbar ul { display: flex; justify-content: center; }`).
- Mission hero: implemented as a full-width block (`.mission-hero`) containing an inline `<img>` scaled to the page width with `object-fit` to control cropping; the heading and paragraph remain in centered `.content` containers above/below the hero.
- Products: each `.product` is a flex row with the image on the left and text on the right; a media query stacks them on small screens.
- Team: `.teammates` uses flex-wrap to create a responsive grid of teammate cards; the background is a full-bleed section (`.team-hero`) with an overlay for legibility.

## Accessibility & performance notes
- Decorative hero images use `aria-hidden="true"` where appropriate. If an image conveys content, prefer a regular `<img>` with an informative `alt` attribute.
- Images are served from `resources/images/`. If you move these files, update the paths in `resources/styles.css` and `index.html`.

## Suggestions for Improvement or Customization
- Change hero/team images: replace files in `resources/images/` and keep filenames or update URLs in `resources/styles.css` and `index.html`.
- Adjust hero height: edit `.mission-hero__img { height: ... }` in `resources/styles.css` (currently 360px desktop, 200px mobile).
- Tweak content width: change `.content { max-width: ... }` to suit your design.

## Credits
- Images: credits are provided in the footer of the site. 

---
# CompanyHomePageWithFlexbox

# Vivienne Hart — Author Website

A single-file author website for literary fiction writer Vivienne Hart. Built with HTML, Tailwind CSS (CDN), and vanilla JS.

## Pages

- **Home** — Full-bleed hero, pull quote, featured books strip, about teaser, press logos
- **Books** — Featured novel (large), two backlist titles, book club CTA
- **About** — Bio, awards sidebar, portrait block, agent info
- **Contact** — Enquiry form with subject selector, confirmation message

All four pages live in `vivienne-hart.html` and are toggled via a lightweight JS router — no framework, no build step.

## Design

| Token | Value |
|---|---|
| Ivory | `#FAF8F4` |
| Blush | `#EDD9CE` |
| Sage | `#B8C4B1` |
| Warm Ink | `#2C2420` |
| Muted Gold | `#C9A96E` |
| Display face | Cormorant Garamond (Google Fonts) |
| Body face | Jost (Google Fonts) |

The botanical SVG watermarks are hand-coded and inline — no external assets required beyond the two Google Fonts.

## Usage

Open `vivienne-hart.html` in any browser. No build process, no dependencies to install.

To deploy, upload the single file to any static host (Netlify, GitHub Pages, Vercel, etc.).

## Customisation

- **Copy** — All text is inline in the HTML; search for the relevant section comment (e.g. `BOOKS PAGE`) to find it quickly.
- **Colours** — Defined in the `tailwind.config` block at the top of the file.
- **Fonts** — Swap the Google Fonts `<link>` and update the `fontFamily` config to change typefaces.
- **Book covers** — Replace the CSS gradient `div.book-cover` blocks with `<img>` tags pointing to real cover images.
- **Form** — The contact form is static. Wire up the `handleSubmit()` function to a service like Formspree, Netlify Forms, or your own endpoint.
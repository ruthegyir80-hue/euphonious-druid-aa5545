# AGENTS.md

## Architecture
This is a static site with no build step. Netlify publishes `public/` (see `netlify.toml`).

- `public/index.html` contains the whole site: markup, a `<style>` block with design tokens in `:root`, and a `<script>` block for the particles, reveal animations, and nav.
- `public/img/` holds the sample screenshots. The originals were base64-embedded in an earlier version of the page; they now live here as files.

## Conventions
- Always reference images through the Netlify Image CDN, e.g. `/.netlify/images?url=/img/<file>&w=900&fm=webp`. Never inline base64 images.
- Use lowercase, hyphenated image filenames.
- Build work samples with the `.sample-card`, `.sample-title`, and `.sample-desc` classes. Each card has a short description under the image.
- Project cards use `.project-card` and stagger with `reveal-delay-1` and `reveal-delay-2`.
- Keep to the existing palette (cream, espresso, terra, gold) and fonts (Playfair Display for headings, Inter for body text).

## Notes
- The contact form is visual only. `handleSend` shows a confirmation but submits nothing. Use Netlify Forms if real submissions are needed.

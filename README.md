# Ruth Salvage Egyir — Portfolio

Personal portfolio for Ruth Salvage Egyir, a customer service and virtual assistant professional based in Cape Coast, Ghana. It covers her background, skills, experience, projects, visual work samples, templates, and contact details.

## Technologies

- A single static HTML page (`public/index.html`) with inline CSS and JavaScript
- Google Fonts (Playfair Display and Inter)
- Netlify hosting, with the Netlify Image CDN serving resized WebP versions of the sample screenshots

## Running locally

```bash
netlify dev
```

You can also open `public/index.html` in a browser. Sample images load through `/.netlify/images`, so they only appear when the site runs under Netlify or `netlify dev`.

## Adding a work sample

1. Save the screenshot in `public/img/` using a lowercase, hyphenated filename.
2. Copy an existing `.sample-card` block in the `#samples` section, then update the title, image path, alt text, and description.

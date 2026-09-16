# Mark Justine Taburada — Portfolio Website

A clean, modern, single-page portfolio site for Virtual Assistant & Graphic Design work.

## File structure

```
portfolio/
├── index.html
├── css/
│   └── style.css
├── js/
│   └── script.js
├── images/
│   ├── portfolio/      → your project images (already placed)
│   └── profile/        → your profile photo (already placed)
└── README.md
```

## How to view it

Just double-click `index.html`, or open it in any browser. No build step, no install — it's plain HTML/CSS/JS.

To publish it, upload the whole `portfolio` folder to any static host (Netlify, Vercel, GitHub Pages, or your own hosting) and it will work as-is.

## What's already set up

- Your profile photo (`images/profile/profile.png`) and all six portfolio pieces from your PDF are already in place and linked in `index.html`:
  - Aura "Lavender Sky" packaging
  - Crunchy Bites chip bag
  - Salo-Salo Chicharon packaging
  - Digital marketing social ad
  - "Get More Clicks" YouTube thumbnail
  - Channel welcome graphic
- Your bio, tools (Canva, Adobe Photoshop, CapCut, Google Fonts), and experience note are taken directly from your original portfolio content.
- Your email (`markjustinetaburada.va@gmail.com`) and phone (`+63 997 822 6927`) are wired into the Hire Me buttons, footer, and contact form.

## Things to customize

**Add more portfolio pieces**
Duplicate one `<figure class="portfolio-item">` block inside the `<section class="portfolio">` in `index.html`, point it at your new image in `images/portfolio/`, and set `data-category` to `packaging`, `social`, or `thumbnail` (or add a new category — just add a matching filter button above the grid).

**Social links**
The footer and contact section currently only show email and phone, since no social links were in your original file. To add Facebook, Instagram, or a Canva/Behance link, add an `<a>` tag inside `.footer-contact` in `index.html` and (optionally) near the contact list too.

**Contact form**
Right now the form opens the visitor's email app pre-filled with their message (no backend needed). If you'd rather have messages land directly in your inbox without opening an email app, sign up for a free form service like Formspree (formspree.io), then change the `<form>` tag's behavior in `js/script.js` to POST to your Formspree endpoint instead of using `mailto:`.

**Colors & fonts**
All colors and fonts are defined as CSS variables at the very top of `css/style.css` (the `:root` block) — change a value there and it updates everywhere.

**Text**
Section headings, the about text, and service/skill descriptions are all plain text inside `index.html` — search for the section (e.g. `id="services"`) and edit directly.

## Notes

- No fake clients, testimonials, or years of experience were added — only what was in your original portfolio, plus the service categories you asked to include.
- Images use `loading="lazy"` and are sized/compressed for fast loading while keeping full quality.
- The site respects `prefers-reduced-motion` and is keyboard/screen-reader accessible (skip link, focus states, alt text, semantic headings).

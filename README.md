# Personal academic website

Static site — plain HTML and CSS, no build step. Edit `index.html` and push.

## Structure

```
.
├── index.html              ← the whole site (content + styles live here)
├── assets/
│   ├── profile.jpg         ← your photo (square, ~800×800, replace the placeholder)
│   ├── favicon.svg
│   ├── favicon-32.png
│   ├── favicon-64.png
│   └── apple-touch-icon.png
└── files/
    ├── CV.pdf              ← drop your CV here (this exact filename, or update the links)
    └── paper-one.pdf       ← paper PDFs, if you host them yourself
```

## Things to change before publishing

Search `index.html` for these and replace:

- `Your Name` — name, in the title, hero, structured data and footer
- `yourusername.github.io` — your site URL, in the `og:` / `twitter:` tags and structured data
- `you@university.edu` — email
- `scholar.google.com/citations?user=XXXXXXX` — Scholar profile (or delete that icon)
- `github.com/yourusername`, `linkedin.com/in/yourusername` — social links
- The About text, papers, publications and news entries

To add a paper, copy one `<div class="entry">…</div>` block and edit it.
To remove a section, delete the whole `<section>…</section>` and its link in the nav.

## Local preview

Open `index.html` in a browser, or run `python3 -m http.server` in this folder
and visit http://localhost:8000.

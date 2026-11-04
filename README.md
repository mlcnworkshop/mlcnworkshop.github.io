# MLCN workshop website

Source for <https://mlcnworkshop.github.io> (Jekyll, AcademicPages theme, built by GitHub Pages).

## Yearly update checklist

1. **`_data/workshop.yml`** – year, city, dates (also the ISO dates for search engines), links, banner photo and credit, keynotes, FAQ. Almost every page reads from this file, as do `llms.txt` and the structured data for Google.
2. **`_data/history.yml`** – after a workshop, add it at the top (keynotes, organizers).
3. **Archive the program** – move `_pages/program.md` content to `_pages/<year>/program.md` with permalink `/<year>/program/`; reset `_pages/program.md`.
4. **Organizers** – edit `_pages/community_organizers.md`.
5. **Search** – update the year in the `description:` lines of the pages and in `_config.yml`.
6. **Files** – put templates and copyright forms in `files/` and link them from `workshop.yml`.


Local preview: `bundle install && bundle exec jekyll serve`, then open http://localhost:4000.

## Search engines

- Structured data (Event, Organization, FAQ) is added on the home page from `_data/workshop.yml` (`_includes/head/custom.html`).
- `sitemap.xml` is generated automatically; `robots.txt` points to it; `llms.txt` gives AI assistants a plain-text summary.
- Add the site in Google Search Console and paste the verification code into `google_site_verification` in `_config.yml`.

## What is in this repository

- `_pages/` – the pages (Markdown + Liquid)
- `_data/` – yearly workshop data, past editions, menu
- `_layouts/`, `_includes/`, `_sass/`, `assets/` – the trimmed AcademicPages theme
- `images/` – logos, favicon, banner photo
- `robots.txt`, `llms.txt` – search engines and AI assistants

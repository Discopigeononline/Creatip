# CREATIP Hugo Site Guide

## Commands
- Build: `hugo --minify`
- Start dev server: `hugo server -D` (includes draft content)
- Clean build: `rm -rf public/ && hugo --minify`
- Deploy: Automated via GitHub to Netlify

## Configuration
- Site config: `config.toml` (baseURL, title, params)
- CMS config: `static/admin/config.yml` (Decap CMS settings)

## Content Structure
- Content in Markdown under `/content/` directory
- French language: `languageCode = 'fr-fr'`
- Sections: actu, annuaire, recherche, formation
- Always use YAML frontmatter (---) not TOML (+++)
- Use kebab-case for filenames (e.g., my-article.md)

## CMS Guidelines
- Document files go in `/static/documents/`
- Image files go in `/static/images/`
- Research articles should use `document` field for PDFs
- All CMS fields must match template parameters exactly

## Style Guidelines
- HTML templates in `/layouts/`
- SCSS styling in `/assets/sass/main.scss`
- Use Hugo partials for reusable components
- Follow Hugo naming conventions (kebab-case for files)
- Shortcodes in `/layouts/shortcodes/`
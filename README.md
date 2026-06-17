# Academic Personal Website

A minimal [GitHub Pages](https://pages.github.com/) site for Olivier Rubel, built with [Jekyll](https://jekyllrb.com/) and Markdown.

**Live site:** [https://ormarketing.github.io](https://ormarketing.github.io) (after deployment)

## Pages

| Page | File to edit |
|------|--------------|
| Home | `index.md` |
| Research | `research.md` |
| Teaching | `teaching.md` |
| CV | `cv.md` |
| Contact | `contact.md` |

Site-wide settings (title, email, navigation) are in `_config.yml`.

## Deploy to GitHub Pages

1. Create a new repository on GitHub named **`ormarketing.github.io`** (must match your username exactly).

2. Push this folder to the repository:

   ```bash
   cd "/Users/orubel/Library/Mobile Documents/com~apple~CloudDocs/github page"
   git init
   git add .
   git commit -m "Initial academic website"
   git branch -M main
   git remote add origin https://github.com/ormarketing/ormarketing.github.io.git
   git push -u origin main
   ```

3. In the repo on GitHub, go to **Settings → Pages** and confirm the source is **Deploy from branch: main / (root)**.

4. After a minute or two, the site will be live at [https://ormarketing.github.io](https://ormarketing.github.io).

## Preview locally (optional)

Requires Ruby. On macOS:

```bash
bundle install
bundle exec jekyll serve
```

Open [http://localhost:4000](http://localhost:4000).

## Customization

- **Navigation:** Edit the `navigation` list in `_config.yml`.
- **Styling:** Edit `assets/css/style.css`. Colors and fonts are defined at the top in `:root`.
- **Add a photo:** Place an image in `assets/images/` and add it to `index.md`.
- **Google Scholar / SSRN:** Add links in `contact.md` and optionally `_config.yml`.

## Structure

```
├── _config.yml          # Site settings
├── _layouts/default.html
├── _includes/nav.html
├── assets/css/style.css
├── index.md             # Home
├── research.md
├── working-papers.md
├── teaching.md
├── cv.md
└── contact.md
```

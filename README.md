# Mod Studio website

Source for the Mod Studio website, built with [Jekyll](https://jekyllrb.com/) and deployed to GitHub Pages by GitHub Actions.

Mod Studio is a project of [ModSolutionz](https://modsolutionz.com).

## Structure

| Path | What it is |
| --- | --- |
| `index.html` | Home page |
| `_includes/cooking.svg` | Animated "Cooking something cool" illustration |
| `privacy-policy.md` | Privacy Policy (`/privacy-policy/`) |
| `terms-of-service.md` | Terms of Service (`/terms-of-service/`) |
| `_includes/footer.html` | Footer with legal links and contact email |
| `_config.yml` | Site title, contact email, parent company |
| `.github/workflows/pages.yml` | Build and deploy workflow |

## Run locally

Requires Ruby 3.x.

```bash
bundle install
bundle exec jekyll serve --livereload
```

Then open http://localhost:4000.

## Deploy

Every push to `main` builds the site and deploys it to GitHub Pages.
In the repository settings, **Settings → Pages → Build and deployment → Source** must be set to **GitHub Actions**.

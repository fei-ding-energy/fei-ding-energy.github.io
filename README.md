# fei-ding-github-pages

This repo contains a Jekyll site for GitHub Pages. It includes pages for Home, Projects, Papers, Talks, and Others.

## One‑time setup

1. Create a new GitHub repository (e.g., `feiding.github.io` or any name you like).
2. Upload this folder's contents to the repo (or unzip and drag‑drop).
3. In **Settings → Pages**, choose:
   - **Source:** `GitHub Actions` (recommended) *or* `Deploy from a branch` with branch = `main`, folder = `/root`.
4. (Optional) Set your custom domain and enable HTTPS.
5. After build, your site appears at `https://<username>.github.io/` or your custom domain.

## Editing

- `_config.yml`: site title, tagline, links, analytics.
- `index.md`: main page with About, Education, Experience, and Honors.
- `/projects`, `/publications`, `/talks`, `/others`: edit Markdown files within each folder.
- Add images to `/assets` and link as `![alt](/assets/your-image.png)`.

## Local preview

```bash
# Requires Ruby, Bundler, and Jekyll
gem install bundler jekyll
bundle init && echo 'gem "github-pages", group: :jekyll_plugins' >> Gemfile
bundle install
bundle exec jekyll serve
```
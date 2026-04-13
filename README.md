# TALE Journal Site

This is a GitHub Pages-compatible Jekyll website for **Technology-enhanced Assessment & Learning Environments (TALE)**.

## Run locally

1. Install Ruby and Bundler (if needed):
   - `gem install bundler`
2. Install project dependencies:
   - `bundle install`
3. Start local server:
   - `bundle exec jekyll serve`
4. Open:
   - `http://127.0.0.1:4000`

If you edit files, Jekyll will rebuild automatically while the server is running.

## Update current issue

Edit `_data/issue.yml`:

- `volume`
- `issue`
- `year`
- `theme`
- `note`

The home page reads these values automatically.

## Add or update papers

Edit `_data/papers.yml` and add entries in this format:

```yaml
- title: "Paper title"
  authors: "Author One, Author Two"
  year: 2026
  pdf_url: "/papers/your-paper-file.pdf"
```

If `pdf_url` is empty, the site shows "PDF link coming soon."

## Where to place PDF files

Store files in a folder such as `papers/` at project root and link with a relative path:

- `/papers/paper-name.pdf`

## Deployment on GitHub Pages

1. Push this project to a GitHub repository.
2. In repository settings, open **Pages**.
3. Set source to **Deploy from a branch**.
4. Select `main` branch and root folder.
5. Save and wait for the site to publish.

# Duc Tung Nguyen — Jekyll personal website

A text-first personal academic website with a scholarly medieval-library feel: parchment background, serif typography, ink-brown text, muted green and antique-gold accents. No decorative images are required.

## Publish on GitHub Pages
1. Create a repository on GitHub, for example `duc-tung-nguyen`.
2. Upload all files and folders from this package, including hidden files if your upload method supports them.
3. Open **Settings → Pages**.
4. Choose **Deploy from a branch**, branch `main`, folder `/(root)`, then Save.
5. Wait for the deployment. GitHub shows the published URL under Settings → Pages.
6. If the site is published at `https://USERNAME.github.io/duc-tung-nguyen/`, set `baseurl: "/duc-tung-nguyen"` in `_config.yml`. If the repository is named `USERNAME.github.io`, keep `baseurl: ""`.

GitHub Pages docs: https://docs.github.com/en/pages

## Add a blog post
Create a Markdown file in `_posts` named like:
`2026-11-01-my-first-article.md`

Start it with:
```yaml
---
layout: default
title: "My first article"
date: 2026-11-01
categories: [data]
---
```
Then write the article below using Markdown. The Notes page and homepage list update automatically.

## Add a YouTube video
In a post, replace `VIDEO_ID` with the ID from `https://www.youtube.com/watch?v=VIDEO_ID`. Example:
```html
<div class="video">
  <iframe src="https://www.youtube-nocookie.com/embed/VIDEO_ID" title="YouTube video" allowfullscreen></iframe>
</div>
```
For a channel link, replace the YouTube URL in the placeholder with your channel URL.

## Customize
- Global colors, fonts and layout: `assets/css/style.css`.
- Navigation: `_config.yml` (`header_pages`) and the Markdown page files.
- Homepage content: `index.md`.
- Static pages: `about.md`, `research.md`, `teaching.md`, `projects.md`.
- Documents: add public PDFs under `assets/documents/`, then link to them with a relative URL.
- Cards: copy or remove `<article class="card">...</article>` blocks.

## Notes
GitHub Pages builds Jekyll automatically when publishing from a branch. This starter uses the `github-pages` gem for local preview compatibility. A local preview requires Ruby and Bundler; it is not required just to publish on GitHub Pages. Do not upload private student data or confidential documents to a public repository.

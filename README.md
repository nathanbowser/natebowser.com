# natebowser.com

Static personal site for Nate Bowser.

## Deployment

This site is plain static HTML/CSS and can be deployed directly to GitHub Pages.

Files intentionally published for search engines and AI agents:

- `index.html`, `about/index.html`, `projects/index.html`, `resume/index.html` plus `.html` redirect shims
- `index.md`, `projects.md`, `resume.md`, `about.md`
- `llms.txt`
- `agent-corpus.ndjson`
- `robots.txt`
- `sitemap.xml`

GitHub Pages should preserve these static files as-is. `.nojekyll` is included so dot-directories and static support files are not processed by Jekyll.

## Analytics

Recommended simple option: Cloudflare Web Analytics. It is free, privacy-first, and works by adding a small JavaScript beacon snippet to each HTML page.

Add the Cloudflare snippet just before `</body>` in each `.html` file after creating the site in Cloudflare Web Analytics.

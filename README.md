# limsijie93.github.io

Personal site: resume, project write-ups, and blog. Built with Jekyll + [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/), hosted on GitHub Pages ("Deploy from a branch", `main` / root — no custom build workflow needed for the site itself).

## Writing a new blog post

1. Add a new file to `_posts/` named `YYYY-MM-DD-your-title.md`:
   ```yaml
   ---
   title: "Your Title"
   date: 2026-08-15
   categories: [ai]
   tags: [llm]
   excerpt: "One-line summary shown on the blog index and RSS feed."
   ---
   Post body in markdown...
   ```
2. Commit and push to `main`. GitHub Pages rebuilds automatically (~1 minute) and the post appears on [/blog/](https://limsijie93.github.io/blog/) and in [/feed.xml](https://limsijie93.github.io/feed.xml).

No index to update by hand — the blog listing and pagination are generated automatically from everything in `_posts/`.

## How resume.md stays in sync

`resume.md` is **not hand-edited here**. It's overwritten automatically by a GitHub Actions workflow (`sync-resume.yml`) that lives in the private [`career-resume`](https://github.com/limsijie93/career-resume) repo, which fires whenever `master-cv/Lim_Si_Jie_CV_master.md` changes there. That workflow runs `scripts/render_public_resume.py` (also in `career-resume`) to strip the private conversion frontmatter and phone number, hyperlink the contact line, and add this site's Jekyll frontmatter, then pushes the result here as `resume.md` — which itself triggers a Pages rebuild.

If you ever need to re-point or debug the sync:
- Workflow: `career-resume/.github/workflows/sync-resume.yml`
- Transform script: `career-resume/scripts/render_public_resume.py`
- Auth: a fine-grained PAT stored as the `SITE_REPO_TOKEN` secret in `career-resume`, scoped to **Contents: Read and write** on this repo only.
- Non-secret config: `PUBLIC_GITHUB_URL` / `PUBLIC_LINKEDIN_URL` repo variables in `career-resume`.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

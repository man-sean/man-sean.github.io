# Personal Academic Website (Jekyll)

## Origin
- The visual design is inspired by Jon Barron’s academic webpage.
- Leonid Keselman adapted that style into a Jekyll-based template, which this repo builds on.
- This repository is a customized fork for my own content and layout needs.

## Local Setup
Prerequisites:

- Ruby installed (Homebrew Ruby is recommended for macOS): `/opt/homebrew/opt/ruby/bin`
- Bundler available (`gem install bundler` if needed)

Install dependencies and run locally:

```
bundle install
bundle exec jekyll serve
```

Then visit `http://127.0.0.1:4000`.

## Project Quirks & Notes
- Posts use `permalink: /` to avoid dedicated post pages. This creates multiple entries in `sitemap.xml` pointing to `index.html`.
- If you want multi-paragraph excerpts, set `excerpt_separator: <!--more-->` in `_config.yml`.
- Thumbnails are generated with `_make_thumbnails.sh` and stored in `tn/`.
- Some posts contain legacy front matter fields (e.g., `author`, long descriptions). They can be ignored or cleaned up as needed.

## Deployment to GitHub Pages
- Ensure `baseurl` and `url` in `_config.yml` match your GitHub Pages settings.
- Commit and push to the default branch used by Pages (commonly `main` or `master`).
- For user/organization sites, the site is served from the root; for project sites, it is served under `/<repo-name>/`.
- GitHub Pages builds automatically on push; no local build output should be committed.

## Content and Licensing
- Please respect copyright for materials under `images/`, `pdfs/`, and `_posts/`.

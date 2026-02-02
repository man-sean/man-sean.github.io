# TODO: Personalize Website

## Current Starting Point
- [x] Forked Jekyll template with Leonid Keselman’s content still present.
- [x] Site title updated to “Sean Man” with a “[WIP]” tag under the main title.
- [x] Bundler-based setup is in place for local dev (see `README.md`).

## Phase 1: Minimal Launch (fast cleanup to go live)
- [ ] Replace the main bio paragraph(s) in `_layouts/default.html`.
- [ ] Update contact links (Email, GitHub, Google Scholar, LinkedIn) in `_layouts/default.html`.
- [ ] Swap the profile image: `images/circle_bw_crop.jpg` (and update its `alt` text).
- [ ] Update `url` and `baseurl` in `_config.yml`.
- [ ] Remove/replace the most visible posts in `_posts/` that appear on the homepage.

## Phase 2: Full Personalization (recommended)
- [ ] Replace all remaining posts in `_posts/` with your own entries.
- [ ] Curate `images/`, `pdfs/`, and `tn/` so only your assets remain.
- [ ] Update favicon via `_make_favicon.sh` if desired.
- [ ] Review styles in `style.scss` and `_sass/` for branding changes.

## Phase 3: Polish & Maintenance
- [ ] Clean up legacy front matter fields in posts.
- [ ] Confirm sitemap behavior and permalink settings.
- [ ] Verify `CNAME` and GitHub Pages settings.

---

## Data Needed From You (Provide in this format)

### 1) Profile/Bio
```
name: "Sean Man"
title_line: "PhD Student, [Lab/Dept], [University]"  # optional
bio_paragraphs:
  - "Short paragraph 1"
  - "Short paragraph 2"
contact:
  email: "your@email.com"
  github: "https://github.com/yourname"
  scholar: "https://scholar.google.com/citations?user=..."
  linkedin: "https://www.linkedin.com/in/..."
```

### 2) Publications / Projects (one per item)
```
- title: "Paper or Project Title"
  authors: "First Author, Second Author, ..."
  venue: "Conference/Journal, Year"
  year: 2025
  category: "research"  # use research/intel/misc to match sections
  image: "/images/your-image.png"
  thumbnail: "/tn/images/your-image.png"  # optional if you use thumbnails
  links:
    arxiv: "https://arxiv.org/abs/..."       # optional
    pdf: "/pdfs/your-paper.pdf"              # optional
    code: "https://github.com/..."           # optional
    video: "https://..."                     # optional
    website: "https://..."                   # optional
  excerpt: "1–2 sentence summary for the homepage."
```

### 3) Awards / Teaching / Service (optional)
```
- title: "Award Name"
  year: 2024
  details: "Short description."
```

Once you send the data, I can replace the existing content and remove any leftover template material.

---
title: "How this site was made"
description: site documentation
menu:
  sidebar:
    name: Site documentation
    identifier: sitedoc
    weight: 1
tags: ["Website","HUGO", "Toha", html", "Markdown", "YAML"]
categories: ["Website"]
---
## Overview

This site was generated using the [Hugo](https://github.com/gohugoio/hugo) platform,
with the [toha](https://github.com/hugo-toha/toha) theme  as a base.
The site showcases my profile, skills, experiences, education, and personal/practice projects, all managed via Hugo's content organization and the powerful configuration features of Toha.

### Key Features

- **Modern Static Site:** Fast, secure, and easily deployable anywhere.
- **Custom Sections:** About, Skills, Education, Experiences, Projects, and Documentation, each configurable via YAML files in `data/sections/`.
- **Project Documentation:** Each project has dedicated pages under `content/docs/` (see `cloudbenchmark.md` for a data engineering example).
- **Responsive Design:** The Toha theme ensures good appearance on all devices.
- **Custom Navbar & Sidebar:** Navigation is handled via modular layouts in `layouts/`, with easily editable site structure.
- **Social & Badges:** Integrated social links, certifications, and soft skills in the About section.
- **Easy Theming:** Background, logos, and colors are customizable via theme parameters and assets.
- **Multilingual & Search Support:** Ready for internationalization and site-wide search (see sidebar).

## Structure

- `content/` — Main markdown content, including documentation pages.
- `data/` — Site and section configuration in YAML format.
- `layouts/` — Custom HTML layouts and partials for theme overrides.
- `static/` — Static assets (images, logos, etc.).
- `.github/workflows/` — Workflow configuration for automated deployment (e.g., GitHub Pages).

## Usage

### Prerequisites

- [Hugo](https://gohugo.io/getting-started/install/) (extended version recommended)
- Basic YAML and Markdown familiarity

### Running Locally

```bash
git clone https://github.com/Christos-workspace/Christos-workspace.github.io.git
cd Christos-workspace.github.io
hugo server
```

Browse to `http://localhost:1313` to view the site.

### Building for Production

```bash
hugo --minify
```

The generated site will be found in the `public/` directory.

### Deployment

This site is published to **GitHub Pages** using **GitHub Actions** for automation. The deployment process follows the official Toha theme procedure—see the [Toha guide for GitHub Pages deployment](https://toha-guides.netlify.app/posts/getting-started/github-pages/) for detailed instructions.

You can deploy the `public/` folder to any static site hosting service (e.g., GitHub Pages, Netlify, Vercel). See `.github/workflows/deploy-site.yaml` for an automated deployment example.

## Customization

- **Content:** Add/edit markdown files in `content/docs/`, or update other sections via YAML in `data/sections/`.
- **Appearance:** Adjust theme logos, background, and colors via `site.Params` and static assets.
- **Social & Badges:** Update `data/author.yaml` and `data/sections/about.yaml` as needed.
- **Theme section overrides:** To customize or override various theme sections, edit or add files in the `layouts/partials/` and `layouts/_default/` directories as needed.

## Credits

- [Hugo Static Site Generator](https://gohugo.io/)
- [Toha Theme](https://github.com/hugo-toha/toha)
- All referenced images, logos, and badges remain property of their respective owners.

---

Feel free to fork and adapt for your own portfolio!

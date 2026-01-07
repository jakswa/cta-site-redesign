# Civic Tech Atlanta Website Redesign

A proposed redesign of [civictechatlanta.org](https://www.civictechatlanta.org) built with Jekyll and ready for GitHub Pages deployment.

## What This Is

This is a **draft redesign** created to address gaps in the current site:
- No project showcase
- No first-timer volunteer guide
- No partner engagement pathway
- No blog for updates

## What's Included

| Page | Description |
|------|-------------|
| Home | Hero, action cards, 5 principles (original wording preserved) |
| Projects | Showcase with filtering (needs real project data - see below) |
| Partner | Services overview + 5-step proposal process + Google Form |
| Volunteer | First-timer guide + FAQ + Google Form |
| Blog | Post listing with RSS feed |
| About | Org description, team placeholders, governance links |
| Civic Tech 101 | YouTube embed preserved |
| Code of Conduct | Full original content |

## Inspiration & Attribution

This redesign was informed by research into peer civic tech organizations:

- **[OpenOakland](https://openoakland.org/)** - The "Partner With Us" services model and framing
- **[Chi Hack Night](https://chihacknight.org/)** - Project showcase patterns
- **[BetaNYC](https://beta.nyc/)** - Program/initiative organization

The color palette, layout, and components are original work, but the *information architecture* borrows heavily from these organizations who've figured out how to serve similar audiences. Thank you to those communities for working in the open.

## Content That Needs Attention

### Projects Collection
The `_projects/` folder contains project cards from the [CivicTechAtlanta GitHub org](https://github.com/CivicTechAtlanta). Currently 8 projects (5 active, 3 complete).

**Adding a project:** Create a markdown file with this frontmatter:
```yaml
title: Project Name
status: active | complete
partner: Partner Org Name (or null)
tech: [JavaScript, Python, etc.]
github: https://github.com/CivicTechAtlanta/repo-name
featured: true | false
```

**Selection criteria:** Community partner, documentation quality, visual appeal, tech diversity, good story for volunteers.

### Team Data
`_data/team.yml` contains placeholder entries. Replace with real organizer info.

### Governance Pages
- `code-of-conduct.md` - Complete (from original site)
- `bylaws.md` - Complete (all 9 articles from civictechatlanta.org)
- `conflict-of-interest.md` - Has content, should be verified

### Blog
Contains one draft announcement post. Delete or edit before launch.

## Local Development

```bash
bundle install
bundle exec jekyll serve
```

Site will be available at http://localhost:4000

## Technical Notes

- Jekyll 4.x with jekyll-seo-tag and jekyll-feed plugins
- No external theme - fully custom layouts
- Responsive breakpoints at 480px, 768px, 1024px
- CSS variables for consistent theming
- Vanilla JS only (mobile nav toggle, project filters)

### Blog & Social Sharing

The blog includes:
- **RSS feed** at `/feed.xml` via jekyll-feed plugin
- **OpenGraph meta tags** for Facebook, LinkedIn, etc. (via jekyll-seo-tag)
- **Twitter Card meta tags** for Twitter/X previews (via jekyll-seo-tag)
- **Structured SEO metadata** for search engines

Blog posts should include these frontmatter fields for best sharing:
```yaml
title: "Post Title"
description: "A short summary for social previews"
date: 2026-01-06
author: Civic Tech Atlanta
image: /assets/images/some-image.jpg  # optional, for og:image
published: false  # optional, hides from build until ready
```

To preview unpublished posts locally: `bundle exec jekyll serve --unpublished`

See [Jekyll docs on drafts](https://jekyllrb.com/docs/posts/#drafts) for more options.

## Color Palette

| Role | Color | Hex |
|------|-------|-----|
| Primary | Pink | `#e63366` |
| Secondary | Navy | `#1e3a5f` |
| Accent | Coral | `#f4a261` |

## Status

See the [draft blog post](/_posts/2026-01-06-welcome-to-our-new-site.md) for review checklist and GitHub issues addressed.

---
title: "Website Redesign Status"
description: "Tracking progress on the Civic Tech Atlanta website redesign. Delete this post before launch."
date: 2026-01-06
author: Claude and Jake
image: /assets/images/hero-bg.jpg
published: true
---

> **Note:** This is a working status page for the redesign project. Delete or replace before launch.

## Review Checklist

- [ ] `_data/team.yml` - Add real organizers
- [x] `_projects/*.md` - Real projects from CivicTechAtlanta GitHub + past projects with images
- [ ] Edit or replace this draft post
- [x] `index.md` - Changed to static schedule ("every 2nd & 4th Monday")
- [x] `bylaws.md` - Complete (all 9 articles)
- [x] `_config.yml` - Set `baseurl: "/cta-site-redesign"` for GitHub Pages demo
- [ ] Reset `baseurl: ""` when deploying to civictechatlanta.org root

## GitHub Issues Addressed

- [x] #1 Homepage
- [x] #2 Blogging
- [ ] #3 Blog sharing - Partial (RSS + OpenGraph implemented; ActivityPub needs research)
- [x] #6/#13 Project Proposal Flow
- [x] #29 Code of Conduct

Not addressed: #34 (Python script - unrelated to website)

---

## What's New

- **Project Showcase** - Browse active and completed projects, filter by tech/status
- **First-Timer Guide** - Volunteer page with everything for first hack night
- **Partner Pathway** - Clear proposal-to-partnership flow with Google Form
- **Blog** - RSS feed, OpenGraph/Twitter Cards for social sharing

## About This Blog

This blog was inspired by [GitHub issue #3](https://github.com/CivicTechAtlanta/civictechatlanta.org/issues/3), which asked about sharing posts to the Fediverse via ActivityPub.

**What we've implemented:**

- **RSS Feed** - Subscribe at [/feed.xml](/feed.xml) to get new posts in your favorite reader
- **Social Sharing Previews** - Posts include OpenGraph and Twitter Card meta tags, so links shared on social media show proper titles, descriptions, and images
- **SEO-Friendly** - Each post generates structured metadata for search engines

**What's still being researched:**

- **ActivityPub/Fediverse Integration** - Automatically federating posts to Mastodon and other ActivityPub platforms isn't straightforward with static sites like Jekyll/GitHub Pages. See [issue #3](https://github.com/CivicTechAtlanta/civictechatlanta.org/issues/3) for discussion.

## Get Involved

The best way to get started is to [join us at a hack night](/volunteer/). We meet on the 2nd and 4th Mondays of each month. No experience necessary - just bring curiosity and a willingness to help.

See you soon!

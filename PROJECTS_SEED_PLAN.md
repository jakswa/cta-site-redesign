# Projects Seed Plan

## Problem
The current `_projects/` collection contains hallucinated projects:
- "Vaccinate Georgia" - does not exist
- "Sustainable Communities Web Challenge" - does not exist
- "CivicTechAtlanta.org Redesign" - this one is real (it's what we're doing)

## Goal
Replace hallucinated projects with real CTA projects from their GitHub org and any other discoverable sources.

## Research Sources

### Primary: GitHub Organization
https://github.com/CivicTechAtlanta (74 repositories)

**Known real projects from initial scan:**
| Repo | Description | Status |
|------|-------------|--------|
| `apd-crime-data` | Atlanta Police Department crime statistics | ? |
| `georgia-court-reminders-2022` | Court attendance reminder system | Archived |
| `marta-js` | JavaScript library for MARTA transit APIs | ? |
| `show-me-the-food` | Food resource mapping application | ? |
| `mapsforus` | Leaflet maps auto-generated from Google Docs | ? |
| `proj-green-careers-map` | Green career mapping for youth | ? |
| `open-data` | Atlanta open data resources list | ? |
| `citycamp` | CityCamp Atlanta 2025 website | Active |
| `agua-vida-poc` | Water chlorination proof-of-concept | ? |
| `proj-holistic-community-health` | Community health project | ? |
| `connector` | Brigade project management tool | ? |

### Secondary: Other Sources to Check
- Meetup event descriptions (past projects mentioned?)
- Slack archives (if accessible)
- Blog posts or meeting notes (if any exist)
- Code for America brigade network mentions

## Selection Criteria
When choosing projects to showcase, consider:

1. **Impact** - Did it help real people? Any metrics?
2. **Completeness** - Is it finished or actively maintained?
3. **Partner involvement** - Was there a community partner org?
4. **Visual appeal** - Does it have a demo, screenshots, or clear output?
5. **Tech diversity** - Show range of skills (Python, JS, data viz, etc.)
6. **Story** - Is there a compelling narrative?

## Recommended Approach

### Phase 1: Scan GitHub Repos
For each repo in CivicTechAtlanta org:
- Read README for project description
- Check last commit date (active vs archived)
- Look for partner mentions
- Note tech stack from repo languages
- Flag repos with good READMEs as showcase candidates

### Phase 2: Prioritize
Aim for 3-6 showcase projects with mix of:
- 1-2 "Active" status (recruiting contributors)
- 2-3 "Complete" status (demonstrating past impact)
- Variety of tech stacks
- At least one with clear community partner

### Phase 3: Write Project Cards
For each selected project, create `_projects/[slug].md` with:
```yaml
---
title: [Project Name]
status: active | complete | archived
partner: [Partner Org or "Internal"]
tech:
  - [Tech 1]
  - [Tech 2]
github: https://github.com/CivicTechAtlanta/[repo]
featured: true | false
---

[2-3 sentence description]

## Impact / Goals
- [Bullet points]

## Get Involved (if active)
- [How to contribute]
```

## Current State
- `_projects/civictechatlanta-website.md` - KEEP (real, it's this project)
- `_projects/vaccinate-georgia.md` - DELETE (hallucinated)
- `_projects/sustainable-communities.md` - DELETE (hallucinated)

## Notes
- Don't invent metrics or impact claims without sources
- When in doubt, use vague language ("helped community members" vs "helped 10,000 people")
- Link to GitHub repo so visitors can verify claims
- Mark projects as "featured: false" until vetted by CTA team

# All About VLSI — Project Guide for Claude

## Project Overview
A VLSI learning and interview-prep website replicating allaboutvlsi.com with a custom article management backend. Articles are uploaded as files (Markdown/AI-generated) and automatically structured and published.

## Repository & Branch
- **Repo:** `dhatsme/all_about_vlsi_website`
- **Dev branch:** `claude/basic-website-setup-FL0Vr`
- **Deploy:** GitHub Actions → GitHub Pages (static frontend)
- **Live URL:** `https://dhatsme.github.io/all_about_vlsi_website/`

## Commit Rules
- Every commit must have a meaningful message: what changed and why
- Format: `<type>: <short summary>` — types: `feat`, `fix`, `style`, `refactor`, `docs`, `chore`
- Example: `feat: add System Verilog category page with article listing`
- Never commit "WIP", "update", "fix stuff", or empty messages
- Always push to the designated dev branch after committing

## Tech Stack (to be confirmed)
- **Frontend:** Plain HTML/CSS/JS (no framework) — kept minimal and fast
- **Backend:** TBD based on user decision
- **Article format:** Markdown files (AI-friendly, auto-structured)
- **Deployment:** GitHub Pages (frontend) + separate backend host TBD

## Site Structure (based on allaboutvlsi.com)
```
/                        → Home (hero + category grid)
/interview-questions     → Interview Q&A listing
/freshers-grads          → Beginner content
/upto-2-3-years          → Intermediate content
/system-verilog          → SV tutorials
/verilog                 → Verilog tutorials
/uvm                     → UVM content
/projects                → Hands-on projects
/ai                      → AI vs traditional processors
/article/:slug           → Individual article view
```

## Article Upload Feature
- Admin uploads a Markdown (or AI-generated) file
- Backend parses frontmatter (title, category, tags, date)
- Article is auto-assigned to correct category
- No manual CMS needed — file upload = published

## Coding Principles
- Keep code as simple and minimal as possible
- No frameworks unless clearly justified
- No unnecessary abstractions or premature optimization
- Comments only when the WHY is non-obvious
- Mobile-first, fast-loading pages

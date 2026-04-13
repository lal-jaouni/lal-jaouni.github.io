# Personal Portfolio Site Plan

## Purpose
Dual-purpose personal site: **job applications** (linked from resumes, cover letters, LinkedIn) and **professional brand** for potential future consulting work.

## Hosting & Tech
- **Hosting:** GitHub Pages (free, deploys from repo)
- **Stack:** Static site — minimal JS, fast load, easy to maintain
- **Domain:** GitHub Pages default initially; custom domain later if desired
- **Blog:** Not at launch — can add later

---

## Research-Backed Design Principles

These are drawn from a survey of 60+ hiring managers and multiple recruiter studies.

### What Actually Matters
1. **Project quality and presentation** — this is what hiring managers spend time on
2. **Real-world problem solving** — 60%+ of recruiters prioritize this over tech stack
3. **Quantified contributions** — performance gains, data scale, measurable impact
4. **Code accessibility** — recruiters WILL click through to GitHub repos
5. **Screenshots and demos** — visual-first beats text-heavy every time
6. **Mobile responsive, no broken links, looks maintained** — table stakes

### What Doesn't Matter
- Flashy animations or complex SPA frameworks
- The site being a technical showcase itself (unless applying for frontend roles)
- Having 10+ projects — 3-5 well-presented ones outperform a long list

### Personality vs. Professional
Research shows the **sweet spot is authentic professionalism**:
- Hiring managers who got a sense of who the person is were more interested
- Your scientist-to-engineer story IS a differentiator — use it
- Write in your own voice, not corporate-speak
- A brief "about" section with your background and what drives you

---

## Site Structure (Multi-Page)

GitHub Pages supports full multi-page static sites — unlimited pages, custom routing, static assets, HTTPS, custom domains. Multi-page is better here because:
- Each project gets a **dedicated URL** you can link from resumes and applications
- Better for SEO (each page can target different keywords)
- Cleaner navigation — visitors aren't scrolling through everything

```
/ (Home / Landing Page)
├── Hero Section
│   ├── Name + headline (not "Full Stack Developer" — something specific)
│   ├── 1-2 sentence positioning statement
│   └── CTA buttons: Resume (PDF) | GitHub | LinkedIn | Contact
├── About Preview (short — links to /about for full version)
├── Featured Projects (3 cards — links to /projects/{name})
└── Quick contact / footer

/about
├── Your story: biomedical scientist → software engineer
├── What you do now and what drives you
├── Professional photo
├── Skills / expertise grouped by domain
└── Experience timeline (lightweight, links to resume PDF)

/projects (Gallery Page)
├── Project cards with screenshots/diagrams
├── Each card: title, one-liner, key metric, tech tags
├── Filter/sort by domain (AI/ML, Life Sciences, Embedded, etc.)
└── 4-6 curated projects (not a dump)

/projects/{project-name} (Individual Project Pages)
├── Problem statement — what needed solving and why
├── Approach — how you tackled it (concise, not a spec doc)
├── Results / impact — quantified where natural
├── Tech stack
├── Screenshots, diagrams, or demo GIFs
└── Links: GitHub repo, live demo (if applicable)

/contact
├── Email, LinkedIn, GitHub links
├── Location (McLean, VA)
└── "Open to opportunities" or "Available for consulting" note
```

---

## Content to Create

### Visuals Needed
- [ ] Professional headshot
- [ ] Project screenshots or architecture diagrams for each featured project
- [ ] Optional: short screen recordings / GIFs of tools in action

### Written Content Needed
- [ ] Hero headline + positioning statement
- [ ] About section (3-5 sentences, your voice)
- [ ] Project descriptions (problem → approach → result format)
- [ ] Skills section copy

### Project Showcase Candidates
Choose 4-6 from this list. Each gets its own /projects/{name} page:

| Project | Best For | Key Metric | Page Weight |
|---------|----------|------------|-------------|
| HyperSight | AI/ML, Full-Stack, Consulting | 64,300+ LOC, 100+ LLM providers | Featured |
| DARPA Triage Challenge | Clinical ML, Healthcare AI, Data Science | 0.938 AUROC, 327 GB data | Featured |
| Bioassay LIMS | Life Sciences, Scientific Software | 55K LOC, 20-100x speedup | Featured |
| Jira AI PM | AI/Automation, Productivity | Workflow automation | Standard |
| PlateHandler / Embedded | Automation, IoT, Robotics | ESP32, motion control | Standard |
| Grad Research (Astrocyte TBI) | Life Sciences, Clinical, Research | Tissue engineering, immunofluorescence | Shorter |

**Grad Research inclusion rationale:**
- Proves you're a scientist who codes, not just a developer who read some biology
- Strong differentiator for life sciences, clinical, and healthcare AI roles
- Shows bench work, tissue engineering, immunofluorescence — real lab credibility
- Shorter page format: research context, your contribution, techniques used, outcome
- Links to thesis/publication if available

**Content Status:**
- [x] Grad Research (Astrocyte TBI) — full project page content ready in `Projects/GRAD_RESEARCH_ASTROCYTE_TBI.md`
  - Headline, one-liner, problem/approach/results narrative, techniques, recommended figures from thesis
- [ ] HyperSight — needs project page narrative
- [ ] DARPA Triage Challenge — needs project page narrative
- [ ] Bioassay LIMS — needs project page narrative
- [ ] Jira AI PM — needs project page narrative
- [ ] PlateHandler / Embedded — needs project page narrative

---

## Design Direction

### Color Palette
- Clean, professional — dark navy / white / accent color
- NOT the typical developer "dark mode neon" aesthetic
- Should feel like a scientist's portfolio, not a bootcamp grad's

### Typography
- Clean sans-serif (Inter, Source Sans, or similar)
- Good hierarchy: clear headings, readable body text

### Layout
- Multi-page: landing page, about, project gallery, individual project pages, contact
- Each project gets its own URL (shareable, linkable from resumes)
- Mobile-first responsive

### Tone
- Confident but not boastful
- Technical but accessible
- Shows the person behind the work

---

## Implementation Phases

### Phase 1: Foundation
- Set up GitHub Pages repo
- Build landing page with hero, about, and contact sections
- Get the site live with basic content

### Phase 2: Project Showcase
- Create project detail content (descriptions, screenshots)
- Build project cards with click-through details
- Add 3-5 curated projects

### Phase 3: Polish
- Skills/expertise section
- Experience timeline
- SEO basics (meta tags, Open Graph for link previews)
- Custom domain (optional)

### Phase 4: Growth (Future)
- Blog section
- Consulting services page
- Case studies for consulting pitches

---

## Sources & Research

- [Survey of 60+ hiring managers on portfolio sites](https://dev.to/profydev/this-survey-among-60-hiring-managers-reveals-don-t-waste-your-time-on-a-react-portfolio-website-17ge)
- [What recruiters look for in developer portfolios](https://pesto.tech/resources/what-recruiters-look-for-in-developer-portfolios)
- [Personal branding for job seekers](https://blog.theinterviewguys.com/personal-branding-for-job-seekers/)
- [Portfolio guide: what to include and avoid](https://www.8seneca.com/en/blog/technology/software-engineer-portfolio-guide-what-to-include-and-what-to-avoid)
- [How recruiters actually look at portfolios](https://blog.opendoorscareers.com/p/how-recruiters-and-hiring-managers-actually-look-at-your-portfolio)
- [Developer portfolio templates 2026](https://templifica.com/blog/developer-portfolio-templates-creating-a-job-winning-portfolio)
- [Well-designed engineer portfolio examples](https://www.sitebuilderreport.com/inspiration/engineer-portfolios)

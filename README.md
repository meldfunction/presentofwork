# The Present of Work

You have been told a story about work your entire life. The story goes like this: find a job, show up, earn your place, repeat until you die or retire — whichever comes first. That story isn't natural law. Someone wrote it. And they wrote it for a reason.

**This site is the investigation.**

---

## What This Is

The Present of Work is an independent publication that refuses to treat "work" as a fixed fact of human existence. It is a deep excavation of how the modern relationship between human beings and their labour was constructed — through enclosure, through the Protestant ethic, through slavery's contribution to financial capitalism, through every Silicon Valley utopia that promised liberation and delivered a new kind of precarity.

Twenty-nine essays. Three series. One relentless question: *who decided this, and what would we choose instead?*

Everything is free to read. No paywall. No algorithm deciding what you see. Produced in the commons.

---

## The Publication

**Series I — The History of the Present**
Before the clock, before the factory, before the office — human beings had radically different relationships to time, contribution, and community. This series traces how selling your hours became a moral virtue rather than a historical accident. From medieval feast days to Amazon's bathroom-break algorithms. The line is shorter than you think.

**Series II — The Future of the Present**
Every decade brings a new promise: automation will free us, the internet will flatten hierarchies, the sharing economy will make us all entrepreneurs. It never quite works out that way. This series asks why every technological utopia still needs you to clock in — and who keeps collecting the upside when you don't.

**Series III — The Present ∞**
Not a manifesto. Not a five-point plan. A living, growing collection of what people are actually doing right now — cooperatives, care economies, mutual aid, degrowth, commons governance. The experiments that don't make the business press because they aren't optimising for shareholder return.

Read in any order. Start anywhere. Come back.

---

## The Site

| Page | Purpose |
|------|---------|
| `/` | Homepage |
| `/publication.html` | Full essay index across all three series |
| `/essays/` | Essay browser |
| `/essays/{slug}/` | Individual essays |
| `/podcast.html` | Field Notes podcast |
| `/concepts.html` | Conceptual map of ideas |
| `/map.html` | Geographic/relational map |
| `/ecosystem.html` | Directory of aligned organisations |

---

## Tech Stack

Jekyll, GitHub Pages, zero JavaScript frameworks. Fast, readable, owned.

- **Templating:** Liquid (Jekyll)
- **Markdown:** Kramdown + Rouge
- **Fonts:** Bebas Neue, Roboto Mono, Libre Baskerville
- **Styling:** CSS custom properties, light/dark mode

## Running Locally

```bash
bundle install
bundle exec jekyll serve
open http://localhost:4000
```

## Repository Structure

```
_essays/          # 29 essay markdown files (0.1 – 3.10)
_episodes/        # Podcast episode transcripts
_layouts/
  default.html    # Nav, footer, global styles
  post.html       # Individual essay template
essays/index.html # Essay browser (Liquid, uses _essays collection)
publication.html  # Full series index
index.html        # Homepage
```

## Contributing

Essays are markdown files in `_essays/` with YAML front matter:

```yaml
---
title: "Essay Title"
series: "Series I: The History of the Present"
series_num: "1.1"
layout: post
excerpt: "Opening paragraph..."
---
```

Filename determines URL: `_essays/1-1-my-essay.md` → `/essays/1-1-my-essay/`

Contact: [hello@presentofwork.org](mailto:hello@presentofwork.org)

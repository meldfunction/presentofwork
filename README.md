# The Present of Work

A publication, podcast, map, and gathering place for all forms of work — not occupational employment, but the full range of human contribution.

## What This Is

The Present of Work is an independent publication exploring what work actually is, how it came to be organised the way it is, and what we might choose instead. It asks a deceptively simple question: *what is work — really?*

The site hosts three interlocking essay series, a podcast, a conceptual map of ideas, and a living directory of organisations and communities doing things differently. Everything is produced in the commons and free to read.

## The Publication

Twenty-nine essays organised into three series:

**Series I — The History of the Present**
How did selling your time become the definition of a good life? Traces the genealogy of wage labour from pre-enclosure commons through the industrial revolution to the 20th-century office.

**Series II — The Future of the Present**
Why do all our promised futures still need you to earn your place in them? A reckoning with techno-utopian promises from the Jetsons to AGI.

**Series III — The Present ∞**
What if your worth was never up for negotiation? Plural economies, practices of resistance, new structures — ever-growing, no grand theory.

Essays are readable in any order. Start anywhere.

## The Site

| Page | Purpose |
|------|---------|
| `/` | Homepage |
| `/publication.html` | All three essay series with full essay index |
| `/essays/` | Essay browser by series |
| `/essays/{slug}/` | Individual essay pages |
| `/podcast.html` | Field Notes podcast |
| `/concepts.html` | Conceptual map |
| `/map.html` | Geographic/relational map |
| `/ecosystem.html` | Directory of aligned organisations |

## Tech Stack

Built with [Jekyll](https://jekyllrb.com/) and hosted on GitHub Pages. No JavaScript framework, no build pipeline beyond Jekyll's standard processing.

- **Templating:** Liquid (Jekyll)
- **Markdown:** Kramdown with Rouge syntax highlighting
- **Fonts:** Bebas Neue, Roboto Mono, Libre Baskerville (Google Fonts)
- **Styling:** CSS custom properties with light/dark mode toggle

## Running Locally

```bash
# Install dependencies
bundle install

# Serve with live reload
bundle exec jekyll serve

# Open in browser
open http://localhost:4000
```

## Repository Structure

```
_essays/          # 29 essay markdown files (numbered 0.1 – 3.10)
_episodes/        # Podcast episode transcripts
_layouts/
  default.html    # Site-wide nav, footer, scripts
  post.html       # Individual essay template
essays/
  index.html      # Essay browser (Liquid template, uses _essays collection)
publication.html  # Full publication page with series index
index.html        # Homepage
about.html
podcast.html
concepts.html
map.html
ecosystem.html
```

## Contributing

Essays are markdown files in `_essays/` with YAML front matter:

```yaml
---
title: "Essay Title"
series: "Series I: The History of the Present"
series_num: "1.1"
layout: post
excerpt: "Opening paragraph text..."
---
```

The filename determines the URL: `_essays/1-1-my-essay.md` → `/essays/1-1-my-essay/`.

Contact: [hello@presentofwork.org](mailto:hello@presentofwork.org)

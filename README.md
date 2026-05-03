# The Present of Work

> *"Amazon's fulfillment centers track worker productivity in increments of fractions of a second. Algorithms monitor the time between scans. A worker who spends too long in the bathroom triggers an alert."*

This is not a dystopian novel. This is Tuesday.

And it didn't start with Amazon. It started roughly five hundred years ago — as a fight. This site is the investigation of how we got here, who made the choices that got us here, and what people are doing right now to make different ones.

---

## Things You Probably Weren't Taught

**Wall Street is named after a wall built by enslaved people to protect Dutch merchants.** The financial architecture of modern capitalism — Lloyd's of London, the VOC, the New York Stock Exchange — was underwritten by the plantation. The plantation was the proto-factory. This is not ancient history. It is the foundation.

**The five-day work week was a corporate invention, not a labour victory.** Henry Ford introduced it in 1926 to create more consumers with more leisure time to spend money. The weekend is a market mechanism.

**Medieval peasants worked fewer hours per year than you do.** Between feast days, saint's days, and seasonal rhythms, the average 14th-century English agricultural worker had somewhere between 8 and 12 weeks of non-working days annually — not counting the hours lost to rain, prayer, and communal obligation. The clock hadn't colonised labour yet.

**"Vocation" once meant a calling from God.** Weber traced the Protestant Reformation's transformation of *Beruf* — the German word for both "calling" and "occupation" — into a theological endorsement of hard work as a sign of grace. Hustle culture is five hundred years old. It has a church.

**The word "unemployment" didn't exist before the 1880s.** You can't be unemployed if work isn't yet a category separate from the rest of life. The concept required the factory, the wage, and the clock to precede it.

---

## Why This Matters Right Now

**The layoffs aren't a bug.** In 2022–2024, over 500,000 tech workers were laid off by companies that had collectively added trillions in market capitalisation. The workers who built those platforms were removed the moment the platforms no longer needed them to scale. This is not a market correction. It is the logical endpoint of treating labour as a variable cost rather than a constituent of the enterprise.

**AI is the newest version of an old promise.** Every wave of technology — mechanisation, electrification, computing, the internet, the sharing economy — promised to liberate workers from drudgery. Each one restructured who captures the gains. The current wave of large language models and automation is not categorically different. The question is not whether AI will change work. It is who will own the productivity it creates.

**"Just become an entrepreneur" is not a solution.** The gig economy rebranded precarious piecework as freedom. TaskRabbit, Uber, Deliveroo: the sharing economy's broken promise was that platform capitalism dressed contingency labour in the language of autonomy. When the algorithm sets your rate, you are not your own boss.

**Care work is the largest economy you've never heard of.** Unpaid reproductive labour — childcare, eldercare, domestic work, emotional support — underpins every other form of economic activity. It is performed disproportionately by women, disproportionately by women of colour, and it does not appear in GDP. Feminist economists have been saying this for fifty years. The mainstream has not caught up.

---

## The Publication

Twenty-nine essays. Three series. One question that gets harder to answer the longer you sit with it: *what is work, really?*

**Series I — The History of the Present**
Before the clock, before the factory, before the performance review — human beings had radically different relationships to time, contribution, and community. This series traces how selling your hours became a moral virtue rather than a historical accident. From the commons to the cubicle. From *ayni* — Quechua reciprocal labour with no ledger and no time horizon — to the Amazon warehouse bathroom alert.

*You are living in this series every time a manager talks about "productivity culture" as if it were a law of nature.*

**Series II — The Future of the Present**
The Jetsons promised a 2-hour workday by 1990. The internet was going to flatten hierarchies. The sharing economy was going to make everyone an entrepreneur. AGI is going to do — what exactly? Each wave of techno-utopianism recycles the same script with higher stakes and the same distribution of gains. This series asks why every promised future still needs you to clock in.

*You are living in this series every time a CEO announces layoffs the same quarter they announce record profits.*

**Series III — The Present ∞**
Not a manifesto. Not a five-point plan. A living, growing collection of what people are actually building right now — worker-owned cooperatives, care economies, mutual aid networks, degrowth communes, commons governance. The experiments that don't make the business press because they aren't optimising for shareholder return. No grand theory. Many honest experiments.

*You are living in this series every time you wonder if there's a different way to organise things — and then discover someone already is.*

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

Everything is free to read. No paywall. Produced in the commons.

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

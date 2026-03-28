# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## What This Repository Is

**marxFromANewEngels** is a personal knowledge base and political education resource, published as a static site via Jekyll (GitHub Pages, `jekyll-theme-hacker`). It is not a software project — there are no build steps, tests, or linting pipelines.

Content spans political theory, personal development, and practical life guides. The name frames the project as reinterpreting Marxist theory for a new audience — accessible, clear, and grounded in practice.

Source material was originally imported from `dessalines/essays` and is being extended and personalized here.

**Editing workflow:** Edit markdown files directly → preview locally → commit via git.

For full formatting rules, naming conventions, and tone guidelines, see [`AGENTS.md`](AGENTS.md).

---

## Content Map

### Root directory (~25 files) — Political theory and reference
Primary content: socialist/Marxist theory essays, glossaries, FAQs, historical documentation, and media/resource lists.

Key files:
| File | Purpose |
|------|---------|
| `crash_course_socialism.md` | Entry point for new readers; broad introduction |
| `socialism_faq.md` | Comprehensive FAQ (247 KB) |
| `glossary_of_socialist_terms.md` | Term definitions (~3 sentences each) |
| `us_atrocities.md` | Historical documentation list (374 KB) |
| `capitalism_doesnt_work.md` | Core critique essay |
| `dessalines_marxism_study_plan.md` | Structured reading curriculum |
| `audiobooks.md` | Curated socialist audiobooks with magnet links |
| `whatAreWeAbout.txt` | Manifesto-style introduction (ELI10 rewrite of *The Communist Manifesto*) |
| `README.md` | Site landing page / navigation index |

Other root essays cover: Lenin's strategy (`lenin_lwc.md`), cyber-communism (`paul_cockshott_cyber_communism.md`), Nietzsche critique (`nietzsche.md`), ACAB (`acab.md`), Star Trek and communism (`star_trek_communism.md`), Microsoft critique (`microsoft.md`), privacy (`why_not_signal.md`), torrenting (`how_to_torrent.md`), China/Deng analysis (`supercooper_china_deng.md`).

### `recipes/` (27 files) — Vegan/vegetarian cooking
Plant-based staples: beans, lentils, tofu, tempeh, chickpeas, falafel, fried rice, sourdough, pizza, ramen, hibiscus tacos, plus beverages (coffee, green tea, oat milk, flavored waters, beer brewing).

### `buddhism/` (4 files) — Buddhist study and practice
`buddhism_study_guide.md`, `meditation.md`, `buddhist_questions.md`, `mind illuminated 10 stages.md` (note: this filename has spaces — a known naming inconsistency).

### `language_learning/` (2 files) — Language study guides
`mandarin_guide.md`, `toki_pona_guide.md`.

### `reviews/` (5 files) — Book and media reviews
Lenin's *Imperialism*, Zak Cope's *Divided World Divided Class*, *The People's Republic of Walmart*, Barbie movie essay, JS imperialism favorites.

### `routines/` (4 files) — Personal development
`goals.md`, `routines.md`, `tank_energy.md` (health/energy optimization), `workout_routine.md`.

---

## Link Paradigm

This site is rendered by Jekyll, so `.md` files become HTML pages. Links should follow these rules:

- **Internal links**: Relative paths with `.md` extension — e.g., `[Crash Course Socialism](crash_course_socialism.md)` or `[Glossary](../glossary_of_socialist_terms.md)` from a subdirectory.
- **External links**: Full absolute URLs.
- **No wikilinks**: This is standard CommonMark — no `[[double-bracket]]` syntax.
- **Descriptive link text**: Avoid "click here" or bare URLs as link text.
- **`README.md`** is the site's root landing page. It is what GitHub Pages renders at `/`.

---

## Editorial Standards (Summary)

Full rules in [`AGENTS.md`](AGENTS.md). Quick reference:

- **Audience**: ELI10 accessibility for glossary and introductory content; more depth acceptable in long-form essays
- **Tone**: Scholarly but accessible; avoid jargon without defining it
- **Sources**: Link to Wikipedia or authoritative sources when introducing concepts
- **Headers**: ATX style (`#`, `##`, `###`)
- **File names**: `snake_case.md`
- **Grammar**: Oxford commas; inclusive, non-discriminatory language

---

## Improvement Roadmap

The following are known gaps and polish tasks — work through these incrementally.

### High priority
- [ ] **Expand README navigation** — `README.md` only links to political theory content; `recipes/`, `buddhism/`, `routines/`, `language_learning/`, and `reviews/` sections are entirely absent from the landing page
- [ ] **Convert `whatAreWeAbout.txt` to `.md`** — rename the file and link it from README as the project introduction
- [ ] **Rename `buddhism/mind illuminated 10 stages.md`** — spaces in filename violate naming conventions; rename to `mind_illuminated_10_stages.md` and update any internal links

### Medium priority
- [ ] **Add subdirectory index files** — `recipes/README.md`, `buddhism/README.md`, etc. so each section has a navigable entry point
- [ ] **Cross-link essays ↔ glossary** — essays should link to glossary definitions on first use of key terms; glossary entries should link back to essays where terms are explored in depth
- [ ] **Audit internal links in README** — verify every link in `README.md` resolves to an actual file at its stated path

### Lower priority / ongoing
- [ ] **Personalize imported content** — files from `dessalines/essays` may need voice/perspective edits to fit this project's framing
- [ ] **`assets/style.scss`** — minimal styling; could improve typography and readability for long-form reading
- [ ] **Add a "start here" guide** — a single recommended reading path for new visitors across the full knowledge base (theory → practice → personal development)
- [ ] **`favorite_apps_and_services.md`** — consider whether this belongs in root or a new `resources/` or `tools/` subdirectory

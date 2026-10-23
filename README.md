# Racknotes

Pre-launch landing page for **Racknotes** — a curiosity-driven lab log about homelab and self-hosting, AI in practice, and emerging tech.

**Positioning:** I run tomorrow's tech in my own rack and tell you whether it survives — the numbers, the failures, and the receipts.

## Brand idea

Racknotes is a blogging + digital content brand around technology, homelab/self-hosting, AI, and emerging tech. Monetized via affiliate links, display ads, and digital marketing/video. Goal: $100/month as a proof-of-viability milestone, not a ceiling.

Core principle: **curiosity over hype** — "document the experiment, not the announcement."

News is raw material, not the product. No pillar ships an announcement without an attached experiment. Every piece ends with a verdict: Buy / Wait / Skip.

### Content pillars (current strategy)

| Pillar | Scope | Share of output |
|--------|-------|-----------------|
| **Patch Notes** | The rack's changelog — what changed, broke, and stayed | ~50% (flagship) |
| **Model Behavior** | Local models, real workflows, failure modes | ~25% |
| **First Contact** | 30-day tests of genuinely new tech | ~15% |
| **Field Notes** | Biweekly dispatch; news lives here as curation | ~10% |

Cadence: Weekly (not daily). Run three experiments in parallel, publish serially. ~6–9 hrs/week.

Entertainment: Yes, but for retention, not reach. 20% wrapper / 80% substance.

### Target audience
- The Sovereign Tinkerer
- The Career-Curious Technologist

### Visual identity
- Ink `#141414`, cream `#F4EFE6`, signal amber `#D98E3A`, muted terminal green `#7FB069`
- Typefaces: Fraunces (headings) + Inter (body) + JetBrains Mono (labels/code)

## Status

Pre-launch. Single-page launch site with an email waitlist.

## Structure

- `index.html` — the entire site (inline CSS + JS, no build step)
- `.nojekyll` — lets GitHub Pages serve the file tree as-is

## Local development

No build step. Either open `index.html` directly in a browser, or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Known TODOs before real launch

- [ ] Connect the two email signup forms to a provider (Buttondown, MailerLite, ConvertKit, or Formspree). Currently in demo mode: they show a message and do not submit anywhere.
- [ ] Remove `data-demo` from both `<form>` elements and delete the demo `querySelectorAll` block at the bottom of `index.html`.
- [ ] Replace placeholder social links in the footer (currently `href="#"`).
- [ ] Update `hello@racknotes.dev` if the real contact address differs.
- [ ] Reconcile the content pillars in the HTML (currently shows the older 5-pillar names; strategy is now 4 pillars — see table above).
- [ ] Add a real OG image (`og:image` meta tag is not yet set).

## License

Content © Racknotes. Code is not currently licensed for reuse.

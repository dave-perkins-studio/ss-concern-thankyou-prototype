# Concern Worldwide — attribution question prototypes

Six approaches to one question — *"What motivated your contribution today?"* —
switchable from a bar at the top of the page. Published so it can be sent as a
link.

**Live:** https://dave-perkins-studio.github.io/ss-concern-thankyou-prototype/

| Tab | Approach |
|---|---|
| A | Dropdown — what is live today |
| B | Radio list |
| C | Chips |
| D | Two-step |
| E | Typeahead |
| F | Off the form entirely, on the thank-you page after payment |

A to E change the **control**, in the real Address step of the monthly donation
form. F changes **where the question is asked**, and frames the whole thank-you
page.

This repo is **public only to serve the page**. It holds nothing but the built
prototypes. The project they belong to — the brief, the deck, the research, the
QA reports and the decisions journal — stays private in
`dave-perkins-studio/ss-concern-attribution`.

## Not an official Concern build

These are SystemSeed design prototypes. The Concern branding is a
reconstruction, made so the question can be judged in its real surroundings;
photography and illustration are placeholders, and each page carries that
notice in its footer. Both are marked `noindex, nofollow` so they will not be
indexed as Concern's own pages.

## Files

| Published | Source of truth in `ss-concern-attribution` |
|---|---|
| `index.html` | `design/prototypes/attribution-variants.html` |
| `thank-you-attribution.html` | `design/prototypes/thank-you-attribution.html` |

Tab F frames `thank-you-attribution.html` by relative path, which is why that
file keeps its name here rather than being renamed.

## Do not edit these files directly

They are **copies**. Edit the sources above, then republish from that repo:

```bash
./tools/publish-prototype.sh
```

`--check` exits non-zero if a published copy has drifted from its source.
Editing a copy here means the next publish silently overwrites your work.

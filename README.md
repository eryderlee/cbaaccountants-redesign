# CB Accountants — Redesign

A static marketing site for CB Accountants — Australian-registered tax agent and IPA member.

**Live URL:** _set after first Netlify deploy_
**Repo:** https://github.com/eryderlee/cbaaccountants-redesign

## Stack
Plain HTML + CSS + small vanilla-JS for the drawer, scroll header, and reveal animations. No build step required.

- `index.html` — homepage (the cinematic dark-navy hero, services, audiences, why-us manifesto, testimonials, about, insights, final CTA)
- `book.html` — booking / contact page (form + alternative contact methods)
- `cb-logo.png` — CB monogram (used inline)
- `netlify.toml` — Netlify build + headers config

## Design system

All tokens derive from the CB logo (deep navy `#001A4A`). The accent (`#3B6FDB`) is the same hue lifted to a clear electric blue. Backgrounds are cool icy off-white (`#F1F4F9`). Typography: **Geist** display + **Inter** body + **Geist Mono** for tags / dates / labels.

| Token | Value | Use |
|---|---|---|
| `--ink-1` | `#001A4A` | Primary text, monogram, dark backgrounds |
| `--paper-1` | `#F1F4F9` | Page background |
| `--accent-1` | `#3B6FDB` | Buttons, links, focus |

The double-navy rounded outline that frames the hero card + about portrait directly mirrors the logo's rounded-square stroke.

## Local dev

```bash
# Any static server works
python -m http.server 8765 --bind 127.0.0.1
# Then open http://127.0.0.1:8765
```

## Deploy

Netlify auto-deploys from the `main` branch. `netlify.toml` is at repo root.

## Open items

See `OWNER-CONFIRMATIONS.md` for content the owner still needs to confirm before launch (real testimonials, owner portrait, ABN, etc.).

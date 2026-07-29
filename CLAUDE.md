# The Underline — event website

One-page event site for **The Underline** (World Cup Weekend event) — a
Productions client. Static HTML, deploys via **GitHub Pages**.

- Public URL: https://avant-garde-factory.github.io/underline-website/
- Renamed from `agp-theunderline-website` on 2026-07-29. Because this is a
  GitHub Pages project site, that rename changed the public URL — if the old
  address is linked anywhere, point it here (or give this repo a custom domain).


<!-- ═══════════════════════════════════════════════════════════════════
     SHARED AVANT GARDE FACTORY HOUSE RULES  —  do not edit this block here.
     Canonical source: avant-garde-factory/standards/HOUSE-RULES.md
     (also baked into the launchpad-site-template).
     To change a rule: edit it in `standards`, then re-sync every repo's copy.
     ═══════════════════════════════════════════════════════════════════ -->

# Avant Garde Factory — house rules (shared across all repos)

These rules are the same in every AGF repo so Michael, Rico, and any cloud or
scheduled agent all work the same way. Your personal preferences (tone,
token-saving, etc.) belong in your own `~/.claude/CLAUDE.md`, never here.

## The units (each is its own standalone business)

Avant Garde Factory is the umbrella. The units refer work to each other and
their scopes can overlap, but none is a sub-brand or "counterpart" of another.

- **Launchpad** — creative agency. Its job is **creating and managing company
  websites** (plus web, social, photo, video, print). Launchpad builds the
  sites; a site repo is named for the brand it's *for*, not for Launchpad.
- **Productions (AGP)** — event production & rental: staging, lighting, sound,
  rigging, event build-out, rentals.
- **Media (AGM)** — photo & video production. Already live and earning.

## Check `standards` before researching

`avant-garde-factory/standards` holds researched, cited decisions so the same
question never gets researched twice. **Before any research pass or real
design/UX/technical judgment call, check that repo's `README.md` index first.**
If a decision covers the situation, use it and say you did. If it doesn't, say
so plainly and do fresh research — then add a cited decision back to `standards`
(copy `decisions/TEMPLATE.md`). Don't wait to be asked.

## Repo naming: `brand-type`

Lowercase, hyphenated, **no `ag`/`agl`/`agp` prefixes** (the org name already
carries "Avant Garde").

- **brand** = whose it is — a unit (`launchpad`, `productions`, `media`) or a
  client (`reflections`, `underline`). Named for who it's *for*, not who built it.
- **type** = `website`, `portal`, `clients`, `template`.
- **Other work** (social, print, photo for a client) gets **its own repo**, or a
  folder inside `launchpad-clients` — never crammed into a website repo.
- `standards` and `.github` stay bare — they're org-wide singletons, not brand repos.

## House style: start every new site from the template

Every new Avant Garde site starts from **`launchpad-site-template`** (the tokens
+ component + layout system). Don't reinvent the layout system per project.
Stack: **Astro** static output → **Cloudflare Pages**, git-connected (push to
`main` rebuilds the site).

## Never commit

Secrets, API keys, tokens, `.env` files — use the host's environment variables.
No raw media (photos/video/footage) — that lives in Google Drive, not git.

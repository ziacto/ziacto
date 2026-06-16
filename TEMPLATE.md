# Make this profile yours — in 15 minutes

This profile README is hand-crafted by [@ziacto](https://github.com/ziacto) and open to fork. Here's the customization map.

> _If you use it, a credit link in your README would mean a lot — but no obligation. Pay it forward by leaving the next fork better than you found it._

---

## Quick start

```bash
# 1. Create your own profile repo (named exactly like your GitHub username)
# 2. Click "Fork" on github.com/ziacto/ziacto OR copy these files manually:
README.md
TEMPLATE.md            # (optional — delete or keep)
assets/banner.svg
assets/*.png           # your product / project icons
.github/workflows/*.yml
```

If you don't already have a special profile repo: GitHub auto-detects a public repo with the exact name as your username and renders its README on your profile page. Create one and copy the files in.

---

## What to change (priority order)

### 🔴 MUST change

| File | What | Where |
|---|---|---|
| `README.md` | Every `ziacto` → your GitHub username | search & replace |
| `README.md` | Every `Zia Shahid` / `ziagaggoo@gmail.com` / LinkedIn URL → yours | search & replace |
| `assets/banner.svg` | `ZIA SHAHID` text → your name | line ~70 |
| `assets/banner.svg` | `CHIEF TECHNOLOGY OFFICER` → your title | line ~73 |
| `assets/banner.svg` | The 3 tower labels (`UAE_PASS`, `DUBAI_NOW`, `BUZDY`) | search the file |
| `assets/*.png` | Your product / project icons (240×240 PNG) | replace in place |
| `.github/workflows/metrics.yml` | Add a `METRICS_TOKEN` repo secret (PAT with `repo, read:org, read:user, read:packages`) | one-time GitHub setting |

### 🟡 SHOULD change

- The whole **"Hi, I'm \[Name]"** intro paragraph
- The YAML **identity card** block
- All section content (timeline, products, founder's lens, credentials, etc.)
- The **typing SVG** at the top (`readme-typing-svg.demolab.com?...&lines=...`) — encode your own lines
- Status pill badges — your real availability / location / response time
- Mermaid diagrams: mindmap (skills), timeline (career), pie (time allocation)

### 🟢 NICE to change

- Gradient colour palette in the banner (`#ff009d → #ff5e62 → #00b4d8 → #6a4c93 → #ff9000`). Pick yours at <https://capsule-render.vercel.app>
- Section emoji icons (🧭 👥 🏗️ 🛡️ 🗣️ ⚒️) — pick what fits your taste
- The "I Wrote the Book" section — swap for your own signature artifact (talk, OSS repo, course, podcast)

---

## File-by-file walkthrough

### `README.md`

The single source for the rendered profile. Structure:

```
1. Banner (links to ./assets/banner.svg)
2. Status pills (4 — symmetric)
3. Typing SVG intro
4. Action buttons (4 — symmetric)
5. Stats badges (4 — symmetric)
6. Opening quote
7. "Hi, I'm ___" paragraph + YAML identity
8. "What I Do as [Role]" — 3×2 icon grid
9. Signature artifact (book, talk, OSS) — your hero credential
10. Mermaid mindmap (skills)
11. Products / projects (3 cards)
12. Founder/Solo project spotlight
13. Mermaid timeline (career arc)
14. Mermaid pie chart (time allocation)
15. "How I Operate" — collapsible field notes
16. Mission Control (GitHub stats widgets)
17. The Workshop (tech badges, collapsible by category)
18. Credentials & receipts (3-col grid)
19. Let's Talk (contact row)
20. Fork CTA + footer
```

Keep the symmetry: **groups of 3 or 4 always.** Mixed counts read as noise.

### `assets/banner.svg`

A 1200×380 hand-coded SVG with:
- A 5-stop colourful gradient backdrop (matches the capsule-render footer)
- A dark overlay for text readability
- 16 twinkling animated stars
- A skyline silhouette (back layer + mid layer)
- 3 featured "towers" (your flagship projects)
- Animated data-flow lines between towers
- A monogram in the top-left, status indicator in the top-right
- A vertical scan-line animation

**Tower customisation:** each tower has `<text>` label + body rectangle. Search for `UAE_PASS`, `DUBAI_NOW`, `BUZDY` and replace with your projects.

### `.github/workflows/`

Three GitHub Actions that auto-generate dynamic widgets daily:

- **`snake.yml`** — generates a "snake eats contributions" SVG on the `output` branch. No setup needed beyond the default `GITHUB_TOKEN`.
- **`metrics.yml`** — generates a multi-plugin metrics megacard (`github-metrics.svg`). **Requires** a repo secret named `METRICS_TOKEN` (classic PAT with `repo, read:org, read:user, read:packages`).
- **`3d-contrib.yml`** — generates a 3D contribution cube under `./profile-3d-contrib/`. No setup needed.

After forking and first push, manually trigger each from the **Actions** tab once to populate.

### `assets/*.png`

Square 240×240 PNGs work best at the `width="128"` displayed in the README. Sources for app/project icons:
- Play Store CDN: `https://play-lh.googleusercontent.com/<hash>=w240-h240`
- App Store: scrape from product page
- Or generate with Figma / Affinity / Excalidraw

---

## Pitfalls others have hit

- 🔴 **Don't use `ansi` as a code-fence language** — GitHub mis-parses `[ ok ]` style markers as ANSI escape sequences and cascades the indentation. Use plain code fences with `✓` or `→`.
- 🔴 **Don't URL-encode emoji into shields.io badge URLs** — shields.io uses Verdana which lacks colour-emoji glyphs. Use `logo=` params instead.
- 🟡 **Don't use `github-readme-streak-stats.herokuapp.com`** — retired free tier. Use `streak-stats.demolab.com` (Vercel mirror).
- 🟡 **Don't rely on `gstatic.com/encrypted-tbn0` image URLs** — they rotate and 404. Save icons locally to `./assets/`.
- 🟡 **Avoid fake testimonial sections** — paraphrased quotes from "a colleague, probably" undermine credibility. If you don't have real ones, skip the section.
- 🟢 **Mermaid blocks must be top-level markdown** — wrapping them in `<div>` or `<table>` cells can break rendering.

---

## Credits

Hand-crafted by [Zia Shahid](https://github.com/ziacto) · CTO, founder, and author of [The Unicorn CTO](https://www.amazon.com/Unicorn-CTO-Fastest-route-developer-ebook/dp/B0994S3TF8).

Forks welcome. Build something even better — and tag me when you do.

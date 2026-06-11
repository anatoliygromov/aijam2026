# 🚀 AI Jam — get set up in 5 minutes

Two tools: **Claude (Cowork)** to build your page, **GitHub Desktop** to publish it.
You will **not** write any code by hand — you prompt Claude, Claude writes it.

**Repo:** `github.com/anatoliygromov/aijam2026` · **Live site:** `anatoliygromov.github.io/aijam2026/`

---

## Setup (one-time)

1. **Accept the invite.** Click the link in the email → **Accept invitation** on GitHub. You're now a collaborator.
2. **Install GitHub Desktop** and **sign in** with your GitHub account. (This handles the publish login for you — no tokens, no terminal.)
3. **Clone the repo:** in GitHub Desktop, **File → Clone repository → GitHub.com →** pick `aijam2026` → choose a folder → **Clone.**
4. **Connect that folder in Claude:** open Claude (Cowork) and connect the cloned folder. Claude can now read & edit your page.

---

## Build & publish loop

5. **Build by prompting.** Open your team's brief at `teams/team-N.md` (your number) — it has your page, theme, required tech, and a paste-ready prompt. Paste it into Claude, swap in your inspiration, and let it build. Review, re-prompt, repeat until it slaps.
6. **Add visuals** as **URLs**: generate images in our agreed image tool and paste the links; load 3D models/textures from a **CDN**; synthesize audio in code. (See the asset rule below.)
7. **Commit:** in GitHub Desktop you'll see your changed file → type a short summary → **Commit to main.**
8. **Push:** click **Push origin.** This uploads it and makes it live.
9. **Verify:** wait ~30–60s, refresh the live site, check your page. Repeat 5–8 to keep iterating.

---

## 📏 The rules that matter

- **Edit only your own page file. Never touch `nav.css` or `nav.js`.** That shared nav is the seam holding all four pages together.
- **No local asset files.** Load images as URLs, 3D/textures from a CDN, audio generated in code. Keeps publishing fast and avoids size limits. (Need a local file? Commit it via GitHub Desktop — never the connector.)
- **Images are bring-your-own.** Claude doesn't generate images here — use the image tool we agree on and paste URLs.

## 🎬 Your page, theme & required tech

| Team | Members | File | Theme | Required tech |
|---|---|---|---|---|
| 1 🪓 | Essie · Nastya · Susanne | `index.html` | Epic Norse saga | WebGL 3D (three.js) |
| 2 🏛️ | Jon · Ella | `about.html` | Grand historical era | Scroll-driven animation |
| 3 🃏 | Anton · Lona | `team.html` | Collectible trading cards | CSS 3D transforms |
| 4 🕵️ | Sandy · Markus | `contact.html` | Spy dead-drop | GLSL fragment shader |

Your **theme and tech are set**; your **inspiration is open** — pull the look from any films, books, music or plays in that world. Your full brief + paste-ready prompt is in **`teams/team-N.md`**.

---

> ⚡ **Optional power-user shortcut:** if you've enabled the GitHub connector in Claude *and* tested that it commits straight to `main`, you can skip GitHub Desktop and just ask Claude to commit. If you haven't tested it, use GitHub Desktop — it's the reliable path.

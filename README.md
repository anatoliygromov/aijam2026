# 🎬 Umain AI Jam — The Exquisite Corpse

Four teams each build **one page** of the Umain website — blind to each other — each with a
**set theme**, free to draw inspiration from any **films, books, music or plays** in that
world. Every page pulls in one shared nav (`nav.css` + `nav.js`), so four wildly different
worlds still snap together under the same header. Then we open the live site and click through.

**Format:** 45–60 min · 9 people · 4 teams (3 pairs + a trio) · Tools: Claude (Cowork) + GitHub Desktop + an image-gen tool (no Figma)

---

## 🌐 The live site

Once GitHub Pages is on, the site is live here:

> **https://anatoliygromov.github.io/aijam2026/**

It already works from minute zero — every nav link is wired, the pages are just
placeholders waiting for each team to replace them.

---

## 🧩 The pages & teams

Theme + tech are set per team; inspiration is open — pull from any film, book, album or play.
Each team's full brief (theme, tech, prompt) lives in **`teams/team-N.md`** — open only yours.

| Team | Team members | Page | File | Theme | Required tech |
|------|--------------|------|------|-------|---------------|
| 1 | Essie · Nastya · Susanne | Homepage | `index.html` | Epic Norse saga | WebGL 3D (three.js) |
| 2 | Jon · Ella | About Umain | `about.html` | Grand historical era | Scroll-driven animation |
| 3 | Anton · Lona | Design Team | `team.html` | Collectible trading cards | CSS 3D transforms |
| 4 | Sandy · Markus | Contact | `contact.html` | Spy dead-drop | GLSL fragment shader |

(The `404.html` page stays as the site's default fallback — no team works on it.)

---

## 📜 The 3 rules

1. **Edit only your own page file** — and only the part between the `▼▼▼ … ▲▲▲` markers.
   Keep the filename.
2. **Never touch `nav.css` or `nav.js`.** That's the shared nav: it's injected into every
   page and auto-highlights the current one. Leave the two nav lines in your file exactly
   as they are.
3. **One self-contained page, no build step.** Put your CSS in the `<head>` or inline and
   JS in the page or from a **CDN**. Pull assets from **URLs/CDN** or data-URIs — or, if you
   need to ship a local file (3D model, texture, audio), drop it in your **`assets/teamN/`**
   folder and reference it relatively (e.g. `assets/team1/scene.glb`). No bundler, no Figma.

## 🧱 How it's wired

The nav lives in **one place** — `nav.css` (styles) and `nav.js` (markup + active-link
logic + the mobile menu). Each page is a thin shell that links both and drops a single
`<div id="umain-nav"></div>` placeholder; `nav.js` fills it and marks the active link by
filename. So the nav is identical everywhere, no team can break it, and a change to the
nav means editing one file — not five.

Repo files: `index.html` · `about.html` · `team.html` · `contact.html`
(the four team pages) + `404.html` (default fallback, left as-is) + `nav.css` · `nav.js` ·
`logo.svg` (shared — hands off). Per-team briefs live in **`teams/team-N.md`**.
Prefer CDN / procedural assets and image URLs — no local files needed.

---

## 🛠️ How each team works & publishes (no terminal needed)

1. **Set up** — accept the GitHub invite, **Clone** the repo in GitHub Desktop, then connect
   that folder in **Claude (Cowork)**. (Full steps in `ONBOARDING.md`.)
2. **Build with Claude** — open your brief at `teams/team-N.md`, paste its prompt, pick your
   inspiration, iterate. Claude edits your page directly; images come in as URLs.
3. **Publish** — in **GitHub Desktop**: write a summary → **Commit to main** → **Push origin**.
4. Wait ~30–60s, refresh the live URL. Your page is on the real site. 🎉

> Power-user option: if you've tested that the GitHub connector can commit to `main`, you can
> skip GitHub Desktop and have Claude commit directly.

---

## 🎤 The reveal

Open the live URL on the big screen and walk the pill nav: **Home → About Us → Product Design Team → Contact**. Four worlds, one set of seams.

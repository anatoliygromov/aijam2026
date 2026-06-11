# 🎬 Umain AI Jam — The Exquisite Corpse

Five teams each build **one page** of the Umain website — blind to each other — in the
aesthetic of a **film of their choosing**. Every page pulls in one shared nav
(`nav.css` + `nav.js`), so five wildly different film worlds still snap together under the
same header. Then we open the live site and click through.

**Format:** 45–60 min · 10 people · 5 teams of 2 · Tools: Claude + image gen (no Figma)

---

## 🌐 The live site

Once GitHub Pages is on, the site is live here:

> **https://anatoliygromov.github.io/aijam2026/**

It already works from minute zero — every nav link is wired, the pages are just
placeholders waiting for each team to replace them.

---

## 🧩 The pages & teams

| Team | Page | File | Vibe | Pick a film like… |
|------|------|------|------|-------------------|
| 1 | Homepage | `index.html` | Epic Norse saga | The Northman, How to Train Your Dragon |
| 2 | About Umain | `about.html` | Grand historical era | Marie Antoinette, Gladiator, Barry Lyndon |
| 3 | Design Team | `team.html` | Collectible trading cards | Into the Spider-Verse, Ocean's Eleven |
| 4 | Contact | `contact.html` | Spy dead-drop | Mission: Impossible, James Bond, Kingsman |
| 5 | 404 | `404.html` | Film-noir crime scene | Sin City, Chinatown, Blade Runner |

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

Repo files: `index.html` · `about.html` · `team.html` · `contact.html` · `404.html`
(the five team pages) + `nav.css` · `nav.js` · `logo.svg` (shared — hands off).
Each team also has an **`assets/teamN/`** folder for any local files they want to ship
(optional — most pages won't need it).

---

## 🛠️ How each team works & publishes (no terminal needed)

1. **Get your starter** — open your file on GitHub, click **Raw**, copy everything.
2. **Build with Claude** — paste it in, use your team card's prompt, pick your film, iterate.
   Get images from your image-gen tool as URLs and drop them in.
3. **Publish back** — on GitHub open your file → click the **✏️ pencil (Edit)** →
   select all → paste your finished HTML → **Commit changes** to `main`.
4. Wait ~30–60s, refresh the live URL. Your page is on the real site. 🎉

> Git-comfortable? Same idea: `clone` → edit only your file → `commit` → `push`.

---

## 🎤 The reveal

Open the live URL on the big screen and walk the pill nav: **Home → About Us → Product Design Team → Contact → 404**. Five films, one set of seams.

## 🏆 Awards (pick 3–4)

- **Most on-brief** — nailed the film world completely
- **Most unhinged** — went furthest off the deep end
- **Would actually ship** — secretly kind of great
- **Best whiplash** — funniest jump from the page before it

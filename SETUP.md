# ⚙️ Facilitator setup — ~10 min, do this before Thursday

You only do this once. After it, every team commit auto-publishes to the live URL.

## 1. Create the repo
- Go to github.com → **New repository**.
- Name: `aijam2026` · Visibility: **Public** (required for free Pages + a public URL).
- Create it.

## 2. Upload the site
- On the repo page: **Add file → Upload files**.
- Drag in **all** the files from this folder — including the shared nav files:
  `index.html`, `about.html`, `team.html`, `contact.html`, `404.html`,
  `nav.css`, `nav.js`, `logo.svg`, the `teams/` folder, `README.md`, `ONBOARDING.md`,
  `PRESENTATION.md`, `SETUP.md`.
- **Commit changes.**

## 3. Turn on GitHub Pages
- **Settings → Pages.**
- **Source:** Deploy from a branch → Branch: **`main`**, folder: **`/ (root)`** → **Save.**
- Wait ~1 min. The page shows your live URL:
  **`https://anatoliygromov.github.io/aijam2026/`**

## 4. Verify
- Open the URL. You should see the placeholder homepage with a working nav.
- Click each nav item — every page should load (Home · About Us · Product Design Team · Contact · 404).

## 5. Live now ✅
- Site: **https://anatoliygromov.github.io/aijam2026/** · Repo: **https://github.com/anatoliygromov/aijam2026**
- Per-team file links follow this pattern:
  `https://github.com/anatoliygromov/aijam2026/blob/main/index.html` (swap the filename per team).

---

## On the day
- Each team works from its brief: `teams/team-N.md` (page, theme, required tech, paste-ready prompt).
- Flow: **Clone in GitHub Desktop → connect the folder in Claude → prompt → Commit to main → Push origin.** ~30–60s later it's live.
- Reveal: open the live URL on the big screen, click Home → About → Team → Contact.

## Tip
- Tell everyone: **only edit your own file, never the locked seam.** Different files =
  zero merge conflicts, so all four teams can commit to `main` freely.
- Need a local asset (3D model, texture, audio)? Drop it in your **`assets/teamN/`** folder
  via **Add file → Upload files** (no terminal) and reference it relatively. Most teams can
  skip this and just load assets from a URL/CDN or generate them in code.
- Want a dramatic simultaneous reveal instead? Have each team commit to a branch named
  after them, and you merge all four at the end. (Adds one merge step — optional.)
- Optional upgrade: import the repo into **Vercel** for auto-deploys + per-commit preview
  URLs. GitHub Pages is the zero-cost default.

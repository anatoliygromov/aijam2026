# 🎬 Umain AI Jam — The Exquisite Corpse
### Slide-by-slide (compact). Each `---` = one slide. _Italic = say out loud._

---

## 1 — Title

**THE EXQUISITE CORPSE**
**An Umain AI Jam · 4 teams · 4 pages · 1 live website · ~1 hour**

_"We're building one website together — and we're not allowed to agree on what it looks like."_

---

## 2 — What & why

**The game:** Surrealists folded paper, each drew one body part blind, then unfolded one beautiful monster.
**Today:** 4 teams each build **one page** of the Umain site — each with a **set theme**, free to draw inspiration from any **films, books, music or plays** in that world — without seeing the others. One shared nav stitches them together.
**Why:** ship something real with AI in an hour · constraints make it funnier · the whiplash is the whole point.

---

## 3 — How you'll work: you prompt, Claude builds

**Nobody hand-writes HTML today.** You describe what you want; Claude writes and edits the code in your page. You direct, review, and re-prompt until it's right.

**🚫 No Figma.** Your only tools are **Claude** (builds the page) and an **image generator of your choice** (for visuals). That's it.

**3 rules to keep in your prompts:**
**①** Have Claude change **only your page file** — name it, and tell it to leave every other file alone.
**②** **Hands off the nav** (`nav.css` / `nav.js`) — never ask Claude to restyle the shared header/nav. That's the seam holding the corpse together.
**③** **One self-contained page, no build step** — inline CSS, images from URLs/CDN or generated.

_"You're a director, not a typist. Keep Claude inside your one page, never let it touch the nav, keep it a single file. Your team card's prompt already bakes these in."_

---

## 4 — Setup: Cowork + GitHub Desktop (one-time)

**Two tools: Claude (Cowork) to build, GitHub Desktop to publish.**
**①** Accept the GitHub invite in your email → you're a collaborator.
**②** Install **GitHub Desktop**, sign in, **Clone** `anatoliygromov/aijam2026` → it lands in a local folder.
**③** In Claude, **connect that folder** (Cowork). Claude can now read & edit your page.

**Repo:** `github.com/anatoliygromov/aijam2026` · **Live:** `anatoliygromov.github.io/aijam2026/`

_"Two tools. Claude builds your page; GitHub Desktop puts it live. Accept the invite, clone with GitHub Desktop, point Claude at that folder. Full steps in ONBOARDING.md."_

> Images: there's no built-in generator — bring an image tool (we'll all use the same one) and drop results in as **URLs**.

---

## 5 — The build loop

**① Prompt** — paste your team-card prompt, name your theme + required tech. Claude writes your page. You never hand-write HTML.
**② Iterate** — re-prompt, pull in images as URLs, load assets from a **CDN** or generate them in code (no local files).
**③ Commit** — in GitHub Desktop: type a summary → **Commit to main.**
**④ Push** — click **Push origin.** Refresh the live URL in ~30–60s. You're online. 🎉

_"Prompt, review, re-prompt in Claude — then Commit and Push in GitHub Desktop. Refresh and you're live. Commit early and often."_

---

## 6 — Teams

**4 teams. Your brief is secret — open your team's file in the repo to see your page, theme & required tech. No peeking at the others.**

| Team | Who |
|---|---|
| **1** | Essie · Nastya · Susanne |
| **2** | Jon · Ella |
| **3** | Anton · Lona |
| **4** | Sandy · Markus |

_"Here's who's on each team — and that's all you get on the big screen. Your actual mission is in your team's file in the repo: `teams/team-[your number].md`. Open only yours. What everyone's building stays secret until the reveal."_

---

## 7 — Timing (~60 min)

| Time | Doing |
|---|---|
| 0–5 | Intro + pick your theme direction |
| 5–10 | Accept invite · clone in GitHub Desktop · connect the folder in Claude |
| 10–45 | **Build** — prompt, generate, commit early & often |
| 45–50 | Polish + final commit (confirm it's actually live!) |
| 50–60 | **The reveal** |

_"Commit early — a live ugly page beats a perfect one stuck in a draft."_

---

## 8 — The reveal 🎬

**Big screen, walk the nav in order:** Home → About → Design Team → Contact ⚡
**Four worlds, one set of seams. Watch the whiplash.**

_"Click through together, live. Same nav every time, a completely different universe underneath. Unfold the corpse."_

---

## 9 — Wrap up

**You just shipped a live website with AI in under an hour — no hand-written code.**
Idea → live page, absurdly fast · constraints made it better, not worse · done-and-live beats perfect-and-draft.

**The site stays up: `anatoliygromov.github.io/aijam2026/` — share it, confuse people.**

# ✅ Pre-flight checklist — settle the tool decision (~10 min)

Run these on your own machine before Thursday. Each test ends in a **decision** so the
workshop tooling is locked by evidence, not guesswork.

**Repo:** `github.com/anatoliygromov/aijam2026` · **Live:** `anatoliygromov.github.io/aijam2026/`

---

## Test 1 — Can the GitHub connector WRITE? (~3 min)

This decides whether Cowork can publish on its own, or whether you need GitHub Desktop.

1. In Claude: **Settings → Connectors → GitHub → Connect** → authorize your account.
2. Start a chat and paste:
   > "Using the GitHub connector, in repo `anatoliygromov/aijam2026` add the line
   > `<!-- connector write test -->` to the end of `404.html` and commit it to `main`."
3. Watch what happens, then check the repo's commit history on GitHub.

**Decision:**
- ✅ **It commits** → connector can write. Make **Cowork + connector** the default path; GitHub Desktop becomes optional.
- 🔒 **It only reads / says it can't write** → connector is read-only. Make **Cowork + GitHub Desktop** the default.
- ⚠️ **It asks for more permission** → re-auth granting write scope, then retry once.

> Clean up after: delete that test line (or just leave it — it's a comment, harmless).

---

## Test 2 — Does the push step actually work end-to-end? (~3 min)

Only needed if Test 1 was **not** a clean ✅ (i.e. you'll use GitHub Desktop).

1. Install **GitHub Desktop**, sign in, **Clone** `aijam2026`.
2. Edit any page (even by hand) — add a comment line.
3. In GitHub Desktop: **Commit to main → Push origin.**
4. Refresh the live site after ~1 min — confirm the change is there.

**Decision:**
- ✅ Push works → GitHub Desktop is your reliable publish button. Lock the Cowork + Desktop flow.
- ❌ Auth/clone problems → fix sign-in before the day (this is the #1 thing that eats workshop time).

---

## Test 3 — Image generation: built-in or bring-your-own? (~2 min)

The brief assumes an "image gen tool of choice" — confirm what people will actually use.

1. In Claude, ask: *"Generate a 16:9 hero image of a Viking longship at dawn and save it as a file."*
2. See whether you get an actual image file, or whether Claude says it can't generate images here.

**Decision:**
- ✅ It generates → great, image gen is in-app; note it on the build slide.
- ❌ It can't → **standardize one external tool** (e.g. Firefly / Midjourney / DALL·E) and put it on a slide so 10 people aren't each hunting for one. Either way, images go in as **URLs**.

---

## Test 4 — Asset strategy: CDN/procedural vs local binaries (~2 min)

Decides whether the connector is viable or you must use real git for assets.

1. Skim the `assets/teamN/README.md` files — they already say assets can be **procedural or CDN-loaded (zero local files)**.
2. Decide the house rule you'll announce.

**Decision (recommended):**
- ✅ **Default = no local binaries.** Tell teams: load 3D models/textures from a CDN (three.js examples, jsDelivr), synthesize audio in code, use AI-image **URLs**. Keeps every publish path fast and dodges GitHub Pages size limits.
- 📦 **If a team insists on a local file** (custom `.glb`, recorded `.mp3`): they must use **GitHub Desktop or Claude Code** to commit it — the connector handles binaries poorly. Keep files well under ~100MB.

---

## 🏁 Final call (fill in after testing)

| Question | Result |
|---|---|
| Connector can write? | ☐ Yes ☐ No |
| GitHub Desktop push works? | ☐ Yes ☐ N/A |
| Image gen in-app? | ☐ Yes ☐ No → tool: ________ |
| Local binary assets allowed? | ☐ No (CDN/procedural) ☐ Yes (Desktop/Code only) |
| **→ Official path for the deck:** | ________________________ |

**Most likely outcome for a designer audience:** Cowork for building · GitHub Desktop for publishing · CDN/procedural assets · one agreed image-gen tool. Tell me the results and I'll lock the deck + ONBOARDING to match.

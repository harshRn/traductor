---
published: false
---

# traductor-www — maintainer notes

Static site that hosts the **Privacy Policy** and **Support** pages
required by the App Store listing for the Traductor iOS app.

Hosted via GitHub Pages. The two URLs that go into App Store Connect:

- Privacy policy URL: `https://harshrn.github.io/traductor-www/privacy/`
- Support URL: `https://harshrn.github.io/traductor-www/support/`

## Files

- `README.md` — landing page. Doubles as the GitHub repo front page
  *and* the GitHub Pages site root (Pages serves `README.md` at `/`
  when no `index.md` exists).
- `privacy.md` — privacy policy. Mirrors the "Data Not Collected"
  posture declared in the app's `PrivacyInfo.xcprivacy` manifest.
- `support.md` — support page with contact email and FAQ.
- `_config.yml` — minimal Jekyll config; uses the `jekyll-theme-minimal`
  theme so the markdown renders with basic styling.
- `INDEX.md` — this file. `published: false` front matter keeps it out
  of the public site; it lives in the repo as maintainer notes only.

## GitHub Pages setup (one-time)

1. Repo created on GitHub as `harshRn/traductor-www`. ✅
2. Pushed via `git push -u origin main`. ✅
3. **Settings → Pages** → Source = "Deploy from a branch",
   Branch = `main` / `/ (root)` → Save. Wait ~1–2 min for the first
   build.
4. Verify both URLs return 200 with no JavaScript required:
   - `https://harshrn.github.io/traductor-www/privacy/`
   - `https://harshrn.github.io/traductor-www/support/`
   Cheapest check: `curl -I <url>` — expect `HTTP/2 200` and
   `content-type: text/html`.
5. Confirm the support email in `privacy.md` + `support.md` is the
   address you want public on the App Store listing — currently
   `hardyharsh82@gmail.com`. Apple displays this on the public store
   page.
6. Record the live URLs in the parent iOS repo at
   `docs/plan/release.md` § Live submission URLs, and remove the
   "finalise at submission" tag from the two URL rows in
   `docs/plan/audits/28-app-store-checklist.md`.

## Updating

Edit the `.md` files, commit, push. GitHub Pages rebuilds automatically
in ~30 seconds.

If the `Last updated` date in either file changes materially, also
update the App Store release notes for that version.

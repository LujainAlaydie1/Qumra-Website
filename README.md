# Qumra (قُمـــرة) website

Four self-contained, bilingual (Arabic/English) static pages. Arabic is the
default language, with an EN/عربي toggle in the nav. This one is intentionally
dark-themed, matching the app's own moody, film-camera aesthetic (the app has
no light mode either).

- `index.html` — landing page
- `terms.html` — Terms of Use
- `privacy.html` — Privacy Policy
- `support.html` — Support / FAQ

## Deploy to Vercel via GitHub

1. `git init && git add . && git commit -m "Qumra website"`, push to a new GitHub repo.
2. In Vercel: **Add New Project** → import that repo. No build command needed.
3. Add a subdomain (e.g. `qumra.lsquared.sa`) under **Settings → Domains**.
4. `vercel.json` enables clean URLs.

## Important note

Qumra has no confirmed public App Store listing yet, so "Get the App" shows
a "Coming Soon" pill rather than a guessed link. Send me the real URL once
it's live.

## Content notes

The "In its own words" quote on the landing page is adapted directly from
the app's actual onboarding screen (`QumrahLanding.swift`) — the app already
explains its own concept better than marketing copy could, so I used it
almost verbatim in both languages. Qumra is fully on-device (SwiftData, no
Firebase, no account) — Terms and Privacy both call out the one deliberate,
by-design quirk worth knowing: undeveloped film that isn't opened in time is
permanently deleted, and that's intentional, not a bug.

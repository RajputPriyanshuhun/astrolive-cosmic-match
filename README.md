# Cosmic Match — AstroHack 2026 Prototype

A single-file, zero-backend prototype of a **double-sided referral loop** for AstroLive:
a compatibility report that only unlocks when the user invites a real person in, and
that person completes their own chart.

## Deploy to GitHub Pages (5 minutes)

1. Go to [github.com/new](https://github.com/new) and create a **public** repository
   (e.g. `astrolive-cosmic-match`).
2. On the repo page, click **Add file → Upload files**, and upload `index.html`
   (the one in this folder). Commit directly to the `main` branch.
3. Go to **Settings → Pages** (left sidebar).
4. Under "Build and deployment", set **Source: Deploy from a branch**, **Branch: main**,
   folder **/ (root)**. Click **Save**.
5. Wait ~1 minute, then refresh — GitHub shows your live URL, something like:
   `https://<your-username>.github.io/astrolive-cosmic-match/`
6. Open that URL, click through the flow once yourself to confirm it works live
   (the WhatsApp share and invite link both use the real deployed URL automatically —
   no code changes needed).
7. Make sure the repo is **Public** (Settings → General → Danger Zone → Change visibility,
   if it isn't already) — Unstop requires the link to be viewable by anyone.

That URL is what goes in the submission form as your prototype link.

## What's real vs. simulated in this prototype

| Feature | Status |
|---|---|
| Zodiac sign detection from DOB | Real logic (date-range lookup) |
| Compatibility scoring | Real algorithm (element-pair matrix + deterministic variance) — same two people always get the same score |
| Invite link generation | Real — encodes the inviter's data into the URL itself, so it works across two different phones/browsers with **no backend** |
| WhatsApp share | Real deep link (`wa.me`) |
| Score card image download | Real (via html2canvas, loaded from CDN — needs internet to work) |
| "Friends joined" / "minutes earned" on the dashboard | Sample numbers, clearly labeled — a real backend would track this across devices |

## Before you submit

- Double-check the final file naming rule for the **report PDF**:
  `AstroLive_TeamName_LeaderName.pdf`
- If you're a 2-member team, only the **Team Leader** should submit.
- Re-open your GitHub Pages link in a private/incognito window right before the
  deadline to confirm it's really public and loads correctly.

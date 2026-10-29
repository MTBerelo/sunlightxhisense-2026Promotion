# Sunlight × Hisense Promotion 2026: Campaign Dashboard

A single-page, read-only reporting dashboard for the Sunlight × Hisense washing machine promotion. It shows registrations, coupons issued and redeemed, top Hisense models, top selling stores, weekly trends and reminder results.

## What's in this repo

| File | Purpose |
|------|---------|
| `index.html` | The whole dashboard (HTML, CSS, JS and logos in one file) |
| `README.md` | This file |
| `.gitignore` | Ignores OS and editor files |

## Viewing it

- **Locally:** open `index.html` in any browser.
- **GitHub Pages:** push to GitHub, then go to **Settings → Pages**, set the source to the `main` branch and `/ (root)`. The dashboard will be live at `https://<your-account>.github.io/<repo-name>/`.

The only external dependency is Chart.js, loaded from cdnjs, so an internet connection is needed for the charts.

## Updating the figures

The dashboard has no edit mode. All figures live in the `DEFAULT` object near the top of the `<script>` block in `index.html` (registrations, retailers, models, coupons, weeks, stores, reminders, salespeople). To update:

1. Edit the values in `DEFAULT`, including the `updated` date.
2. Commit and push. GitHub Pages republishes automatically.

## Notes

- Data source: SAC cleaned export (ClientID-1525), as at 28 October 2026.
- The page includes a Print button, which prints all tabs.
- This dashboard is marked Confidential. Use a **private** repository, and note that GitHub Pages on a private repo requires a paid plan and is public to anyone with the link unless access control is enabled.

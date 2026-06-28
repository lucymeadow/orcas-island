# Orcas Island — Ian's 50th Birthday Trip 🐋

A living itinerary site for an Orcas Island trip, **Aug 5–10, 2026**.

**Live site:** https://lucymeadow.github.io/orcas-island/

## What's here

| File | Purpose |
|------|---------|
| `index.html` | All trip content (overview, conditions table, day-by-day, dining, shopping, logistics) |
| `styles.css` | Styling (colors, layout, responsive nav) |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is (no Jekyll build) |

## Adding details as they get scheduled

Everything lives in `index.html`. The most common edits:

- **Add a bullet to a day** — find the matching `<article class="day-card">` and add an `<li>...</li>`.
- **Add a labeled item** — start the bullet with a colored tag, e.g.
  `<li><span class="tag tag-water">Tour</span> Booked: 12:30 pm departure</li>`
  Available tags: `tag-run`, `tag-hike`, `tag-water`, `tag-food`, `tag-night`, `tag-spa`.
- **Update the conditions table** — edit the rows inside `<section id="reference">`.

After editing, commit and push:

```bash
git add .
git commit -m "Update itinerary details"
git push
```

GitHub Pages redeploys automatically within a minute or two.

## Sources

Sun/moon/tide timings reflect the trip dates; tides are MLLW from the NOAA Orcas
station (9449798), the nearest station to Deer Harbor. Bookings (whale watch,
bioluminescent kayak, spa) should be confirmed directly with each provider.

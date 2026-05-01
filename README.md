# Adamant Data Dashboard

A scenario comparison dashboard showing LNG Expansion vs Clean Economy Investment across key economic metrics.

## Files

- `index.html` — the full dashboard (HTML, CSS, JS in one file)
- `public/scenarios.json` — all data. Edit this file to update metrics, values, or add scenarios. No code changes needed.
- `vercel.json` — Vercel deployment config

## Updating data

Open `public/scenarios.json` in any text editor or directly in GitHub. Edit the `values` fields for each metric. Push to GitHub and Vercel redeploys automatically within 60 seconds.

## Adding a new metric row

Add a new object to the `metrics` array in `scenarios.json`:

```json
{
  "id": "your-metric-id",
  "label": "Your Metric Label",
  "source": "Source name and year",
  "sourceUrl": "https://source-url.com",
  "values": {
    "lng-expansion": "Value for LNG column",
    "clean-economy": "Value for clean economy column"
  }
}
```

## Adding a new scenario column

Add a new object to the `scenarios` array and add a matching key to every metric's `values` object.

## Deployment

Hosted on Vercel. Any push to the main GitHub branch triggers an automatic redeploy.

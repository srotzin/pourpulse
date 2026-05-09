# PourPulse

Real-time construction intelligence powered by embed sales data.

## Overview

PourPulse tracks foundation embed product sales across the United States to predict building activity 90 days before structures break ground. Embed products (anchor bolts, holdowns, mudsill anchors) are cast into concrete during the foundation phase — making them the earliest physical signal that a permitted project is actually proceeding to construction.

## Key Insight

The 90-day Concrete Wave Pipeline:

```
Permit Issued (Day 0)
    -> Embed Products Ordered (Day 30-45)
        -> Concrete Pour (Day 45-60)
            -> Framing Hardware Ordered (Day 90-120)
                -> Structure Out of Ground (Day 120-150)
```

Embed sales are the leading indicator. Everything else is lagging.

## Data Sources

- **Census Bureau Building Permits Survey** — Monthly state-level permits
- **Census Bureau New Residential Construction** — Monthly housing starts
- **BLS Local Area Unemployment Statistics** — Monthly state unemployment
- **DOL Unemployment Insurance Weekly Claims** — Weekly initial claims
- **Freddie Mac Primary Mortgage Market Survey** — Weekly 30-year rates
- **Industry Embed Sales Aggregation** — Daily anonymized sales data

## Tech Stack

- React 19 + TypeScript
- Vite 7
- Tailwind CSS 3.4
- Recharts
- Framer Motion
- Lucide React

## Development

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

## Deploy

Static site — deploy the `dist/` folder to any static host (Render, Vercel, Netlify, etc.)

# When AI Learns to Agree
### *Rationalized Harm and Multi-Turn AI Sycophancy in Gambling Advice*

An interactive data story for the QSS 45 final paper.

---

## What's in the site

- **Hero** with animated statistics
- **Experiment overview** — scenario grid, scoring rubric
- **6 interactive Chart.js visualizations**
  - Sycophancy by risk condition (bar)
  - Sycophancy across turns (line)
  - Turn × condition compound effect (dual line)
  - Response type distribution (stacked bar)
  - GPT-4o-mini vs GPT-5.2 comparison (grouped bar)
  - CatBoost feature importance (horizontal bar)
- **Conversation replayer** — step through 5 key turns of the coping scenario to see the drift happen
- Scroll-triggered reveal animations, reading progress bar

---

## Deploy to Vercel

### Option A — Vercel CLI (fastest)

```bash
# Install Vercel CLI if you haven't
npm install -g vercel

# From inside this folder
cd sycophancy-site
vercel
```

Follow the prompts (link to your account, name the project). It will deploy and give you a live URL immediately.

### Option B — GitHub + Vercel Dashboard

1. Push this folder to a GitHub repo
2. Go to [vercel.com/new](https://vercel.com/new) and import the repo
3. Leave all build settings as default — Vercel will detect it's a static site
4. Click **Deploy**

That's it. No build step, no dependencies, no node_modules.

---

## Local preview

Just open `index.html` in a browser — no server needed.

---

## Files

```
sycophancy-site/
├── index.html    # entire site — HTML, CSS, JS, charts, all inline
├── vercel.json   # tells Vercel to serve the folder as static
└── README.md     # this file
```

---

## Data sources

All chart data comes directly from the DATASHEET.md accompanying the paper. The condition-level turn breakdown (Figure 3 chart) is estimated from the paper's Figure 3, with values constrained to match the reported aggregate turn totals exactly.

---

*Bhagat, Shyam. QSS 45, Dartmouth College, 2026.*

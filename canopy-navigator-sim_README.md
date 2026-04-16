# canopy-navigator-sim

Interactive patient encounter simulation for the Canopy Navigator SDOH screening platform — Eisenhower Health Emergency Department pilot.

## Live demo

After deploying to GitHub Pages, the simulation will be available at:

```
https://<your-username>.github.io/canopy-navigator-sim/
```

## What this is

A 16-step interactive walkthrough of a complete Emergency Department SDOH encounter:
- Patient-facing tablet screens (exactly what Rosa Mendez sees at each step)
- Branching logic decisions (why certain follow-up questions appear)
- Live system event log (Z-code triggers, alert routing, billing activations)
- AI teach-back exchange with grading
- Full billing cascade (96160, 99285, G0019, TCM)
- Epic FHIR write-back payload

**Patient:** Rosa Mendez, 71, Medicare FFS — CHF exacerbation presenting to ED with food insecurity and transportation barriers.

## Deployment (GitHub Pages — 2 steps)

1. **Create the repository** named `canopy-navigator-sim` on GitHub (public, no README — you'll push this one).

2. **Push the files:**
```bash
git init
git add .
git commit -m "Initial simulation"
git branch -M main
git remote add origin https://github.com/<your-username>/canopy-navigator-sim.git
git push -u origin main
```

3. **Enable GitHub Pages:** Go to Settings → Pages → Source: Deploy from branch → Branch: `main` → Folder: `/ (root)` → Save.

Your URL will be live within ~60 seconds: `https://<your-username>.github.io/canopy-navigator-sim/`

## Navigation

- Click **Next / Prev** buttons to step through the encounter
- Use **keyboard arrow keys** (← →) for fast navigation
- Click any **dot** in the progress row to jump to that step
- Click **stage labels** at the top to jump to a section

## Files

```
canopy-navigator-sim/
├── index.html    ← Complete standalone simulation (all CSS + JS inline)
└── README.md     ← This file
```

The simulation is fully self-contained in `index.html` with no external dependencies — it works offline and loads instantly.

## Citation / usage

This simulation is part of the Canopy Navigator clinical and financial specification for the Eisenhower Health SDOH intake pilot. For questions, contact the Canopy 360 team.

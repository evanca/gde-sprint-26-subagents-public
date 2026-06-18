# Build a Weekend Glow-Up Planner with Parallel Subagents

**In this codelab you use Antigravity 2.0 to orchestrate parallel subagents:** one
orchestrator agent spawns short-lived subagents that first analyze a Stitch
prototype, then generate disjoint files concurrently — so you ship a working web
app faster, without agents colliding on files or saturating each other's context.

A hands-on lesson in orchestrator-driven parallelism: one Antigravity 2.0 agent
spawns short-lived subagents in two parallel phases — report-only analysts that
inspect the prototype, data contract, and UX contract, then disjoint-file
builders that generate the data, styles, and behavior concurrently against an
interface the orchestrator defines. You practice context isolation,
interface-first integration, conflict-free parallel generation, and verifying a
measurable UX contract — the orchestration discipline that keeps parallel agents
from saturating context or colliding on files.

**▶️ Start the codelab:** https://happycode.studio/gde-sprint-26-subagents-public/

## What you'll build

A small static Weekend Glow-Up Planner — three swappable themes that update every
content section, a checklist whose state persists across refreshes, and
keyboard-accessible controls — built from your own Stitch prototype by an
orchestrator and its parallel subagents.

![The finished Weekend Glow-Up Planner web app — themed sections and a persistent checklist, built by parallel Antigravity 2.0 subagents](./weekend-glow-up-planner/img/36765c55c60b6513.png)

## Get the starter files

Pull down just the `workspace/` folder with a sparse checkout — that folder is
your working directory, no copy step needed:

```bash
git clone --no-checkout --depth 1 https://github.com/evanca/gde-sprint-26-subagents-public.git
cd gde-sprint-26-subagents-public
git sparse-checkout init --cone
git sparse-checkout set workspace
git checkout
```

- `workspace/contracts/` — the data schema and the UX acceptance contract you
  build against.
- `workspace/design/` — where your own Stitch export goes.
- `workspace/app/` — the agents fill this; it starts empty.

Open `workspace/` in Antigravity 2.0 and follow the codelab from there.

---

Google Cloud credits were provided for this project as part of the Agentic Architect Sprint 2026.

#AgenticArchitect #GoogleAntigravity

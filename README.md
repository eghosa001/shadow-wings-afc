# Shadow Wings — AFC Virtual League

**Project:** Shadow Wings — AFC Virtual League  
**Coach:** Aighewi Eghosa  
**Team:** Shadow Wings  
**League:** C  
**Country:** Nigeria  
**Current baseline:** V2  
**Current tactical identity:** balanced vertical-transition football

## Core principles

- compact without the ball
- look forward first after regaining possession when safe
- nearest appropriate player presses; never everyone
- quick progression when available
- no blind attacking
- no passive possession for its own sake

## Read this first

For any AI sync, read **[SYNC_MANIFEST.md](SYNC_MANIFEST.md)** first.

Then read **[CONTROL_FILE.md](CONTROL_FILE.md)** before doing Shadow Wings work.

**DO NOT MODIFY THE FROZEN V2 BASELINE DIRECTLY.**

All future tactical experiments must create a new version (V2.1, V2.2, ...). See [prompts/V2_BASELINE.md](prompts/V2_BASELINE.md).

## Repository map

| Path | Contents |
|---|---|
| `SYNC_MANIFEST.md` | Lowest-cost AI synchronization entry point |
| `CONTROL_FILE.md` | Single source of truth |
| `prompts/` | Frozen V2 baseline + prompt changelog |
| `tactics/` | Match-day plan + Shout Playbook V1.1 |
| `competition/` | Rules & structure, confirmed facts, TBC & conflicts, source register |
| `practice/` | Data-capture protocol v1.1, practice allocation, match reports |
| `league/` | League match reports |
| `scouting/` | Opponent scouting template |
| `analytics/` | Match scorecard |
| `experiments/` | Experiment template, keep/revert framework, changelog |
| `handoff/` | Current state + AI sync protocol |

Canonical tactic files use underscores: `tactics/MATCH_DAY_PLAN.md` and `tactics/SHOUT_PLAYBOOK_V1.1.md`.

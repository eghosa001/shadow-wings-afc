# Shadow Wings Sync Manifest

**Purpose:** cheapest possible cross-agent synchronization point.

## Current project state

- Repository: `eghosa001/shadow-wings-afc`
- Branch: `main`
- Prompt baseline: **V2 — FROZEN**
- Shout Playbook: **V1.1 — FROZEN**
- Capture Protocol: **v1.1 — READY**
- Practice matches played: **0**
- League matches played at handoff: **0**
- Formation: **TBC — portal read required**
- Player models: **TBC — portal read required**
- Deployment health: **TBC — portal read required**

## Current next action

Read the live AFC portal configuration and practice panel before spending Practice Match 1.

Required portal capture:

1. exact formation shown
2. exact model for each of the five players
3. deployment status/health for each agent
4. practice matches available/remaining
5. replenishment/carryover information
6. practice opponents and repeatability
7. cooldown/retry/abandon/error-attempt behaviour
8. exact competitive window start/end displayed
9. shout limits/cooldown/persistence information if exposed
10. report/replay/log retention information if exposed

## Files a synced AI must read now

1. `CONTROL_FILE.md`
2. `handoff/CURRENT_STATE.md`
3. `prompts/V2_BASELINE.md`
4. `competition/TBC_AND_CONFLICTS.md`
5. `practice/DATA_CAPTURE_PROTOCOL_V1.1.md`

## Latest material change

2026-09-23:

- Added this sync system.
- Recorded a current-source scoring conflict: the live AFC leaderboard currently labels a clean match as **+5 points**, while transferred KB Rev 21 material recorded **+10 for a clean sheet**.
- Do **not** optimize around the disputed clean-match bonus until the current portal/rules resolve it.
- Official AFC tutorial still confirms live coach shouts are up to **200 characters** and go to **every agent on the pitch**.
- Published Strands technical material still describes a **1-second** hard decision contract, which conflicts with transferred Virtual League KB material describing about **5 seconds / repeat previous action**. Live Virtual League telemetry remains the authority for Shadow Wings.

## Sync command contract

When the coach says **SYNC SHADOW WINGS**:

1. Read this file first.
2. Read only the files listed above plus any files explicitly named under “Latest material change”.
3. Do not perform unrelated research.
4. Do not modify frozen baselines.
5. Do not assume portal values.
6. Report only: baseline version, changes since previous sync, next action, and unresolved blockers.

## Public repository safety

Never commit passwords, tokens, cookies, private portal links, billing information, registration-email addresses, or other secrets.

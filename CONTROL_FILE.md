# SHADOW WINGS CONTROL FILE — Single Source of Truth

## Project identity

- Team: Shadow Wings
- League: C
- Country: Nigeria
- Competition: AFC Virtual League (AWS Agentic Football Cup)
- Coach: Aighewi Eghosa

No registration email, passwords, API keys, tokens, cookies, or private identifiers are stored in this repository.

## Current state

- Prompt baseline: V2 — **FROZEN** (`prompts/V2_BASELINE.md`)
- Formation: **TBC / PORTAL READ REQUIRED**
- Models: **TBC / PORTAL READ REQUIRED**
- Shout Playbook: V1.1 — **FROZEN** (`tactics/SHOUT_PLAYBOOK_V1.1.md`)
- Capture Protocol: v1.1 — **READY** (`practice/DATA_CAPTURE_PROTOCOL_V1.1.md`)
- Practice Match 1: **NOT YET PLAYED**
- League matches: **0 played at the time of handoff**
- AI sync entry point: `SYNC_MANIFEST.md`
- Source of truth: this repository

## Tactical identity

Balanced vertical-transition football:

- compact without the ball
- look forward first after regaining possession when safe
- nearest appropriate player presses; never everyone
- quick progression when available
- no blind attacking
- no passive possession for its own sake

## Launch gate

Before Practice Match 1:

1. Verify five live V2 prompts against `prompts/V2_BASELINE.md` character-for-character.
2. Record exact live formation; never assume the portal default.
3. Record models for all five players.
4. Confirm deployment health.
5. Read the live practice panel: current remaining attempts, replenishment/carryover, opponents, cooldown and retry/abandon/error behaviour.
6. Record exact competitive-window start/end displayed.
7. Preserve portal configuration evidence.
8. Finalize practice allocation **BEFORE** spending the first attempt.

## Practice strategy

If the available practice budget permits:

- Practice Match 1: V2 unchanged, formation unchanged, Benchmark FC if available, no shout, full evidence captured.
- Practice Match 2: identical setup to Match 1.

No V2.1 change should be made merely because Match 1 is won or lost.

## Version-control rule

**Evidence → Hypothesis → One modification → Practice test → Measurement → KEEP or REVERT**

Never overwrite V2. Every change is a new versioned revision.

## Current scoring caution

A current AFC leaderboard page states **Clean match = +5 points**. Transferred KB Rev 21 material recorded **+10 clean sheet**. This is an active source conflict.

Until the live portal/current rules resolve it, do not optimize tactics around the clean-match bonus value.

## Next action

**Read the live AFC portal configuration and practice panel.**

Do not play anything until the practice allocation is agreed.

## Decisions log

- 2026-09-23: Prompt Set V2 approved and frozen.
- 2026-09-23: Shout Playbook V1.1 frozen (three corrections: S3, S5, S8).
- 2026-09-23: Data-capture protocol v1.1 established with portal-read launch gate.
- 2026-09-23: Persistent Shadow Wings state handed off into this repository.
- 2026-09-23: GitHub sync manifest/protocol added for low-Cognition cross-agent synchronization.
- 2026-09-23: Current leaderboard +5 clean-match value recorded as a conflict against transferred KB +10.

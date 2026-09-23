# Shadow Wings Portal Launch Checklist

Complete this **before Practice Match 1**. Copy portal values exactly; do not infer missing values.

## A. Team configuration

- Portal timestamp:
- Competition window shown:
- Formation exact name/value:
- Formation screenshot/reference:
- Redeploy status:

## B. Player-by-player deployment

| Player | Portal role/slot | Model | Deployment status | Live prompt exact-match V2? | Notes |
|---|---|---|---|---|---|
| 0 | Goalkeeper | | | YES / NO | |
| 1 | Defender | | | YES / NO | |
| 2 | Midfielder | | | YES / NO | |
| 3 | Forward 1 | | | YES / NO | |
| 4 | Forward 2 | | | YES / NO | |

If any live prompt differs from `prompts/V2_BASELINE.md`, stop. Record the diff before doing anything else.

## C. Practice panel

- Practice attempts available now:
- Weekly ceiling displayed:
- Replenishment/reset timing:
- Carryover stated:
- Opponents shown:
- Can the same opponent be repeated?
- Cooldown:
- Retry/reset rule:
- Does abandon consume an attempt?
- Does technical error consume an attempt?
- Any practice-only restrictions:

## D. Coach shout UI

- Character limit shown:
- Cooldown shown:
- Per-match limit shown:
- Persistence/duration shown:
- Replacement/stacking information shown:
- Other UI behaviour:

If the portal does not state an item, write **NOT EXPOSED** rather than guessing.

## E. Reports and evidence

- Match report available:
- Replay available:
- Event log available:
- Decision log available:
- Per-agent latency available:
- Command distribution available:
- Download/export available:
- Retention period shown:

## F. Scoring display

- Clean match / clean sheet value shown:
- Win points shown:
- Draw points shown:
- Loss points shown:
- Goal-margin bonus shown:
- Streak bonus shown:

Capture this because current public leaderboard (+5 clean match) conflicts with transferred KB Rev 21 (+10 clean sheet).

## G. Launch decision

Practice Match 1 may begin only when:

- all five V2 prompts are exact-match
- formation is recorded
- all five models are recorded
- deployment health is confirmed
- current practice budget/restrictions are recorded
- evidence-capture options are understood
- the practice allocation has been finalized from the actual remaining budget

**Baseline policy:** no shout, no tactical edit, no formation edit, no model edit during the run.

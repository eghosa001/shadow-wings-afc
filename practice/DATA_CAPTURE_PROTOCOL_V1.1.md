# Shadow Wings Data-Capture Protocol — v1.1

**Governing rule:** maximize information gained per practice match, not the number of matches played.

V2 stays **FROZEN** throughout baseline capture. No Practice Match 1 is spent until the live portal launch gate is completed.

## 1. Practice availability and launch gate

The registration record confirms **up to 10 practice matches per week**.

The live portal still must provide the operational values needed before allocation:

- attempts available/remaining now
- replenishment timing
- carryover, if any
- opponent choices
- whether opponents can be repeated
- cooldown
- retry/reset limitations
- whether abandoned or errored matches consume an attempt
- exact competitive-window start/end displayed
- report/replay/log retention

Do not confuse the registration ceiling with the current remaining balance.

## 2. Baseline record — complete before Match 1

| Field | Value |
|---|---|
| Pre-match timestamp | ___ (UTC + local time) |
| Formation | ___ exact portal value; never assume tutorial/default formation |
| Opponent | ___ exact portal name |
| Match configuration | ___ |
| Shout policy | NO shout |
| Player models | ___ all five |
| Deployment health | ___ all five |
| Practice attempts remaining before kickoff | ___ |
| Post-match storage | Full report/replay/logs if exposed |

Before kickoff, compare the five live prompts against `prompts/V2_BASELINE.md` character-for-character. Any drift means the run is not a valid V2 baseline.

## 3. Practice Match 1 — pure baseline

1. V2 exactly frozen.
2. Formation unchanged.
3. Use Benchmark FC if that opponent exists in the live panel; otherwise record the exact available opponent.
4. No prompt edits.
5. No formation changes.
6. No coach shout unless a genuine technical abnormality would otherwise make the run unusable.
7. If any shout is used, record exact time, score, text and reason.
8. Do not judge V2 from final score alone.

## 4. Capture everything exposed

### Match level

- final score
- goal timestamps
- possession
- shots
- conversion
- no-concession/clean-match status
- major events

### Per agent

- actions/commands
- command distribution
- decision success/failure
- latency
- timeout/idle/fallback behaviour
- stamina if exposed
- positional/heatmap data if exposed
- contradictions with the frozen role prompt

### Tactical

- progressive-pass attempts/success
- turnovers by zone
- central defensive breaches
- failed presses
- Forward 1 / Forward 2 spacing
- missed runs
- missed shooting opportunities
- defender positioning
- midfielder availability
- goalkeeper distribution/rushing/interception decisions

### Raw evidence

Preserve the full post-match report, replay and any decision/event logs when available. Do not retain only a summary when raw evidence can be saved.

## 5. Observation classification

Every observation gets one label:

- **Isolated event** — one-off; log, do not act.
- **Possible pattern** — repeated within one match, not cross-match confirmed.
- **Repeatable weakness** — repeated across decisions and matches; only class that can justify a prompt change.
- **Insufficient evidence** — state the gap; do not guess.

No V2 change after Match 1 unless there is an obvious technical failure such as repeated timeout/invalid actions or a prompt demonstrably not deployed.

## 6. Practice Match 2 — reproducibility

Where the confirmed available budget permits, repeat Match 1 with the same prompts, formation, opponent and shout policy.

Frozen comparison order:

1. latency / idle-timeout behaviour
2. goals and shots
3. turnovers by zone
4. central breaches
5. command distribution
6. forward spacing
7. progressive-pass success

Only cross-match patterns become V2.1 candidates.

## 7. V2.1 gate

After baseline evidence, choose the single strongest repeatable weakness and use `experiments/EXPERIMENT_TEMPLATE.md`.

One meaningful variable at a time. KEEP/REVERT is decided by `experiments/KEEP_REVERT_FRAMEWORK.md`.

## 8. Scarcity contingency

If the portal shows fewer usable attempts than expected or a limiting cooldown, redesign the remaining allocation before spending another match. Reproducibility may be traded consciously, never silently.

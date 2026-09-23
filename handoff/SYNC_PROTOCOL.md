# Shadow Wings AI Sync Protocol

GitHub is the persistent bridge between the coach, ChatGPT, the AFC Coach Mind, and any replacement AI.

## Source-of-truth order

1. `SYNC_MANIFEST.md` — what changed and what must be reread
2. `CONTROL_FILE.md` — governing project state
3. `handoff/CURRENT_STATE.md` — concise continuation state
4. frozen/versioned tactical files
5. evidence files: match reports, scorecards, scouting, experiments

If an AI's memory conflicts with the repository, the repository wins unless the coach explicitly says the repo is stale.

## After a change made outside the Mind

The AI making the change must:

1. update the relevant project file(s)
2. update `SYNC_MANIFEST.md`
3. preserve frozen baselines unless a new version is explicitly approved
4. commit the change
5. tell the coach which files changed

The coach can then tell the Mind:

> SYNC SHADOW WINGS

The Mind should refresh from the manifest rather than reconstruct the entire project from memory.

## After portal evidence arrives

Store exact observed portal values separately from assumptions.

Do not rewrite historical TBC/conflict records to pretend they never existed. Mark them **RESOLVED** with date, evidence and new operating value.

## Tactical change rule

No tactical revision exists until it is versioned and committed.

Evidence → Hypothesis → One modification → Practice test → Measurement → KEEP or REVERT.

V2 remains immutable. A change becomes V2.1, V2.2, and so on.

## Competition-platform safety

Do not build or use scripts, scraping, emulators, bots or other automation against the AFC platform. Keep project automation limited to documentation, analysis and version control outside the competition platform.

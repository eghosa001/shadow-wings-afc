# Shadow Wings Match-Day Plan

Transferred from Match-Day System v1 (2026-09-23), built on Prompt Set V2 (frozen baseline). Do not invent new tactics during or after this transfer.

NOTE ON SHOUT REFERENCES: the state guidance below predates Shout Playbook V1.1. Shout Playbook V1.1 (SHOUTPLAYBOOK_V1.1.md, FROZEN) supersedes the old six-shout list and is the live playbook. Old shout names below are retained verbatim for historical fidelity; at match time, select the V1.1 shout whose trigger matches the game state - match by trigger, not by name.

Ground rules confirmed by sources (KB Rev 21 Section 7B; Alpha Season mechanics verified 2026-09-23):

- 5-a-side, 2-minute matches, sudden death if level after 2 minutes. Every restart is a kickoff, no out of bounds.
- Scoring: Win +30, Draw +10, Loss +2 flat. Bonuses on wins only: +6 per goal of margin (max +30), +10 clean sheet, +8 per win from the 3rd consecutive win onward. Source: KB Rev 21 Section 8.
- Coach shouts are advisory: injected into each agent's context at the next decision cycle; agents weigh them with their own judgement and can ignore them. Prompts stay locked mid-match.
- Because losses score flat +2 with no bonus, a narrow draw converted to a win is the single most valuable in-match swing (30+bonus vs 10). Protecting a narrow lead is worth more than chasing a big margin.

### State 1 - Normal 0-0 state

- V2 already governs this: compact shape, look forward first when safe, nearest player presses.
- Coach action: watch only. No shout. Let V2 establish the baseline.
- Watch: early turnovers in our defensive third, keeper distribution choice, whether Forward 1/2 hold spacing.

### State 2 - Taking the lead

- No tactical change. V2 is balanced; leading changes nothing in the prompts.
- Coach action: no shout. Record goal timing and how the lead came about (shot vs pressure turnover).

### State 3 - Protecting a narrow lead

- Priority: defend the central route; our scoring maths reward holding the lead (win +30 + clean-sheet +10 if we shut them out).
- Shout if opponents push numbers forward: HOLD SHAPE (see Shout Playbook V1.1, S1 RESTORE SHAPE).
- Watch: defender stepping out of the central lane, keeper rushing unnecessarily, midfield abandoning central space.

### State 4 - Falling one goal behind

- Increase forward intent without breaking compactness: use a forward-tilting shout (GO FORWARD in the old list; nearest V1.1 equivalent by trigger is S3 RAISE THE PRESS) once, not repeatedly.
- V2's Forward rules already allow shooting with a clear lane; the shout tips the balance of judgement, it does not rewrite roles.
- Watch: whether Forward 2 still holds the wide outlet (it should - it is our counter route).

### State 5 - Chasing the game late (behind in final phase)

- Escalate once: ALL-OUT ATTACK in the old list; V1.1 equivalent is S8 ALL-OUT FINAL PUSH. Accept central-space risk deliberately - the shout makes the trade-off explicit to every agent.
- Use with ~30-45 seconds left, not before; a drawn 2-minute match goes to sudden death, so there is still a path at 1-1.
- Watch: whether all five players actually push up or whether agents ignore the advisory (tells us shout weight for future versions).

### State 6 - Opponent using a high press

- V2's counter: keeper clears under dangerous pressure (rule 3), forward-first transitions after winning possession.
- Coach action: no proactive shout. If turnovers pile up in our defensive third, RELEASE THE PRESSURE in the old list; nearest V1.1 equivalent by trigger is S4 PLAY THROUGH THE PRESS - read the trigger before use.
- Watch: intercept/turnover location data - if repeated, this is a candidate V2.1 change from evidence, not a live-shout fix.

### State 7 - Opponent sitting deep

- Threat is stale possession and crowd-out. V2's through-pass rule covers it; Forward 2's wide outlet stretches the block.
- Coach action: none by default. If we dominate the ball with no shots, SHOOT ON SIGHT in the old list; nearest V1.1 equivalent by trigger is S5 BREAK THE BLOCK - final phase only.

### State 8 - Opponent dominating central areas

- V2's compactness should prevent central breaches. If breaches repeat, the shout cannot fix the prompt - it can only blunt the damage.
- Coach action: HOLD SHAPE to reinforce compactness (V1.1 S1 RESTORE SHAPE); log every breach for the debrief. Repeated breaches = V2.1 evidence, not a shout problem.

### State 9 - Defensive emergency (shot threats from central positions)

- CLEAR THE LINES in the old list: safety over possession everywhere. No direct V1.1 equivalent exists; the keeper and defender prompts already govern Clear behaviour under pressure. Do not improvise new shouts.
- Risk is highest here: clearances concede territory. Use only when central breaches are producing shots.

### State 10 - Final phase (last 30-45 seconds)

- Level: sudden death looms - one decisive goal wins. Slight forward tilt acceptable via a forward-tilting shout if we are creating chances; otherwise hold.
- Ahead: protect shape, no risks, protect the win (+30 beats +10) - S2 PROTECT THE LEAD in V1.1.
- Behind: S8 ALL-OUT FINAL PUSH in V1.1. This is the only state where the risk is worth it.

### Shout discipline (applies to all states)

- Maximum 2 shouts per match (internal discipline, not a confirmed AFC rule). Every shout is recorded in the match log as a variable.
- Never stack two shouts at once - attribution dies with stacking.

Measurement rule: every shout used gets logged in the scorecard (shout, minute, state, effect observed). Isolated mistakes are noted, not acted on. Only repeatable patterns move V2.

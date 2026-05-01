# NH Baseball Intel — Build Journal

**Saved:** April 30, 2026
**State:** 14 of 20 teams ingested · 199 players · Spring 2026 season

---

## What this is

A personal analytics dashboard for NH high school varsity baseball. Source
data: GameChanger iPhone screenshots. Workflow: upload screens → OCR/transcribe
→ math-validate → ingest into the dashboard → render Liscio-style.

The dashboard is a single self-contained HTML file (`nh_baseball_dashboard.html`)
that runs in any browser. No server, no build step, no dependencies — just
open the file.

---

## Files

- **`nh_baseball_dashboard.html`** — the full standalone dashboard. Two views:
  per-team batting (with min-AB slider) and head-to-head team comparison
  (sortable on every category, with rank pills).
- **`README.md`** — this journal.

---

## Teams ingested (14 of 20)

| # | Team | Record | Players | Notable |
|---|------|--------|---------|---------|
| 1 | Trinity Pioneers | 8 GP | 15 | C Centorino #35 (1.525 OPS — league #1), A Harris #12 (1.232) |
| 2 | Goffstown Grizzlies | 4-4 | 10 | Z Tarrier #3 (.984 OPS, 11 BB) |
| 3 | Alvirne Broncos | 1-6 | 13 | J Krueger #4 (.943 OPS, 1 HR) |
| 4 | Pinkerton Astros | 7-1 | 14 | K Plasse #3 (1.075), L Beaulieu #4 (1.062), H Braiser #5 (1.004) |
| 5 | Nashua North Titans | 6 GP | 14 | N Sullivan #5 (.862 OPS) — best of a cold lineup |
| 6 | Nashua South Panthers | 3-4 | 14 | A O'Connor #24 (.904 OPS, 1 HR) |
| 7 | Bedford Bulldogs | 7 GP | 14 | Most balanced bottom-half team, 0 HR |
| 8 | Windham Jaguars | 3-3 | 13 | B Urquhart #25 (1.194 OPS, 9 hits all singles, .632 OBP) |
| 9 | Keene Blackbirds | 8 GP | 13 | B French #14 (1.005 OPS), K McDaniels #9 (.844) |
| 10 | Concord Crimson Tide | 9 GP | 14 | Plodzik (.977), Simms (.952), Turant (.929) — three near-elite |
| 11 | Bishop Guertin Cardinals | 8 GP | 14 | Plate-discipline team, 0 HR, no qualified hitter above .800 OPS |
| 12 | Timberlane Owls | 8 GP | 14 | M Santo...sso #4 (1.033 OPS) |
| 13 | Exeter Blue Hawks | 7-1 | 13 | R Plante #1 (1.146), E Battles #12 (1.078) — both league top 6 |
| 14 | Winnacunnet Warriors | 8 GP | 14 | H Reynoso #8 (1.211 OPS, .520 AVG, league #3) |

**Players with partial data** (yellow row, ⚠ marker):
- B Krol #14 (Pinkerton)
- M Conti #8 (Nashua South)

**Truncated names** (GameChanger cut them off mid-string):
- D Marti...hick #10 (Windham)
- M Santo...sso #4 (Timberlane)
- B Pinso...ault #10 (Winnacunnet — likely Pinsonneault)

---

## League OPS leaderboard (Min AB 10, qualified)

| Rank | Player | Team | OPS |
|------|--------|------|-----|
| 1 | C Centorino #35 | Trinity | 1.525 |
| 2 | A Harris #12 | Trinity | 1.232 |
| 3 | H Reynoso #8 | Winnacunnet | 1.211 |
| 4 | B Urquhart #25 | Windham | 1.194 |
| 5 | R Plante #1 | Exeter | 1.146 |
| 6 | E Battles #12 | Exeter | 1.078 |
| 7 | K Plasse #3 | Pinkerton | 1.075 |
| 8 | N Lavigne #11 | Trinity | 1.073 |
| 9 | L Beaulieu #4 | Pinkerton | 1.062 |
| 10 | T Lucier #9 | Trinity | 1.059 |
| 11 | M Santo...sso #4 | Timberlane | 1.033 |
| 12 | B French #14 | Keene | 1.005 |
| 13 | H Braiser #5 | Pinkerton | 1.004 |
| 14 | J Plodzik #22 | Concord | .977 |
| 15 | W Simms #11 | Concord | .952 |
| 16 | B Larck #2 | Winnacunnet | .945 |
| 17 | J Krueger #4 | Alvirne | .943 |
| 18 | J Coviello #7 | Windham | .937 |
| 19 | A Turant #8 | Concord | .929 |
| 20 | A O'Connor #24 | Nashua South | .904 |

---

## Team comparison — top of each category

- **OPS:** Trinity .969 → Windham .771 → Pinkerton .755
- **AVG:** Trinity .316 → Winnacunnet .296 → Windham .293
- **OBP:** Trinity .451 → Pinkerton .413 → Bishop G .378
- **SLG:** Trinity .518 → Windham .395 → Winnacunnet .377
- **Runs/G:** Trinity 8.0 → Pinkerton 6.4 → Windham 5.0
- **Walk rate:** Trinity / Pinkerton tied at 17.5%
- **Lowest K%:** Concord 15.1% → Trinity 15.6% → Bedford 18.9%

### Read of the league

**Trinity is in a tier of one.** .969 OPS leads by ~200 points. They walk
(17.5%), don't strike out (15.6%), and hit for power (4 HR, 27 XBH —
both league-best). Eight runs per game.

**Best record ≠ best offense.** Pinkerton (7-1) and Exeter (7-1) sit at #3
and #6 OPS. Both grind walks and play small ball — they win with pitching
and defense, not bats. Pinkerton has 50 BB (most in league) and zero HR.

**Nashua South (.529 OPS, 1.71 R/G) and Nashua North (.492 OPS, 33.5% K%)
are the league's two coldest offenses.** Nashua N strikes out in a third
of all PA — the only team above 30%.

**Small-ball league.** Trinity has 4 HR. Goffstown, Alvirne, Concord,
Nashua South each have 1. Pinkerton, Exeter, Bishop G, Keene, Winnacunnet,
and Timberlane all have **zero**. Total league HR through 14 teams: ~10.

---

## Schema (locked)

Per-player record:

```js
{
  name:    "C Centorino #35",
  team:    "Trinity",
  GP:      8,
  PA:      29,
  AB:      21,
  AVG:     .524,
  OBP:     .621,
  SLG:     .905,
  OPS:     1.525,
  H:       11,
  "2B":    3,
  "3B":    1,
  HR:      1,
  RBI:     11,
  R:       7,
  BB:      5,
  SO:      3,
  HBP:     2,
  _partial: false  // optional flag, defaults missing
}
```

Notes:
- `1B` is not stored — derivable as `H − 2B − 3B − HR`.
- `K-L` (looking strikeouts) is a subset of `SO`, dropped from unified table.
- `SAC` and `SF` not stored. Some OBP rounding differences (a few
  thousandths) come from GameChanger's handling of these — accepted as noise.

---

## Math validation pattern

Applied to every player on ingest:

1. `AB × AVG ≈ H` (within 0.5 of an integer)
2. `OBP + SLG = OPS` (within rounding)
3. `TB = (H − 2B − 3B − HR) + 2·2B + 3·3B + 4·HR`, then `SLG = TB / AB`
4. `OBP = (H + BB + HBP) / PA` — sometimes off by a thousandth or two
   when GameChanger excludes SAC; accepted

Any row failing this gets flagged. Across 199 ingested players, all but two
(Krol, Conti — flagged `_partial`) hold up clean.

---

## Design system

- **Layout:** Liscio-style. Navy `#1e3a5f` left sidebar, blue `#2563eb` active
  accent, white surfaces, light gray `#F5F6F8` background, `0.5px` borders
  on `#E5E7EB`.
- **Typography:** Inter (web font). 11–12px body, 18px page titles, 500 weight
  for emphasis (no bold-bold).
- **Border radius:** 8px on cards/buttons, 12px on the shell.
- **Rate stat formatting:** 3 decimals, leading zero stripped (`.524` not `0.524`).
- **Min AB:** 10 by default. Slider 0–35.

### Team-tag colors

| Team | Color hex |
|------|-----------|
| Trinity (pioneers) | `#1e40af` |
| Goffstown (grizzlies) | `#92400E` |
| Alvirne (broncos) | `#065F46` |
| Pinkerton (astros) | `#6D28D9` |
| Nashua N (titans) | `#BE185D` |
| Nashua S (panthers) | `#7C3AED` |
| Bedford (bulldogs) | `#B45309` |
| Windham (jaguars) | `#0E7490` |
| Keene (blackbirds) | `#4B5563` |
| Concord (crimson) | `#B91C1C` |
| Bishop G (cardinals) | `#DC2626` |
| Timberlane (owls) | `#4338CA` |
| Exeter (bluehawks) | `#0369A1` |
| Winnacunnet (warriors) | `#15803D` |

Six unused colors saved for the remaining teams: gray, indigo, lime, rose,
cyan, slate.

---

## What's left

### 6 more teams to ingest (#15-20)

Workflow per team:

1. Identify team name from the GameChanger header.
2. Capture all 5 column views:
   - GP / PA / AB / AVG
   - OBP / OPS / SLG / H
   - 1B / 2B / 3B / HR
   - RBI / R / BB / SO
   - K-L / HBP / SAC / SF
3. OCR each column into per-player records.
4. Math-validate (see pattern above).
5. Append the team's array to the dashboard JS.
6. Add to `allPlayers` concat, `teamMeta` object, `teamClass` map.
7. Add team-pick to sidebar with new color.
8. Add CSS for the team-tag class color.

### Londonderry Lancers — partially captured, needs 3 more screens

Already have:
- ✅ GP / PA / AB / AVG
- ✅ AVG / OBP / OPS / SLG

Still need:
- ❌ H / 1B / 2B / 3B
- ❌ HR / RBI / R / BB
- ❌ SO / K-L / HBP / SAC

Visible roster: S Daron #5, J Ruggiero #21 (.988 OPS — top tier), C Jordan #9,
J Stott #3 (.884), C Washington #2 (.907), C Loughlin #0, B Fuller #10,
S Iorio #11, B Labbe #1, B Fitzgerald #8, C Hartley #39, C Kearney #22,
C Marsh #7. Three players above .800 OPS visible — strong upper lineup.

### Optional follow-on builds

- League top 10s view in every category (single page of leaderboards)
- Pitching tab (T mentioned having those screenshots)
- Export CSV (button is wired via `sendPrompt`, not yet built standalone)
- Re-screenshot B Krol and M Conti to fill partial data
- Roster + schedule tabs

---

## Resuming work

Next time, paste in this journal as context, then upload screenshots for the
next team. The pattern is set — 14 teams of practice means each new team
takes one round trip per screen-batch, then a re-render with one new array
appended to the JS.

When tax season ends and full build bandwidth is back, this same Liscio-style
chrome can be lifted into the **CPA practice management app** in Base44 — same
sidebar pattern, same nav structure, same card aesthetic, same Inter +
navy/blue color story. The schema-versioning pattern (every record gets a
`tax_year` field, partial rows flagged) maps directly onto this project's
`_partial` pattern and team-color tagging.

# Pocket Sprint — Project and testing notes

**Latest supplied build:** v1.0.7 (`Pocket_Sprint_V1.0.7.ngc` in the private archive). This public GitHub showcase intentionally does not include the ROM, source tree, assembler, BIOS, toolchain, or submission JSON.

## Play and modes

- Normal and Reverse racing, plus Weapons racing with special item pickups.
- Twelve courses grouped into three four-race championship cups. Races support 3/5/10-lap settings.
- In championships, complete the race, see the result, review cumulative standings, then visit the upgrade garage (acceleration, speed, grip).
- Time Attack records best individual laps, with hazards selectable on/off.
- Local two-player is a same-console head-to-head mode with automatic acceleration; player 1 steers using D-pad, player 2 using A/B. The five-point advantage / five-lap cap rules are described in the supplied private `START_HERE.txt`.
- Link sessions offer host/join setup and race/cup events, including separate garage spending for two players. Both devices must use matching v1.0.7 due to protocol update to 0x16.
- Four unlockable mini-games: Cliff Brake, Bumper Drop, Maze Chase and Bomb Grid.

## Controls

- Solo racing: A accelerate, B brake, Left/Right steering, OPTION pause/resume.
- Title: Up/Down race mode, Left/Right cup, A begin, OPTION options.
- Same-console 2P entry: hold B, then A at championship menu. P1 D-pad, P2 A/B.
- Link: Options > Link Cable (or OPTION on local duel setup), choose one host and one guest; both copies need v1.0.7.
- Records: Options > Records; for qualifying time entries press OPTION to begin QR initials and display.

## Ranked online times — NOT site verified

The private v1.0.7 package inherits its v1.0.6 SPR4 QR format and proposes time-based rankings, not arbitrary score points.

- Full-race fastest time: 12 tracks × 3 race modes × 3 lap options = 108 requested divisions.
- Time Attack best lap: 12 tracks × traps on/off = 24 requested divisions.
- Overall proposal: 132 independent categories, sorted from **lowest time** to highest.
- Only the standard races and Time Attack are included in the QR proposal; mini-game results, cup standings and local two-player/link/attract performances are local only.
- No confirmation was supplied that the public website supports or has activated all 132 divisions, the QR format or the game listing.
- The current QR payload is not cryptographically signed, so the site owner will also need to consider validation.

## v1.0.7 performance notes (supplied emulator measurements only)

The private `PERFORMANCE.md` reports:

- Link race v1.0.6 achieved ~81.7%, 89.3% and 80.6% game speed (Normal, Reverse, Weapons respectively), with uneven 12–13 fps updates in the benchmark.
- v1.0.7 reports approximately 100% / 99.8% (Normal), 100% / 99.9% (Reverse) and 99.4% / 99.2% (Weapons) game speed on host/guest, with a near-locked 20 fps picture cadence.
- Solo race physics/scoring remain unchanged by this update, with smoother presentation in many tested cases.
- These are measured using NgpCraft Studio 4.3.2's emulator core and a timing-model link fixture. They should NOT be presented as physical hardware/cable guarantees.
- Physical NGPC hardware, real link cable and real website upload compatibility remain outstanding.

## Screenshot provenance

- Files `01-title-card.png` and `15-link-cup-setup.png` to `18-link-cup-winner.png` are nearest-neighbour enlargements of 160×152 images already included in the user's v1.0.7 archive.
- Files `02` to `14` and `19` to `41` were captured directly from the supplied C-source game's own host rendering engine, with native game simulation for race driving and completion, then nearest-neighbour enlarged from 160×152 to 640×608. A few menus, courses and unlockable games were selected or unlocked in the preview state to cover more features.
- `00-pocket-sprint-showcase.png` is a manually assembled collage using the above real frames. It is not a single captured game screen.
- None of the game images are AI-generated.

## Publication and rights

This is a **documentation-only** work-in-progress showcase. No ROM or source code is published. The private source includes third-party code and music attributions; check their licensing and game/music rights separately before any eventual public game release. No SNK endorsement is claimed.

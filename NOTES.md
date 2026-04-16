# Future development notes

Running list of deferred items. These aren't blocking the current build —
captured here so they don't get lost between sessions.

## Developer control panel (expanded)

Add an in-game control panel pane (probably hidden behind a dev-mode toggle
in the settings drawer) that exposes every tuneable feel/transition value
as a live slider:

- View fade duration (currently 140 ms)
- Wrong-placement shake duration + amplitude (currently .35 s, 8 px)
- Pole soften: band percentage, max blur, max dim, easing curve
- Outside-view transformed-tile dim level (currently 0.45)
- Inside/outside zoom defaults
- Pulse frequencies (green correct, orange carry, hint cluster, hint target)
- Long-press duration, long-press movement cancel threshold
- Hint cooldown, hint score penalty
- **Combo curve values** (currently [1, 1.5, 2, 3, 5])
- **Exposure timer max** (currently 20s)
- **Exposure recharge/drain amounts** (currently +8s correct, -4s wrong)
- **Difficulty glow tint intensity** (currently .82/.78 RGB)

**Persistence**: the panel should remember the player's selections across
sessions (localStorage), so the creator can dial in the feel over multiple
play sessions without re-tweaking every time. An "export/import JSON" or
"copy as code" button would let dialed-in values get pasted back into the
source as the new defaults.

## Done (moved from backlog)

- ~~Combo streak system~~ ✅ (April 16)
- ~~Reality exposure timer~~ ✅ (April 16)
- ~~Tile difficulty scoring + glow~~ ✅ (April 16)
- ~~Voronoi tessellation~~ ✅
- ~~Outside view atmosphere (backdrop, breathing, idle drift, particles)~~ ✅
- ~~Pole softening~~ ✅
- ~~View fade transitions~~ ✅
- ~~Settings panel (zoom, drift, backdrop, particles, edges, mode, view)~~ ✅

## Remaining deferred polish

- Tile pickup lift + glow animation
- Correct-placement snap + particle burst
- Richer SFX variety (not just one correct/wrong tone)
- Ambient soundtrack
- Star rating screen
- Multi-image test pass (different panoramas stress-test the pole soften +
  UV mapping)
- Screen-edge vignette
- Eased score / progress counter animation
- Daily game system (one new scene per day)
- Capacitor native wrap (iOS/Android)
- Monetisation integration
- Production panorama pipeline (Skybox AI → automated processing)

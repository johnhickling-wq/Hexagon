# Future development notes

Running list of deferred items to tackle after the current A+B+C+D polish
pass lands. These aren't blocking the current build — captured here so they
don't get lost between sessions.

## Developer control panel

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

**Persistence**: the panel should remember the player's selections across
sessions (localStorage), so the creator can dial in the feel over multiple
play sessions without re-tweaking every time. An "export/import JSON" or
"copy as code" button would let dialed-in values get pasted back into the
source as the new defaults.

## Other deferred polish (from backlog.pdf)

- Tile pickup lift + glow
- Correct-placement snap + particle burst
- Richer SFX variety (not just one correct/wrong tone)
- Ambient soundtrack
- Star rating screen
- Multi-image test pass (different panoramas stress-test the pole soften +
  UV mapping)
- Screen-edge vignette (E, deferred)
- Eased score / progress counter (F, deferred)

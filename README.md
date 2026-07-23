# XONOTIC: ARENA

A **bring-your-own-deck trading card game** that turns the open-source arena FPS [Xonotic](https://xonotic.org) into a tabletop game — keeping what actually makes an arena shooter feel like one: **speed, stack management, weapon combos, and map control**, all running on one shared combat engine across every game mode.

🎯 **Play it here → https://m00minpappa.github.io/xonotic-arena/**

## The trio

| Page | What it is |
|------|-----------|
| [**Card Gallery**](index.html) | The pitch + the full card art — engine, 16 weapons, 12 avatars, items, modes, starter decks |
| [**Complete Rules**](rules.html) | The manual — turn structure, combat math, all modes, deckbuilding, twelve signature decks |
| [**Print & Play**](pnp.html) | A printable kit — cut-out cards, location tiles, tokens, and fighter mats (US Letter, 100% scale) |

## About the avatars

The twelve Fighter avatars each carry a buff, a nerf, and a limited-use signature. Ten are modeled on a real playgroup: **idfarms** (the Farmer), **Dr. Shrimp Puerto Rico** (the Clutch), **slipperysalamander** (the Runner), **mouseeyeeater** (the Rookie), **Bingus** (the Machine), **booger** (the Faithful), **kelso** (the Ambusher), **meth_invader** (All-Ears), **trashpanda** (the Perch), and **jared** (the Boomer). Two are house non-players for the empty seats: **wildcard** (the Coin-Flip — boom or bust, enthusiastic either way) and **seajay** (the Wrench — a can-do saboteur who jams anyone's plan, his own included).

## Balance — playtested v0.2

The v0.2 numbers were tuned across a **40-game simulation pass** (a Python engine that plays the game and reports the stats). Highlights: Vortex de-fanged as a safe-sniping tool, idfarms and Bingus brought up to viable, Shrimp's duel dominance trimmed, and CTF retimed to a **10-round match (~20–30 min)**. See the balance note atop the [rules](rules.html).

## Contributing

This is a fan-made design draft, and the fastest way it improves is more hands and
more games. Ideas, playtest data, art, and fixes are all welcome — open an
[issue](../../issues) to propose or discuss, or a pull request for something
concrete. **Cards are just data:** every card lives in a plain JavaScript array
inside the HTML (`AVATARS`, `WEAPONS`, `ITEMS`, `MODES`, `DECKS` …), so adding one
is editing a list, not writing an engine.

### Where to jump in

| Track | What it covers | A good first contribution |
|-------|----------------|---------------------------|
| **Playtesting** | Real games at the table — what felt broken, what never got played, which avatar ran the room | A game log: mode, decks/avatars, final score, and the one thing you'd change |
| **Balance & the sim** | The Python engine that plays the game and reports stats | A new matchup scenario, a bug in the combat math, or a tuning proposal backed by numbers |
| **Special cards** | The trading side — rarity tiers, alt-art, foils, promos, and chase cards groups can swap | A rarity model (Common → Signature) or a promo card with real art |
| **Expansion packs** | Themed sets that bolt onto the core engine (see below) | A pack pitch: theme, 6–12 cards, and the one rule it changes |
| **New avatars** | The buff / nerf / signature framework — model your own playgroup | One avatar entry, balanced against the existing twelve |
| **New modes & maps** | More Xonotic modes as Mode Cards; named arena boards with their own item dials | A Mode Card (win condition + what differs) or a location layout |
| **3D-printed minis & tokens** | Fighter minis, location tiles, stack/momentum dials, ammo & flag tokens | An STL plus a photo of the print |
| **Reference materials** | Player aids — quick-ref cards, a combat-math cheat sheet, a first-game tutorial | A one-page turn/round reference sized for the table |
| **Digital & tooling** | A deckbuilder, a score/stack tracker, or a Tabletop Simulator / Tabletopia port | A rough deckbuilder that enforces the 40-card rules |
| **Art & flavor** | Card art, avatar portraits, box/label art, flavor text | A single reworked card face in the site's visual language |
| **Localization** | Translations of the rules and card text | One page translated, terms kept consistent |
| **Rules & errata** | Clarifications, edge-case rulings, an FAQ | A ruling on an interaction two players read differently |

### Two of the bigger ideas

**Special cards & the trading layer.** The game is bring-your-own-deck, so the
natural collectible hook is *cards worth trading between groups*: rarity tiers,
alternate-art and foil treatments, one-off promos, and signature cards a playgroup
mints for its own fighters. Proposals here should say how a card enters a deck
without breaking the 40-card / copy limits.

**The Host Pack (an expansion concept).** An expansion that turns *server host
settings into table rules*. Real Xonotic cvars become cards and modifiers —
low-gravity (`sv_gravity`), instagib / overkill arenas (`g_instagib`,
`g_overkill`), weapon-arena loadouts, start-ammo and item-respawn tweaks, damage
multipliers, warmup, bot-skill for solo play. This is also the home for **new card
*features*** — cards that override a nerf, grant a temporary buff, or apply a
global modifier for a round — since a host toggle is exactly the fiction for "the
rules just changed." A pack should name its theme, list its cards, and call out the
single core rule it bends.

### Ground rules

- Keep it **fan-made and GPL-friendly** — no copyrighted assets, no claim of
  affiliation with the Xonotic project.
- Balance-affecting changes should come with a reason (ideally a game log or a sim
  run), not just a hunch.
- Match the existing voice and the site's visual language; new cards follow the
  buff / nerf / signature (or weapon / item) shape already in use.

## Status

Design draft `v0.2`. A **fan-made** tabletop concept — not affiliated with the Xonotic project. Xonotic itself is free & open-source under the GPL; see [xonotic.org](https://xonotic.org).

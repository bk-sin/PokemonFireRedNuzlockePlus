# Pokémon FireRed Nuzlocke Plus v1.0

**FireRed with the Nuzlocke rules built into the game.** Every rule and quality-of-life feature can be switched on or off from an in-game menu. The story, maps and trainers are vanilla FireRed. The engine is **pokeemerald-expansion 1.17.1**, so you get Gen 9 battle mechanics, the Fairy type, a physical/special split, and modern learnsets and abilities.

> **AI disclosure:** This hack was made almost entirely with an AI coding assistant: it wrote the code, the data tools and the docs. I came up with the features, directed the work and tested the game.

## Features

### Nuzlocke rules (NUZLOCKE page, shown when you start a new game, editable later from OPTION → SELECT)
The rules switch on once you receive the Pokédex.

- **Permadeath:** a fainted Pokémon is dead. Items, the Pokémon Center, Mom and the PC can't heal or revive it.
- **First encounter only:** one catch per route/area. Later encounters show "You can't catch this POKéMON." and you keep the ball.
- **Dupes clause:** a duplicate of an evolution line you already caught doesn't use up the area. Shiny clause takes priority.
- **Shiny clause:** shinies can always be caught.
- **Statics count:** optional, off by default.
- **Forced nicknames:** a nickname is required when you catch or receive a Pokémon.
- **No battle items:** you can't use bag items in battle (Poké Balls still work).
- **Forced SET battle style.**
- **Level cap:** set by the next Gym Leader's ace (14/21/24/29/43/43/47/50, then Elite Four 54–63). Pokémon at the cap get 0 EXP and Rare Candies are blocked.
- **Pokémon Center heal limit:** unlimited, 2, 1 or 0 heals. Heals refill with each badge, or the number covers the whole game. The nurse shows "Heals left: N", and Mom and blackouts use the same counter.
- **Wiped party:** if your whole party is dead, there are no wild encounters or trainer battles until you take a living Pokémon out of the PC.

### Battle
- **Damage calculator:** shows the estimated damage as a % of the target's HP range in the move menu (e.g. "Normal 46–62%").
- **Battle info panel (R):** stat stages for both sides, weather/terrain with turns left, Trick Room, and type-effectiveness indicators.
- **Battle summary:** after each battle, damage dealt, damage taken and KOs for every Pokémon you used.
- **EXP multiplier:** x0.5 / x1 / x2 / x4. The level cap and permadeath still apply.
- **Physical/special split** (toggle), Gen 9 battle engine, Fairy type.

### Training
- **IV/EV viewer** in the summary screen (A cycles Stats → IVs → EVs).
- **Free move relearner** from the START menu, the summary screen, and an NPC in every Pokémon Center. It also offers egg, TM and tutor moves.
- **Pokémon Center helper:** shop with all 21 Mints, the EV-reducing berries and the Fresh-Start Mochi.
- **Party EXP Share** (toggle, off by default). Reusable TMs.
- **No-trade evolutions:** Kadabra, Machoke, Graveler and Haunter evolve at Lv 36. Item trade evolutions work by using the item from the bag.

### Exploration
- **HM-free field moves:** you need the HM in the bag, the badge, and a party Pokémon that can learn the move.
- **Fast travel:** FLY from the START menu or the Town Map, no Pokémon needed.
- **PC from the START menu.** Running indoors, optional auto-run, and a "use another Repel?" prompt.
- **DexNav:** see what lives on the current route and search for it.
- **Followers:** your first living Pokémon follows you.

### UI
- **HGSS-style Pokédex:** base stats, abilities, evolutions and learnsets, plus area. Seen-only species can open every page too.
- **Strategy Dex:** recommended competitive sets (moves, item, ability, nature, EVs) for 895 species, including 370 of #1–386. On a Pokédex entry press **START** to open them and **A** to see the next set.
- **Bigger bag** with sorting.
- **Everything configurable:** every feature can be toggled on the FEATURES page (OPTION → SELECT → SELECT).

## Download & patching
- **Download:** https://github.com/bk-sin/PokemonFireRedNuzlockePlus/releases/latest (`Pokemon FireRed Nuzlocke Plus.bps`, ~17 MB)
- **Base ROM:** Pokémon FireRed (USA) **v1.0** (not Rev 1)
  - SHA1 `41cb23d8dccc8ebd7c649cd8fbb58eeace6e2fdc`
  - CRC32 `DD88761C`
  - MD5 `e26ee0d44e809351c8ce2d73c7400cdd`
- **Patch tool:** apply the .bps with **Floating IPS (Flips)** or **[Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/)**.
- **Patched ROM:** 32 MB, SHA1 `cc019b4f2f1b5d0de228f1c676819c00992d1f2a`, CRC32 `85F161DC`.
- **Saves:** Flash 128K. Tested on mGBA (recommended). Vanilla FireRed saves aren't compatible, so start a new game.

I can't share ROMs, so please don't ask.

## Known issues
- The HGSS Pokédex list header says "HOENN" (an expansion graphic). The list itself is Kanto, and numbers are national.
- The Pokédex AREA page is a full-screen Kanto map without the page tab bar.
- Followers haven't been tested in every FRLG cutscene. If one looks odd, turn FOLLOWERS off.
- In the Safari Zone, the Safari Ball just plays an error sound on an already-used area.
- Some later-generation evolution items (Protector, Electirizer…) aren't obtainable on the FRLG map.
- The damage calc is an estimate: no crits, accuracy, Focus Sash/damage-reducing berries or Sturdy.
- Strategy Dex sets come from older metagames and were filtered to moves learnable in this game, so some sets are modified. Hidden Power is shown without its type. Some recommended items aren't obtainable, and 13 form-heavy species (Unown, Arceus, Vivillon…) show "No data".
- The patch is large (~17 MB) because the ROM is 32 MB.

## Credits
- **pret** — pokefirered decompilation
- **rh-hideout** — pokeemerald-expansion and all its contributors (see the expansion's CREDITS.md)
- **Pokéxperto** (pokexperto.net) — strategy set data, adapted from their Pokédex strategy pages. Licensed **CC BY-NC-SA 3.0**.
- **Smogon University** contributors — strategy sets, via data.pkmn.cc (pkmn project)
- **mGBA** — testing
- **Floating IPS / Rom Patcher JS** — patching
- **Pokémon** © Nintendo / Creatures / GAME FREAK. This is a free, non-commercial fan project.

**Hack by bk-sin — v1.0**

## Screenshots

![nuzlocke rules page](screenshots/01_nuzlocke_rules_page.png)
![features page](screenshots/02_features_page.png)
![damage calc](screenshots/03_damage_calc.png)
![battle info panel](screenshots/04_battle_info_panel.png)
![battle summary](screenshots/05_battle_summary.png)
![strategy dex](screenshots/06_strategy_dex.png)
![iv ev viewer](screenshots/07_iv_ev_viewer.png)
![follower](screenshots/08_follower.png)
![dexnav](screenshots/09_dexnav.png)
![pokecenter heal limit](screenshots/10_pokecenter_heal_limit.png)

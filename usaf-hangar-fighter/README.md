# Hangar Fighter

A browser-based 2D arcade fighting game prototype with scenario-based matchups, desktop keyboard play, and mobile touch controls.

Play it here:

https://vibezzzcoder.github.io/hangar-fighter/

## Status

This is a stable, published prototype. Versus Mode and Boss Rush Mode are implemented,
and the self-contained release build is live at the link above. Automated QA is green on
the current build, which has also been played and accepted on macOS Safari, on iOS, and
as an iOS home-screen web app. There is no known coding blocker.

## Screenshots

![Flight Suit vs Camo scenario](scenario-flight-suit-vs-camo.png)

![PT Showdown scenario](scenario-pt-showdown.png)

![Formal Face-Off scenario](scenario-formal-face-off.png)

## Features

- Main Mode Select with `Versus Mode` and `Boss Rush Mode`
- Versus Mode uses best-of-three rounds
- Boss Rush uses best-of-three rounds per boss, so a clean run is six rounds
- Three scenarios: Joint Maintenance, PT Showdown, and Formal Face-Off
- Scenario-specific fighter pairings and stage backgrounds
- Boss Rush single-player run: MTI vs Karateka, SecFo, and AI Robot
- Per-stage music, layered sound effects, and an announcer line at the start of a match
- Victory celebration after clearing the final boss, skippable with a tap or `Enter`
- Local two-player keyboard controls
- Optional CPU control for Player 2
- Player 2 CPU support remains available for Versus play (and is enabled by default on phones/tablets)
- Mobile touch controls for phone and tablet browsers
- Punch, kick, jump, crouch, hitstun, knockback, health bars, and win state
- Debug hitbox toggle for tuning and testing

## Game Modes

- `Versus Mode`: pick a scenario and play best-of-three rounds with local PvP or CPU Player 2.
- `Boss Rush Mode`: single-player challenge where MTI fights three bosses in sequence -- Karateka, SecFo, then AI Robot. Each boss is its own best-of-three match: win two rounds to move on, lose two and the run is over. A full clean run is six rounds.
- Controls and core combat actions are shared across both modes.

## Controls

Player 1:

- `A` / `D` = move
- `W` = jump
- `S` = crouch
- `F` = punch
- `G` = kick
- `R` = block

Player 2:

- `Left` / `Right` = move
- `Up` = jump
- `Down` = crouch
- `K` = punch
- `L` = kick
- `O` = block

System:

- `C` = toggle CPU for Player 2
- `H` = toggle hitbox debug
- `Space` = pause
- `Enter` = reset, and confirms menu and round-end prompts

Mobile:

- Touch controls appear automatically.
- `JUMP LEFT` and `JUMP RIGHT` buttons provide mobile-friendly diagonal jumps.
- Portrait and landscape are both playable.
- Landscape gives the roomiest view when the browser supports it cleanly.
- For the best phone experience, use landscape and choose `Add to Home Screen` for fullscreen play.
- Player 2 CPU is enabled by default on phones/tablets.

## Local Play

Open `index.html` directly in a desktop browser, or host the repository with any static file server.

No build step is required for local play.

## Attribution

Created by [@VibezZzCoder](https://github.com/VibezZzCoder).

Hangar Fighter is an independent fan/prototype project and is not an official U.S. Air Force product. It is not endorsed by, sponsored by, or affiliated with the U.S. Air Force, the Department of the Air Force, or the U.S. Department of Defense.

The project uses fictionalized, stylized, military-inspired characters and settings. No official endorsement is implied.

## Contributing

Issues, suggestions, and pull requests are welcome. Please keep contributions respectful and consistent with the project's fictional, unofficial nature.

## License

Hangar Fighter is licensed under the GNU General Public License v3.0 or later.

Copyright (C) 2026 VibezZzCoder

This project is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or, at your option, any later version.

This project is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

The license applies to this project's original code and assets. It does not grant rights to use any third-party trademarks, logos, seals, emblems, or official marks.

The copyright notice applies to this independent fan/prototype project's original code and original assets only. It does not claim ownership of, endorsement by, or affiliation with the U.S. Air Force, the Department of the Air Force, or the U.S. Department of Defense.

See `LICENSE` for the full license text.

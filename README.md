# Omar's Game Arcade

A simple website that lists the games in this repository dynamically.

## Website structure

- `index.html` — arcade home page; it reads the catalog from `games.json`.
- `games.json` — the list of games shown on the home page.
- `games/<game-slug>/index.html` — each game's independent, self-contained page.

## Current games

- Pyramid Jumper
- Cloud Hopper: The Sky Is Falling
- Mountain Climber
- Elemental Fighters
- The High Sky
- Sky Panic: Money Rush

## Add or update a game independently

1. Create a new folder such as `games/my-new-game/`.
2. Put that game's complete HTML in `games/my-new-game/index.html`.
3. Add one object to `games.json` with a unique `slug`, `title`, `description`, and `path`.
4. Commit the change. The home page automatically renders the new game from the catalog.

To update a game later, edit only that game's `index.html` unless its catalog title or description also needs changing. Keep CSS and JavaScript embedded in the game's HTML when practical, so game files remain portable and independent.

## Publish the website

Enable GitHub Pages for this repository from **Settings → Pages**, using the `main` branch and `/(root)` as the source if the repository/account plan supports Pages for its current visibility. The arcade URL will be shown by GitHub Pages after deployment.

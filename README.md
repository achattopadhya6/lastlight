# LASTLIGHT

An original browser battle royale prototype built with Three.js. A single player fights 15 bots on a procedurally illustrated low-poly island. No account, game server, or paid service is required to play.

## Play online

After GitHub Pages is enabled for the repository, open:

**https://achattopadhya6.github.io/lastlight/**

## Play

Serve the repository root with any static HTTP server, then open `index.html`. WebGL and JavaScript must be enabled. Use a mouse and keyboard for the best experience; basic touch controls are included. All game logic and 3D geometry run locally. This is a single-player prototype, not an online multiplayer service.

- WASD: move; mouse: look; left click: fire; right click: aim
- Shift: sprint; Space: jump
- 1/2/3: assault rifle, shotgun, marksman rifle
- R: reload; E: use a medkit; Q: place destructible cover
- Escape: pause; M: toggle synthesized audio
- Walk over glowing supplies to collect ammo, shield, medkits, and building supplies.

Matches contain 16 total combatants. The storm starts closing after 40 seconds and narrows to an 8-unit radius. Bots fight each other and the player, seek the safe zone, and use visibility checks before firing. The last survivor wins. Replay reloads the game with new bot and loot placement.

## Source

`game.js` contains the original scene, input, third-person camera, animation, collision, weapon, bot, storm, and match logic. `style.css` and `index.html` provide the responsive UI. Three.js r170 loads from jsDelivr under the MIT license. Optional Google Fonts have local system fallbacks.

## Current limits

No online multiplayer, persistent progression, matchmaking, full building editor, interiors, or downloadable native application. Desktop mouse capture depends on the browser allowing pointer lock; dragging to look is the fallback. Bots use lightweight local steering rather than a navigation mesh. Gameplay logic has been exercised with a Node simulation harness; full browser playtesting has not been performed.

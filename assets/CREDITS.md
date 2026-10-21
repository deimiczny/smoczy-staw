# Asset credits and provenance

All art in this folder was **AI-generated on 2026-10-21 with the Phaser Game Agent** (MCP tools
`establish_game_style`, `generate_sprites`, `generate_background`, `generate_logo`) for the account
used to build Smoczy Staw, then normalized locally (trimmed, cropped, resized, recolored).

- **Style:** `style-f84ac1dcbf`, "painted" mode (`story` preset), 1280×720, smooth scaling.
- **Source CDN:** `https://gameblocks.nyc3.digitaloceanspaces.com/art/<set>/…` (full-resolution `.full.png` files were used as sources).

| Folder | Source set(s) | Local processing |
|---|---|---|
| `dragons/` | `dragon-blue`, `dragon-yellow`, `dragon-pink`, `dragon-green2` | Trimmed, 512 px wide. `iskierka.png` is `dragon-blue` hue-shifted +55° (the purple generation was lost to background removal). |
| `portraits/` | `portraits` | Trimmed, max 320 px. |
| `fish/` | `fish` | Trimmed, max 192 px. |
| `creatures/` | `creatures-items` | Gloomer and dragonfly recovered from the background-removed sheet; a stray flame fragment cropped off the Gloomer. |
| `ui/heart*.png` | `creatures-items` | Stray fragment removed from the red heart (kept the main alpha island). |
| `icons/` | `icons` | Trimmed, max 128 px. |
| `deco/` | `decorations` | Recovered from the background-removed sheet; daisies, reeds and the stone are rectangle crops that avoid stray style-reference fragments. |
| `tex/deep.jpg`, `tex/shallow.jpg` | `tex-deep-water`, `tex-shallow-water` | Resized to 1536 px; deep water blurred and lowered in contrast. Stretched once over the pond in game (not tiled). |
| `tex/grass.jpg` | `tex-grass` | Mirror-tiled 2×2 into a seamless 1024 px tile. |
| `ui/select-bg.jpg` | `select-bg` | Cropped to 1280×720. |
| `ui/logo.png` | `logo-6525055998` | Trimmed, 900 px wide. |

Code-drawn (not generated): particles, glows, edge arrows, the bubble shield, radius rings, the
food bar, cooldown sweeps, foam lines and the pond outline.

## Audio

| File | Source | Notes |
|---|---|---|
| `audio/music-main.mp3` | Phaser Game Agent `generate_music` (clip model, chiptune), `music/a-cute-top-down-eat-and-grow-game-for-yo-9da338d2db8d.mp3` | 30.8 s loop; the game skips the first 0.06 s (MP3 padding). |
| `audio/music-gloom.mp3` | Phaser Game Agent `generate_music` (clip model, chiptune), `music/the-same-cute-kids-pond-game-about-baby-c518c8eb1a0c.mp3` | 30.8 s loop, crossfaded in during Gloom Waves. |

All sound effects and the win/lose jingles are synthesized at runtime in `src/audio/Sfx.ts` (no audio files).

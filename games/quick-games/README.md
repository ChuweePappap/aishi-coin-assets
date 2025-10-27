# Quick Games Folder

This folder contains casual WebGL games for the "Quick Games" category.

## Game Folders:

- **brick-smasher/** - Classic brick breaking game (formerly test-game-1)
- **speed-runner/** - Fast-paced reflex game
- **memory-match/** - Memory card matching game
- **bubble-pop/** - Bubble popping game

## How to Add a New Game:

1. Create a new folder with the game name (use lowercase and hyphens)
2. Place your WebGL build inside:

   ```
   your-game-name/
   ├── index.html
   ├── Build/
   │   ├── your-game.loader.js
   │   ├── your-game.framework.js.gz
   │   ├── your-game.data.gz
   │   └── your-game.wasm.gz
   └── TemplateData/
       └── style.css
   ```

3. Update the game list in `src/app/page.tsx`:
   - Add to the Quick Games carousel
   - Match the folder name with the game ID
   - Use the format: `quick-games/your-game-name`

## Important:

- Folder names should match the game IDs in kebab-case
- Keep the standard Unity WebGL structure
- Test locally before deploying

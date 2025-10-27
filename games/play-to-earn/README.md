# Play to Earn Games Folder

This folder contains reward-based WebGL games for the "Play to Earn" category.

## Game Folders:

- **test-game-1/** - Already exists (move from parent folder)
- **test-game-2/** - Already exists (move from parent folder)
- **treasure-hunt/** - Treasure hunting game with rewards
- **crypto-race/** - Racing game with prize mechanics

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
   - Add to the Play to Earn carousel
   - Match the folder name with the game ID
   - Use the format: `play-to-earn/your-game-name`

## Important:

- Folder names should match the game IDs in kebab-case
- Keep the standard Unity WebGL structure
- These games require AIShi token payment before playing
- Test locally before deploying

## Note:

You may want to move `test-game-1` and `test-game-2` from the parent `games/` folder into this `play-to-earn/` folder for better organization.

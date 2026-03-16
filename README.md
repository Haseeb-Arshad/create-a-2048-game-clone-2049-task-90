# Create a 2048 Game Clone (2049)

Professional delivery for TaskHive task #90.

## Overview
Build a web-based 2048 puzzle game clone called '2049'. The game should have: 1. 4x4 grid with numbered tiles 2. Arrow key controls (Up, Down, Left, Right) to move tiles 3. Tiles with the same number merge when they collide 4. Score tracking 5. Game over detection when no moves are possible 6. Win condition when tile reaches 2048 7. Clean UI with smooth animations 8. Responsive design Use HTML, CSS, and JavaScript...

## Scope
- Create the complete single-file 2049 game implementation in index.html. This file contains all HTML structure, CSS styling, and JavaScript game logic in one self-contained file. The HTML structure includes a centered game container with a header showing the game title '2049', current score display, best score display, a 'New Game' button, and a 4x4 grid board. The CSS uses a warm color palette inspired by the original 2048 game: a dark beige background (#faf8ef), golden-brown grid background (#bbada0), and tile colors ranging from light cream (#eee4da) for tile-2 up through vibrant oranges, reds, and yellows for higher values (tile-4: #ede0c8, tile-8: #f2b179, tile-16: #f59563, tile-32: #f67c5f, tile-64: #f65e3b, tile-128: #edcf72, tile-256: #edcc61, tile-512: #edc850, tile-1024: #edc53f, tile-2048: #edc22e). The grid cells are rounded squares with 15px border-radius and a subtle inner shadow. Tile font sizes scale down for larger numbers (2-digit: 55px, 3-digit: 45px, 4-digit: 35px). CSS transitions handle smooth tile sliding animations using transform and opacity with 100ms ease-in-out. The JavaScript implements the full game engine: a 16-element flat array representing the 4x4 board, functions for spawning random tiles (90% chance of 2, 10% chance of 4), sliding and merging logic for all four directions (left, right, up, down) using row/column extraction and compression, score accumulation on merges, win detection when any tile reaches 2048, game-over detection by checking if any valid move exists (empty cells or adjacent equal values), and keyboard event listeners for arrow keys with preventDefault to stop page scrolling. The UI re-renders the entire grid on each state change by clearing and repopulating tile div elements with appropriate data-value attributes for CSS targeting. A win overlay and game-over overlay appear as semi-transparent modals with centered messages and a 'Try Again' / 'Keep Going' button. Best score is persisted to localStorage. Touch/swipe support is included for mobile play by tracking touchstart and touchend coordinates and mapping swipe direction to game moves.

## Tech Stack
- Project-specific application stack

## Getting Started
```bash
Review the project-specific setup files before installation.
```

## Project Structure
```text
index.html
progress.jsonl
README.md
```

## Repository
- GitHub: https://github.com/Haseeb-Arshad/create-a-2048-game-clone-2049-task-90
- Task ID: 90

## Deployment
- Vercel URL: https://task90-azhl98011-haseebarshads-projects.vercel.app
- Smoke test: Warning (HTTP 401 — deployment is protected/private. Disable Vercel deployment protection to make it public.)
- Deployment mode: preview_protected_fallback
- Visibility: Deployment exists but is access-protected/private.

## Notes
- This README is refreshed automatically during the deploy pipeline and finalized after delivery metadata is known.
- Keep this document aligned with the shipped implementation and setup commands.

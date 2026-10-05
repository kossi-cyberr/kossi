# SES - Survival Escalade
A game where you shoot down descending projectiles.

## Project Structure
- `index.html` - The game page with UI and styles
- `game.js` - The game engine (classes, collision, rendering)

## How to Play
- Open `index.html` in a browser
- Click to shoot projectiles (bullets)
- Click on descending projectiles to kill them
- Survive as long as possible to increase your score

## Architecture
- `Game` class: Main game loop, state management, and rendering
- `Projectile` class: Represents a projectile (has a `Path2D` shape, position, velocity)
- `Obstacle` class: Represents an obstacle (background object)
- `PathGenerator` class: Generates shapes (circle paths via Path2D)
- Collision detection using AABB (axis-aligned bounding box)

## Key Features
- Canvas-based rendering with requestAnimationFrame
- Projectile spawning system
- Collision checks between projectiles and obstacles
- Difficulty scaling (level increases every 50 points)
- FPS counter and UI updates
- Responsive canvas sizing

## Assets
- Uses browser Canvas API (no external assets needed)
- Shapes generated via Path2D (circles)

## Notes
- The game is designed to be expandable
- Code is structured for maintainability and potential modding

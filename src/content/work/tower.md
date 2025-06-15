---
title: Tower Defense Game Development
publishDate: 2023-04-02 00:00:00
img: /assets/tower.png
img_alt: Example from a Tower Defense game showing enemies and towers
description: |
  A Tower Defense game project focusing on functional programming techniques to create a dynamic, grid-based world where actors (enemies, towers) interact in a strategic environment. Build the game engine, define phases, and manage interactions using pure functions.
tags:
  - Game Development
  - Functional Programming
  - Tower Defense
  - TypeScript
  - Multi-Agent Systems
---

## Tower Defense Game Development

##### Project Overview

Tower Defense is a genre of video games where the player defends terrain from waves of enemies determined to overwhelm the defenses. Enemies follow one or more paths toward an objective and are slowed or blocked by towers through elimination, blocking, slowing effects, etc.

This project, inspired by games like *Kingdom Rush*, lets players strategically place towers and characters along predefined paths to protect the objective.

> **Note:** This project emphasizes **functional programming** (purity and first-class functions) and prohibits object-oriented features such as classes or the `this` keyword. Runtime interaction beyond initial setup is out of scope.

##### Key Features

- **Grid-Based World:** A 2D grid where actors (towers, enemies) are placed and interact.  
- **Multiple Phases:** Each turn consists of phases (move, block, target, fight, etc.).  
- **Functional Paradigm:** All game elements and interactions driven by pure functions.  
- **Autonomous Actors:** Each actor has a decision-making function.  
- **Procedural Generation:** Automatic creation of paths and environments.  
- **Visualization:** Starts text-based, with an optional HTML front end.  

##### Game Phases & Mechanics

- **Move Phase:** Enemies propose movements; the engine resolves conflicts (e.g., collisions).  
- **Block Phase:** Towers and characters block enemy movement.  
- **Target Phase:** Towers select targets based on proximity or custom criteria.  
- **Fight Phase:** Damage calculations are applied; actors may be removed if defeated.  

##### Functional Programming Approach

Actors are immutable entities with actions defined by pure functions. Each action returns an intention (e.g., move, attack), and the engine applies them in sequence.

const actor = {
  pos: { x: 5, y: 7 },
  actions: {
    move: (actor, world) => ({ dx: 1, dy: 0 })
  }
};

##### Project Structure

/               -- Base directory
Makefile        -- Build and run commands
package.json    -- npm configuration
/src            -- Source files (TypeScript)
/tst            -- Test files
/html           -- HTML/CSS visualization
/dist           -- Bundled output

##### Installation & Dependencies

1. **Clone the repo:**
   - git clone https://github.com/yourusername/tower-defense.git
   - cd tower-defense
2. **Install dependencies:**
   - npm install
3. **Build & run:**
   - make build
   - make run
4. **Run tests:**
   - make test
   

##### Development Guidelines

* **TypeScript:** Pure FP style, no classes or `this`.
* **ESLint:** Lint with `npx eslint src tst`.
* **Jest:** Unit tests via `npx jest tst/*.ts`.
* **Parcel (optional):** Serve HTML/CSS with `npx parcel dist/index.html`.

##### Future Improvements

* **AI Actors:** Smarter pathfinding and strategy.
* **Interactive UI:** HTML/CSS front end for live visualization.
* **Additional Phases:** Healing, trading, special abilities.
* **Enhanced Generation:** More varied procedural maps.




---
title: Mansuba Project
publishDate: 2023-02-01 00:00:00
img: /assets/Chaturanga_Chess_Set.jpg
img_alt: A representation of the Mansuba board game inspired by Shatranj
description: |
  A generic board-game framework inspired by ancient games like Shatranj and Chinese Checkers. This project provides the core engine for defining pieces, move rules, and win conditions, along with tooling to compile, run, and test the game.
tags:
  - C Programming
  - Board Games
  - Game Development
  - Object-Oriented Design
---

## Mansuba Project

> A flexible framework for turn-based board games inspired by Shatranj and Chinese Checkers.

This project implements a generic board-game engine where you can define custom piece types, movement rules, and victory conditions. The initial reference implementation models a simple two-player grid game with capture mechanics and win-by-elimination rules.

### Prerequisites

- **GCC** (GNU Compiler Collection)
- **Make**
- **Linux** or POSIX-compatible environment

### Features

- **Modular game server:** core engine for turn management, move validation, and state serialization
- **Plugin-based clients:** dynamically loadable player modules implementing custom strategies
- **Configurable boards:** support for multiple board topologies (square grid, hex grid, custom graphs)
- **Capture mechanics:** define how pieces interact and eliminate opponents
- **Win conditions:** easily specify victory rules (last-piece standing, area control, reach target)

### Installation

1. **Clone the repository**

   - git clone [REPO_URL]
   - cd [PROJECT_NAME]

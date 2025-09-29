# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a vanilla JavaScript Snake game application deployed on Azure Static Web Apps. The project consists of:
- A standalone Snake game (`snake.html`) - fully self-contained HTML file with inline CSS and JavaScript
- A basic landing page (`index.html`) with external stylesheet (`styles.css`)

## Commands

### Development Server
```bash
npm start
```
Runs a local server using sirv on port 8000 with CORS and single-page app support.

### Dependencies
No build process required. This is a vanilla HTML/CSS/JavaScript application.

## Architecture

The codebase is intentionally simple:
- **snake.html**: Complete Snake game implementation in a single file (270 lines)
  - Uses HTML5 Canvas for rendering
  - Vanilla JavaScript for game logic
  - Inline CSS for styling
  - No external dependencies

- **index.html**: Basic landing page (currently just displays a title)
- **styles.css**: Stylesheet for index.html

The Snake game features:
- Grid-based movement (20x20 grid)
- Score tracking
- Speed increases every 5 points
- Game over detection (wall collision, self-collision)
- Keyboard controls (arrow keys)
- Space key to restart after game over

## Deployment

Configured for Azure Static Web Apps deployment via GitHub Actions workflow.
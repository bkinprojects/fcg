### Poker Simulator

A single-file, zero-dependency browser-based Texas Hold'em poker simulator with a retro blueprint CAD aesthetic.

## Features

- Table and Geometry:
  - Widescreen rectangular poker table (3:1 aspect ratio).
  - Clean CAD blueprint wireframe styling with no blurry glow effects.
  - Classic Felt Green (#003318) default theme with dark and light mode support.
  - Real-time responsive HTML5 canvas rendering at 60 FPS.

- Visual Elements:
  - Face-up player hole cards rendered on the table felt above the user plaque.
  - Face-down CPU cards rendered inside the table felt with wireframe crosshatch backs.
  - Folded player cards automatically removed from the felt.
  - Large community board cards (Flop, Turn, River).
  - In-felt bet pods with layered wireframe chip stacks and dollar amount pills.
  - Inactive / checked $0 bet pods hidden automatically.
  - Scaled center pot badge flanked by wireframe chip stacks.
  - Crisp active turn indicators with dotted focus rings and action flashes.
  - High-contrast four-color deck option (Spades white/black, Hearts red, Diamonds blue, Clubs green).

- Game Logic and AI:
  - Texas Hold'em rules engine: pre-flop, flop, turn, river, and showdown.
  - Hand evaluation for all standard 5-card poker combinations.
  - Monte Carlo equity calculator for real-time win probability estimates.
  - Multi-way side pot computation and distribution for all-in scenarios.
  - Configurable CPU AI difficulty levels (from passive calling stations to balanced aggressive AI).
  - Adjustable CPU decision speed delay.

- Tournament Progression:
  - Persistent stack tracking carrying balances across consecutive hands.
  - Player elimination: CPUs reaching $0 chips are permanently marked eliminated.
  - Dynamic dealer button and blind rotation skipping busted players.
  - Heads-up rule transition when only two players remain.
  - Dedicated Victory screen when the human player captures all chips.
  - Dedicated Defeat screen when the human player's chips reach $0.
  - Manual tournament reset and rebuy options.

- Configuration and Customization:
  - Table configuration: 1 to 7 CPU opponents (2 to 8 seats), custom starting stacks, and custom blinds.
  - Quick match presets (Heads-Up, 3-Max, 6-Max, Full Ring).
  - UI Font Size scaling slider (90% to 130%) dynamically adjusting text and canvas elements.
  - Font family selector (Courier New, Times New Roman, Arial, Press Start 2P).
  - Palette settings: color picker, saturation, brightness, and hue shift adjustments.
  - Settings persisted in localStorage.

## Controls

- Action Buttons:
  - FOLD: Surrender the hand and forfeit any bets made.
  - CHECK: Pass action when there is no bet to call.
  - CALL: Match the current highest street bet.
  - BET / RAISE: Wager chips or increase the current bet size.

- Bet Sizing:
  - MIN: Set wager to the minimum allowable raise.
  - 1/2 POT: Set wager to half the current pot size.
  - POT: Set wager to the full pot size.
  - ALL-IN: Wager all remaining chips in your stack.
  - Slider: Drag to adjust the bet amount incrementally.
  - Number Input: Type an exact dollar value.

- Navigation and Management:
  - NEW TOURNAMENT: Reset all player stacks to the starting buy-in and start hand #1.
  - NEXT HAND: Progress to the next hand while preserving accumulated chip stacks.
  - REBUY: Add chips back to your stack after busting.
  - TABLE CONFIG: Access setup options to customize opponents, blinds, and starting stacks.
  - SETTINGS: Configure AI difficulty, animation speed, font size, colors, and display options.

# GameLingo project plan

GameLingo is a game-focused screen translator based on DeskTranslate 2. This repository starts as a fork and keeps the upstream history and MIT license.

> This file records the project direction. The code is still the inherited DeskTranslate application until a GameLingo-specific change is implemented and verified.

## Goal

Help players read dialogue and other text shown in PC games and emulator windows through OCR and a configurable translation overlay. The first version should work alongside a game or emulator without modifying game files or injecting into the emulator.

## First milestone

Build a focused game-session flow on top of the existing screen-capture and translation foundation:

1. Let the player choose a game or emulator window and source and target languages.
2. Guide the player to select the visible dialogue or subtitle region.
3. Run a sample OCR and translation before starting live capture.
4. Save the language, recognition, provider, and overlay settings as a profile for that game.
5. Make the translated text readable during play, with clear pause, resume, and stop controls.

## Acceptance criteria

- A player can configure one game or emulator window without changing its files.
- The selected region can produce a successful sample translation before live mode starts.
- The player can save and reload that title's settings.
- Live capture can be paused and stopped without closing the game.
- Existing upstream behavior and limitations are documented accurately; no OCR accuracy or emulator compatibility is assumed without evidence.

## Next decisions

Choose the first emulator to qualify, the initial language pairs, and whether the default translation path should be local or cloud-based before implementing provider-specific defaults.

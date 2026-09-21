# Hotkey Suite

Keyboard and gamepad hotkeys for the things Gen 1 makes you walk through a menu
for. Seven modules share one hub at `OPTIONS > HOTKEY SUITE`, so binds live in
one place instead of scattered across a mod list.

**Everything ships off.** Every module has its own `ENABLED` switch that starts
`OFF` with nothing bound, so installing the suite changes nothing until you opt
in. Press `START` on any setting for its help text.

## What it changes

- **Autofire Hotkeys** — toggle or hold, five repeat speeds. Fire a fixed button,
  or arm the next button you press. Optional on-screen indicator.
- **Menu Hotkeys & Radial Menu** — bind any START-menu entry to a button or a
  chord of up to four. Menu entries added by other mods are discovered
  automatically. The radial wheel reads either analog stick.
- **Travel Hotkeys** — Fly, return to the last Pokémon Center, and Bicycle,
  each checked against your Bag before it fires.
- **Battle Command Menu** — hold a hotkey and press a direction to pick FIGHT,
  PKMN, ITEM, RUN or a move, plus a dedicated Run button. Optionally shows each
  move's power, type and accuracy.
- **Battle Text** — auto-advance battle messages at four speeds, dismiss the
  level-up window, skip the level-up and move-learned fanfares, and page through
  the learn-a-move prompt up to (never through) the YES/NO.
- **Ball Menu** — a one-line ball selector for battle, or a quick-throw that
  falls back to the first ball in your Bag.

Binding supports gamepad triggers (LT/RT), which the engine's default binding
path does not pick up on its own.

## Compatibility

- Mod API 2, `content` profile: link play is unaffected.
- Adapts to modded battle UIs, drawing its legend against the live playfield
  rather than fixed coordinates, so it stays on screen in portrait on mobile.
- Integrates with **Kanto Ascendant** when present, relocating its START-menu
  entry into that mod's hub. Not required.
- Conflicts with the author's own superseded standalone mods `autofire_hotkey`,
  `menu_hotkeys` and `radial_menu`. Disable those.
- `engine_internals` is declared because the suite reads live battle and menu
  state to know when a hotkey is safe to act on.

## Install

1. Download `hotkey_suite-1.9.1.zip` from the releases page.
2. In the launcher, MODS → **Import mod .zip**.
3. Open `OPTIONS > HOTKEY SUITE`, enable a module, and assign its hotkeys.

Updates come through the launcher's **Update** / **Versions** buttons.

## Credits

Written by ojsaucer. MIT licensed. No ROM-derived content is distributed: the
move-info sword and percent sign are drawn from primitives at runtime.

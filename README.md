# Roll Ledger

## Purpose and features

Keep the table's public roll history in one report. See who rolled, what the
roll was for, and how the dice behaved without searching the chat log.

- Saves public roll records while a GM is online and keeps them after normal
  chat deletion.
- Shows roll events and individual dice as separate counts.
- Filters by date, system, character, player, roll type, die and action.
- Reads PF2e and D&D 5e action details; other systems use generic roll fields.
- Uses Foundry's light/dark theme, with an optional local theme choice.

This is a free, standalone module. It does not change dice results or reveal
private or blind rolls.

## Setup

Requires Foundry V13 or V14. Native action support covers PF2e 7.12.2 on V13
and PF2e 8.x on V14, plus dnd5e 5.3 on V13 and 6.0 on V14. Other systems
retain generic dice, formula, total, date and player data; their system-specific
action details have not been tested.

Install **Roll Ledger** with the
[SpazzMods Installer](https://github.com/Spazzletopia-Studios/spazzmods-installer/releases/latest),
or paste this into Foundry's **Install Module → Manifest URL** box:

`https://github.com/Spazzletopia-Studios/Roll-Ledger/releases/latest/download/module.json`

Enable **Roll Ledger** in your world's **Manage Modules** window. Keep at
least one GM connected so the recorder can save new rolls.

## Quick start

1. Make a normal public roll in the world while a GM is online.
2. Open **Settings → Configure Settings → Roll Ledger → Open Roll Ledger**.
   You can also select **SpazzMods** in the left scene controls and click
   **Roll Ledger**. Hub is optional.
3. Choose a **Session** date, or keep **All dates** to view the full history.
4. Click a player, a die or an action to narrow the report.
5. In **Latest rolls**, click an action name to open that roll's detail panel.
   Use **Close detail** to close it.

## Detailed use

### Filter the report

The top controls select **Session**, **System**, **Character** and **Type**.
Here, a session is a calendar date, not a named game session you create.

Click a player card to focus on that person. Player names and character names
are saved separately, so the same player's rolls can be viewed across their
characters. **All players** removes that filter.

Click a die chip such as **d20** to focus on that die type, or **All dice** to
remove it. Click an action bar to show its records. **All actions** lists
actions beyond the first few bars; **Clear action** returns to all actions.

### Read counts and dice results

**Roll events** counts saved evaluated rolls. **Individual dice** counts the
dice within them. One damage roll can contain several dice, so these totals
need not match. Action and damage events are listed separately.

The dice-results chart shows kept die values before modifiers. Natural 20s
and natural 1s describe the die, not the final success or failure. The table
shows the saved formula, total and any public outcome.

**Latest rolls** lists the newest matching records. Click **Show 100 more**
when available to reveal older rows. Click a row's action name for its saved
system details, player/character, formula and public target or outcome.
**Not recorded** or **Hidden or not recorded** means that value was not
available to the public recorder; it is not a guessed result.

### Keep and recover history

One active GM saves the records to module-owned Journal entries. Normal chat
deletion does not remove saved history. Do not delete those backing entries
if you want to keep the history.

When a GM returns, the recorder catches up from roll messages still present
in chat. Messages deleted before they were saved cannot be recovered. Older
5e chat messages may lack public targets or outcomes because their original
visibility settings cannot be safely recovered.

## Settings

Open **Settings → Configure Settings → Roll Ledger**.

- **Theme**: **System default**, **Light** or **Dark**. This changes only
  Roll Ledger on your device. An open report keeps its filters, focus and
  scroll when the theme changes.
- **Session timezone**: a GM sets the calendar-date timezone for new records.
  The default is **America/Chicago**. Use a named timezone such as
  **Europe/London**, not a numeric offset. An invalid value falls back to
  America/Chicago with a warning. Existing records retain their saved dates.

## Privacy, limits and help

- Private and blind rolls are omitted, along with hidden DCs and outcomes.
- PF2e action identity distinguishes Grapple from a plain Athletics check.
- PF2e reroll cards may contain only the kept result. A complete linked
  history of every physical reroll is not yet available.
- If the status says **Recording paused · no GM online**, reconnect a GM.
  If it reports a recording error or unreadable messages, preserve the error
  text and report it; do not assume those rolls were saved.

[Get Help](https://github.com/Spazzletopia-Studios/spazzmods-support). Include
your module, Foundry and game-system versions and the exact roll or filter
that caused the problem. Do not include private tokens or account details.

## Compatibility record

Recorded native test lines: Foundry 13.351/PF2e 7.12.2 and dnd5e 5.3.3;
Foundry 14.368/PF2e 8.5.0 and dnd5e 6.0.2. These are recorded tested versions,
not a claim that every later engine release has already been checked.

## Legal

This is an unofficial module, not endorsed by Paizo, Wizards of the Coast,
or Foundry Gaming. No copyrighted game text or native pack data is shipped.

# Erinn Progress Ledger

A single-page checklist and progress tracker for Mabinogi's winter 2026 Arcana season.

**Live page:** https://c3d-gg.github.io/mabinogi-ledger/

## What's on the page

- **Daily, weekly and monthly checklists** for the season's events (Master Plan, Pan's attendance, Erinn Adventure Pass, giveaway missions, shop runs)
- **Reset timers in server time** (Pacific): daily reset at 7 AM, weekly reset on Thursday
- **Event progress**: Pan stamps, Adventure Pass level, giveaway points, Arcana Awakening level, plus upcoming Hot Days and deadlines
- **Ogham rune synergies** for your main Arcana, with which runes you already own
- **Gear vs best-in-slot table**

## Saving

Progress is saved in each visitor's own browser (localStorage). Nothing is sent to a server, and progress doesn't carry over between browsers or devices.

## Editing gear

Gear rows are set in the `GEAR_DATA` list near the top of the script in `index.html`. Add one entry per slot:

```js
{order:1, slot:"Weapon", current:"...", bis:"...", next:"...", status:"far"},  // status: bis | close | far
```

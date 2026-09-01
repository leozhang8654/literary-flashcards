# Literary Elements Flashcards

Browser flashcards for the 55 literary terms on the English 11 *Literary Elements and Definitions* worksheet. One self-contained `index.html` — no build step, no dependencies.

**Live page:** enable GitHub Pages (Settings → Pages → Deploy from branch → `main` / root), then open `https://leozhang8654.github.io/literary-flashcards/`

## How to use it

| Action | How |
| --- | --- |
| Flip a card | Click the card, or press <kbd>Space</kbd> |
| Previous / next | <kbd>←</kbd> / <kbd>→</kbd>, or the buttons |
| Mark a card as tricky | <kbd>M</kbd>, or the ☆ button |
| Study only tricky cards | Click the **★ Tricky** chip |
| Quiz yourself the way the worksheet does | Switch to **Def → Term** |
| Randomize order | **Shuffle** |
| Skim everything before a test | **Quick reference** at the bottom |

Tricky marks are saved in the browser's `localStorage`, so they survive a reload on the same device.

## Categories

Plot (13) · Character (10) · Point of View (5) · Irony (4) · Figurative Language (12) · Language & Style (11)

## A note on the source

The worksheet is a fill-in-the-blank sheet: the "Literary Element" column is blank and only the definitions are given. The term names here were filled in from the definitions. Three were judgment calls worth checking against the teacher's answer key:

- "Two opposite contradictory ideas are joined" → **Oxymoron** (some courses call this Paradox)
- "The repetition of certain elements or events within the plot" → **Motif** (may be taught as Repetition)
- "The order in which events happen in time" → **Chronological Order**

## Editing the cards

All content lives in the `CARDS` array in `index.html`. Each entry is:

```js
{ en: "Metaphor", cat: "fig",
  def: "A comparison of two unlike things without using words such as like, as, than, or resembles.",
  ex: "“Time is a thief.”" },
```

`cat` must be one of the keys in `CATS` (`plot`, `char`, `pov`, `irony`, `fig`, `lang`); `ex` is optional.

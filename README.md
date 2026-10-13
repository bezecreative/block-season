# Block Season

A playable proposal for BoreBuddy: an 8-bit, first-person rifle range that runs in the browser.

**Play it:** https://bezecreative.github.io/block-season/

## How it plays

- Five moving targets are set from 30 to 120 yards. The far ones are specks until you scope in.
- Each round gives you eight shots and a clock. Hit at least three of the five to move on; targets speed up each round.
- A dead-centre hit pays double. Ducks flush out of the grass for bonus points, and the dog fetches the ones you hit.
- The rifle is modelled on BoreBuddy's Complete AR22 Apogee Match upper in FDE.

## Controls

| Key | Action |
|---|---|
| W A S D | Walk |
| Mouse | Aim |
| Space or click | Fire |
| Right-click or Q | Scope |
| Scroll | Scope zoom, 3x to 12x |
| Shift | Run |
| J | Jump |
| Esc | Pause |
| M | Sound on or off |

On a phone, the left thumb walks, the right thumb aims, and on-screen buttons fire, scope and jump.

## Adding the proposal link

In `index.html`, find `const PROPOSAL_URL = '';` and paste the link between the quotes. The title card then reads
"Either play your way through our proposal, or simply view it here" and gains a "View the proposal" menu item.

## Files

- `index.html` is the whole game: markup, styles and script in one file. It loads three.js r128 from cdnjs and the Press Start 2P font from Google Fonts.
- `borebuddy-logo.png` is BoreBuddy's logo, shown on the title card.

## Credits

The BoreBuddy name and logo belong to BoreBuddy and appear here as part of a proposal prepared for them.
The game's models and sounds are original; the look is a tribute to 8-bit light-gun games.

# A Proposal for BoreBuddy

A playable proposal for BoreBuddy, by Mox: an 8-bit, first-person shooting game that runs in the browser. Each round is a rifle range out in a field, then an office warehouse full of computers.

**Play it:** https://bezecreative.github.io/block-season/

## How it plays

**Stage one, the range.** Five moving targets are set from 30 to 120 yards. The far ones are specks until you scope in.
You get eight shots and a clock, and need at least three of the five to move on. A dead-centre hit pays double.
Ducks flush out of the grass for bonus points, and the dog fetches the ones you hit.

**Stage two, the office.** The scene cuts to a warehouse office with ten computers: on desks, up on a mezzanine and
riding a conveyor. Three screens show NEMO Arms, three show Smith & Wesson, three show BoreBuddy's own homepage and one
is dead. Scope in to read them and shoot the six competitor screens. You get nine shots and need at least four.
Hitting a BoreBuddy screen costs 1,000 points.

**The pitch.** When the office ends, a card reads "Want to stand out? Go with Mox", with a link to the proposal and a
button to keep playing. Carrying on starts the next round back at the range, faster.

The rifle carries BoreBuddy's AR22 Heavy Precision upper with the 18.5-inch Green Mountain barrel.

## Controls

| Key | Action |
|---|---|
| W A S D | Walk |
| Mouse | Aim |
| Space or click | Fire |
| Right-click or Q | Scope |
| Scroll | Scope zoom, 3x to 16x |
| Esc | Pause |
| M | Sound on or off |

On a phone, the left thumb walks, the right thumb aims, and on-screen buttons fire, scope and jump.

## Adding the proposal link

In `index.html`, find `const PROPOSAL_URL = '';` and paste the link between the quotes. That switches on the
"I just want to see your proposal" button on the title card and the "View proposal" link on the card after the office.

## The office screens

Each site's screen shows a screenshot file where one is listed in `const SCREENSHOTS = { ... };` in `index.html`,
and a simplified drawing in that site's colours otherwise. To add or swap one, put the image in `screens/` and set
its path there, for example `bb: 'screens/borebuddy.jpg'`. The top-left of the image is cropped to 4:3, which keeps
the logo in view. Only add screenshots you have the right to publish.

## Files

- `index.html` is the whole game: markup, styles and script in one file. It loads three.js r128 from cdnjs and the Press Start 2P font from Google Fonts.
- `borebuddy-logo.png` and `mox-logo.png` are the logos on the title card.
- `screens/` holds the homepage screenshots shown on the office computers.

## Credits

The BoreBuddy name and logo belong to BoreBuddy and appear here as part of a proposal prepared for them.
The office screens show supplied screenshots of the BoreBuddy, NEMO Arms and Smith & Wesson homepages. Those sites,
names and marks belong to their owners.
The game's models and sounds are original; the look is a tribute to 8-bit light-gun games.

# Block Season

A playable proposal for BoreBuddy: an 8-bit, first-person shooting game that runs in the browser. Each round is a rifle range out in a field, then an office warehouse full of computers.

**Play it:** https://bezecreative.github.io/block-season/

## How it plays

**Stage one, the range.** Five moving targets are set from 30 to 120 yards. The far ones are specks until you scope in.
You get eight shots and a clock, and need at least three of the five to move on. A dead-centre hit pays double.
Ducks flush out of the grass for bonus points, and the dog fetches the ones you hit.

**Stage two, the office.** The scene cuts to a warehouse office with ten computers: on desks, up on a mezzanine and
riding a conveyor. Three screens show the BoreBuddy homepage, three show NEMO Arms, three show Smith & Wesson and one
is dead. Scope in to read them and shoot only the three BoreBuddy screens. You get six shots; a wrong screen costs 500 points.

Clear the office and the next round starts back at the range, faster.

- The rifle is modelled on BoreBuddy's Complete AR22 Apogee Match upper in FDE.

## Controls

| Key | Action |
|---|---|
| W A S D | Walk |
| Mouse | Aim |
| Space or click | Fire |
| Right-click or Q | Scope |
| Scroll | Scope zoom, 3x to 16x |
| Shift | Run |
| J | Jump |
| Esc | Pause |
| M | Sound on or off |

On a phone, the left thumb walks, the right thumb aims, and on-screen buttons fire, scope and jump.

## Adding the proposal link

In `index.html`, find `const PROPOSAL_URL = '';` and paste the link between the quotes. The title card then reads
"Either play your way through our proposal, or simply view it here" and gains a "View the proposal" menu item.

## Using real screenshots on the office screens

The three site screens are drawn in code by default. To use your own screenshots, add the image files to this
folder (for example `screens/borebuddy.png`) and put their paths in `const SCREENSHOTS = { bb: '', nemo: '', sw: '' };`
in `index.html`. The top of each image is cropped to 4:3. Only add screenshots you have the right to publish.

## Files

- `index.html` is the whole game: markup, styles and script in one file. It loads three.js r128 from cdnjs and the Press Start 2P font from Google Fonts.
- `borebuddy-logo.png` is BoreBuddy's logo, shown on the title card.

## Credits

The BoreBuddy name and logo belong to BoreBuddy and appear here as part of a proposal prepared for them.
NEMO Arms and Smith & Wesson are named on the office screens; those names belong to their owners. The screens are
simplified drawings in each site's colours, not screenshots.
The game's models and sounds are original; the look is a tribute to 8-bit light-gun games.

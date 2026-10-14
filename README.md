# A Proposal for BoreBuddy

A playable proposal for BoreBuddy, by Mox: an 8-bit, first-person shooting game that runs in the browser. Each round is a rifle range out in a field, then an office warehouse full of computers.

**Play it:** https://bezecreative.github.io/block-season/

## How it plays

**Stage one, the range.** Five moving targets are set from 30 to 120 yards. The far ones are specks until you scope in.
You get eight shots and a clock. However it goes, the game moves on to the office. A dead-centre hit pays double.
Ducks flush out of the grass for bonus points, and the dog fetches the ones you hit.

**Stage two, the office.** The scene cuts to a warehouse office with fifteen computers. Eight sit still on desks and
a mezzanine; seven move, riding a conveyor, hanging from overhead trolleys and rising on scissor lifts. Three screens
show BoreBuddy's homepage and the other twelve show NEMO Arms and Smith & Wesson. The card reads "Let's see how your
website stacks up against the competition. Shoot your website to score points." Hitting a competitor screen costs 500 points.

**Stage three, the billboard.** Back outside, a billboard stands beside a two-lane highway and reads "Ready to stand
out? Go with Mox" with a target on it. Pickup trucks drive by now and then. Deer wander the field and ducks fly over for
bonus points (does 600, bucks 1,000). There is no clock and no shot limit. Hitting the billboard target loads the
proposal page. This stage draws at full resolution, so the billboard reads clean; the first two keep the chunky pixels.

The rifle carries BoreBuddy's AR22 Heavy Precision upper with the 18.5-inch Green Mountain barrel.

## Controls

| Key | Action |
|---|---|
| Mouse | Aim |
| Space or click | Fire |
| Right-click or Q | Scope |
| Esc | Pause |
| M | Sound on or off (also the speaker button on screen) |

On a phone, drag anywhere to aim; on-screen buttons fire and scope. Players stay in one spot and don't walk.

## The proposal

`proposal.html` is Mox's website proposal for BoreBuddy. The game links to it from the "I just want to see your
proposal" button on the title card and the target on the billboard at the end of the game. The link lives in
`const PROPOSAL_URL` near the top of the script in `index.html`. It is the relative path `proposal.html`, so the game
and the proposal stay on whichever host serves them. The proposal's menu has a "Back to the Game" link.

## The office screens

Each site's screen shows a screenshot file where one is listed in `const SCREENSHOTS = { ... };` in `index.html`,
and a simplified drawing in that site's colours otherwise. To add or swap one, put the image in `screens/` and set
its path there, for example `bb: 'screens/borebuddy.jpg'`. The top-left of the image is cropped to 4:3, which keeps
the logo in view. Only add screenshots you have the right to publish.

## Files

- `index.html` is the whole game: markup, styles and script in one file. It loads three.js r128 from cdnjs and the Press Start 2P and Archivo fonts from Google Fonts.
- `borebuddy-logo.png` and `mox-logo.png` are the logos on the title card.
- `screens/` holds the homepage screenshots shown on the office computers.
- `proposal.html` is the proposal page the game links to.
- `team/` and `logos/` hold images the proposal serves itself (a roster photo, the Micron logo).
- `vercel.json` and `.vercelignore` set up the Vercel copy.

## Credits

The BoreBuddy name and logo belong to BoreBuddy and appear here as part of a proposal prepared for them.
The office screens show supplied screenshots of the BoreBuddy, NEMO Arms and Smith & Wesson homepages. Those sites,
names and marks belong to their owners.
The game's models and sounds are original; the look is a tribute to 8-bit light-gun games.

# Game is Hard – Level 19 (“I need some rest”) — Walkthrough + Mini Clone

Level 19 is the first “stop touching stuff” check that hard-punishes fidget hands.

## One-line solution (the whole level)
Put your phone flat on a solid table (screen up) and don’t touch it until the orange text turns green, then tap the green **Play** button.

## Recommended walkthrough (with screenshots)
If you want the cleanest reference (and images you can share), use:
- https://gameishard.org/level/19

It gives:
- The exact phrasing for the level
- A quick answer section
- Multiple screenshots showing the state change (orange → green) and the Play button appearing

## What’s in this repo
This repo is two things:
1. A fast, copy-paste-friendly writeup for **Level 19**
2. A tiny browser-based “clone” of the mechanic (flat + still → success)

## Repo structure
.
├─ README.md
└─ level19-clone/
└─ index.html


## Run the mini clone locally
You’ll need a local server (mobile browsers block motion sensors on `file://`).

1. `cd level19-clone`
2. Start a server:
   - Python: `python3 -m http.server 8080`
3. Open:
   - Desktop: `http://localhost:8080`
   - Phone: use your machine’s LAN IP like `http://192.168.x.x:8080`

## How the clone works (matching the real trick)
The clone clears when BOTH are true:
- **Flat**: the phone is roughly face-up (orientation near 0)
- **Still**: motion stays under a small threshold for ~2.5 seconds

When it clears:
- Text flips from orange to green
- A green triangle **Play** button appears
- Tap it to “finish”

## Common fails (aka why people get stuck)
- Holding it “perfectly still” in your hand. Your hand is never still.
- Wobbly case / grip on the back so the phone rocks.
- Not granting motion permission on iOS (you must tap the enable button).

## Credit
- Original level/game: Unico Studio’s **Game is Hard**
- Walkthrough reference page: gameishard.org Level 19
- This clone: fan-made, for learning and repo demo purposes

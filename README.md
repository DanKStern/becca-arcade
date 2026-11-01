# Becca's Arcade

A tiny arcade of browser games, built in an afternoon. `index.html` is the menu; each game is its own static page, no build step, no frameworks.

- **Pitch Bird** (`pitch-bird.html`) — sing higher to fly up, lower to dive down, dodge the pipes. Uses the Web Audio API to detect pitch live from the microphone (autocorrelation) and maps it to the bird's height. Nothing is recorded or uploaded. Add `?test` to the address to fly a demo tone instead of using the mic.
- **Memory Match** (`memory-match.html`) — classic flip-two-cards matching game, Easy (20 cards) or Hard (30 cards).
- **Sound Match** (`sound-match.html`) — match a sound (flute, triangle buzz, square buzz, water drip, all synthesized live) to its oscilloscope-style picture, or the other way around. Alternates direction each round.
- **Takeaway Tower** (`takeaway-tower.html`) — pick the answer to "100 − X", then watch a 100-block tower shrink to check: full ten-rows disappear first, then the leftover ones, so regrouping is visible rather than abstract.
- **Mirror Maker** (`mirror-maker.html`) — a free-draw toy, not a scored game. Draw on the canvas and it reflects live, either side-to-side or full 4-way (mirrored across both axes). 💾 Save downloads a PNG.
- **Mix-It Lab** (`mix-it-lab.html`) — tap red/yellow/blue blobs to mix them in the bowl and match a target color. Uses real paint-style (RYB) mixing math, not RGB averaging, so red+yellow actually makes orange.

Run it by opening `index.html` in Chrome, or serve the folder (`python -m http.server`) and open `http://localhost:8000`. Pitch Bird specifically needs the `http://` serving — Chrome blocks microphone access from a bare `file://` page.

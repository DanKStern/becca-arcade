# Becca's Arcade

A tiny arcade of browser games, built in an afternoon. `index.html` is the menu; each game is its own static page, no build step, no frameworks.

- **Pitch Bird** (`pitch-bird.html`) — sing higher to fly up, lower to dive down, dodge the pipes. Uses the Web Audio API to detect pitch live from the microphone (autocorrelation) and maps it to the bird's height. Nothing is recorded or uploaded. Add `?test` to the address to fly a demo tone instead of using the mic.
- **Memory Match** (`memory-match.html`) — classic flip-two-cards matching game, Easy (12 cards) or Hard (16 cards).

Run it by opening `index.html` in Chrome, or serve the folder (`python -m http.server`) and open `http://localhost:8000`.

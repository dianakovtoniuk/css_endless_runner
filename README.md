# CSS Endless Runner

An endless runner scene built with the Web Animations API. A character runs along a road with parallax layers, jumps with a ground shadow, and shares the road with passing cars.

## Features

- **Run cycle:** the character is a sprite sheet animated with `steps(8)` by shifting `background-position`.
- **Parallax:** the street, background and foreground scroll at different speeds.
- **Jump:** the run cycle pauses mid-air while the character jumps, and a shadow on the ground scales in sync.
- **Speed control:** the whole scene can be sped up, slowed down, paused and resumed through `document.getAnimations()` and `playbackRate`. The speed also slowly decays on its own.
- **Traffic:** cars with random speeds drive across the road, with wheels rotated through the `:before` and `:after` pseudo-elements using the `pseudoElement` option.
- **Async flow:** `animation.finished` and `animation.ready` promises drive the jump and car spawning.

## Controls

| Key         | Action                   |
| ----------- | ------------------------ |
| Arrow Up    | Jump                     |
| Arrow Right | Run faster               |
| Arrow Left  | Run slower               |
| Space       | Pause / resume the scene |

## Run

No build step. Open `index.html` in a browser.

## Project structure

```
index.html   page markup
styles.css   scene layout, character and car styles
script.js    all animations and keyboard controls
assets/      sprites, clouds, background layers, car and wheel
```

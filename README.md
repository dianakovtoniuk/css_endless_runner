# CSS Endless Runner

A pure CSS endless runner scene with parallax layers and a sprite-sheet run cycle. Built as an exercise for a web animations course.

## How it works

- **Run cycle:** the character is a sprite sheet animated with `steps(8)` by shifting `background-position`.
- **Scrolling:** the street loops with `translateX`, while the background and foreground move at different speeds to create a parallax effect.
- **Timing:** all speeds derive from a single `--duration` CSS variable.
- **Jump:** pressing Space adds a `jump` class. It is removed on `animationend`, so the jump can be triggered again.

## Run

No build step. Open `exercise-1/index.html` in a browser.

## Controls

| Key   | Action |
| ----- | ------ |
| Space | Jump   |

## Project structure

```
exercise-1/     the runner scene (HTML, CSS, assets)
animations/     keyframes and animation events
transitions/    transitions and @starting-style
timing-funcitons/  timing functions demo
```

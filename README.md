# fallout-skill-shot-timer

When to launch the ball so it rolls over the skill shot light while the light is ON.

**Live page:** https://sbeckeriv.github.io/fallout-skill-shot-timer/

## What it does

- Works out the launch window and the best cue (light turning ON or OFF) for each phase.
- Everything is adjustable: ball travel time, your reaction time, and each phase's on/off durations. Settings are saved in your browser.
- Practice mode blinks a light at the phase's real rhythm. Press **Launch** (or Space) and it tells you whether the ball would have hit while the light was on, and how early or late you were.

## Default timings

| Phase | On | Off | Cycle |
|---|---|---|---|
| 1 | 2.04 s | 2.17 s | 4.21 s |
| 2 | 0.92 s | 1.22 s | 2.15 s |
| 3 | 4.13 s | 12.43 s | 16.56 s |

The light timings were read from video frame timestamps. Ball travel defaults to 2.3 s (phone stopwatch) and reaction time to 0.22 s.

## Hosting

The whole site is one static `index.html` with no build step. It's served by GitHub Pages from the `main` branch.

# fallout-skill-shot-timer

When to launch the ball so it rolls over the right inlane light while the light is ON. The two inlane lights alternate. The page uses both to find the easiest light change to time your shot from.

**Live page:** https://sbeckeriv.github.io/fallout-skill-shot-timer/

## What it does

- For each phase it looks at all four light changes (right on/off, left on/off) and picks the best cue. It shows the launch window and how much room you have on each side.
- Everything is adjustable: ball travel time, your reaction time, and each phase's right on/off durations. You can also set the gaps when both lights are off. Settings are saved in your browser.
- Practice mode blinks both inlane lights at the phase's real rhythm. Press **Launch** (or Space) and it tells you whether the ball would have hit the right inlane while it was lit, and how early or late you were.

## Default timings

| Phase | Right on | Right off | Left on | Best cue |
|---|---|---|---|---|
| 1 | 2.04 s | 2.17 s | 2.17 s | 0.89 s after the right light goes OFF |
| 2 | 0.92 s | 1.22 s | 1.22 s | The moment the right light comes ON |
| 3 | 1.06 s | 3.13 s | 2.03 s (est.) | The moment the left light comes ON |

The right-light timings were read from video frame timestamps. In phases 1–2 the left light is on exactly while the right is off. In phase 3 both lights stay off for a while after the right goes off. That 1.1 s gap is an estimate, chosen to match the observation that shooting when the left light comes on works best. Ball travel defaults to 2.3 s (phone stopwatch) and reaction time to 0.22 s.

## Hosting

The whole site is one static `index.html` with no build step. It's served by GitHub Pages from the `main` branch.

# Balloon Analog Risk Task

A single-file web app (`index.html`) for the optimization unit of MA 130 (Revisiting Calculus). It is a modified version of the standard Balloon Analog Risk Task (BART), shortened so it can be played quickly in front of a class.

## How it differs from the standard BART
- Balloons pop within 10 pumps, not 100. After *k* successful pumps, the next pump pops the balloon with probability **1/(10 − k)**.
- Each successful pump earns **$10**. You can collect at any time to bank that balloon's money. A popped balloon earns $0.
- The game is played in two rounds of 10 balloons each. By default, both rounds use the same balloons.
- After each round, an optional analysis panel shows the expected-value curve E(n) = 10·n·(10 − n)/10.

Keyboard: Space = pump / next balloon, Enter = collect.

Created with Claude.

## Settings
Use the Settings button or URL parameters, for example:
`index.html?N=10&v=10&b1=10&b2=10&seed=1234`

| Parameter | Meaning |
|---|---|
| `N` | Maximum number of pumps |
| `v` | Dollars per pump |
| `b1`, `b2` | Number of balloons in Round 1 and Round 2 |
| `seed` | Fixes which balloons appear, so a run can be repeated |
| `odds` | 0 or 1: show the pop chance |
| `reveal` | 0 or 1: show where a collected balloon would have popped |
| `reuse` | 0 or 1: Round 2 starts with Round 1's balloons |
| `auto` | 0 or 1: offer auto-pump in Round 2 |



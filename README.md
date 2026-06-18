# ⛵ Calendario

A deeply interactive calendar you **sail** rather than read.

A wobbly, hand-inked sailboat — drawn in the _Peanuts_ / Charlie Brown spirit,
with every outline **"boiling"** (jittering a few times a second, the way Bill
Melendez animated the TV specials) — crosses an ocean of days. The weather of
that ocean — calm sunny water vs. grey storm swells — adapts to **your sleep and
stress**. It's a calendar built on Scott
Barry Kaufman's _Transcend_ metaphor: life isn't a mountain of needs you climb,
it's a **sailboat** you keep adjusting on an open sea. The **hull** is your
security (safety, connection, rest); the **sail** is your growth (exploration,
love, creation).

It still does the plain job of a calendar: shows the days, marks today (⚓), and
lets you log what happened.

## Try it

Open `index.html` in any browser. No build step, no dependencies.

Or serve it:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## How it works

- **The Helm** (top right): two sliders — _slept poorly ↔ well_ and _calm ↔
  stressed_. They steer the sea in real time. Poor sleep / high stress → choppy
  grey swells, headwind, rain, a pitching ship. Good rest / low stress → glassy
  golden water and a steady sail.
- **The day ribbon** (bottom): the month as a strip of waypoints. Click any day
  to log it. Today carries the anchor (⚓). Logged days show a tiny weather icon
  and dots: 🟢 growth, 🔴 security.
- **The Sailboat panel** (right): the cumulative voyage. Logging _growth_ moments
  opens the sail; logging _security_ moments steadies the hull.

Everything is saved to your browser's `localStorage` — private, no server.

## Roadmap

- **Real sleep/stress sync.** Today the inputs are manual sliders. A static page
  can't reach Oura / Apple Health / Fitbit directly (those need OAuth + a
  backend). The weather engine reads a single normalized `condition()` value, so
  a real tracker integration can plug straight in behind it.
- Richer claymation animation (kneading/squash on the hull, gulls, islands as
  events on the horizon).
- Multi-month "open sea" horizontal scroll between legs of the voyage.

## Why these graphics & this psychology

- **Peanuts / Charlie Brown** look: flat vintage color on warm cel-paper,
  hand-lettered headings, zigzag-stripe motifs, and the signature **boiling
  line** — outlines that jitter between micro-offset versions a few times a
  second, exactly how the specials were animated.
- **Scott Barry Kaufman, _Transcend_ (2020)**: the sailboat model of
  self-actualization — security as the hull, growth as the sail.

---

_Boiling-line seas & the psychology of becoming._

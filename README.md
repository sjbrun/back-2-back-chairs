# Back-to-Back Chairs

A tiny browser game made for a 3-year-old. Drag chairs around a room and spin
them into place — when two chairs end up truly back-to-back, they burst into
a firework and disappear. Clear every chair to set off a confetti celebration.

No build step, no dependencies — just a single `index.html` file.

## Play it

Open [`index.html`](index.html) in any browser (double-click the file, or
serve the folder with any static file server).

## Controls

- **Drag a chair's seat** to move it around the room.
- **Drag the little knob** on the back of the chair to rotate it.
- Get two chairs' backs touching and facing each other — they'll explode
  into fireworks and vanish.
- A few decorative objects (plant, picture, box) sit in the room too; they
  just wiggle when tapped and don't count toward clearing the room.
- Clear all the chairs to trigger the celebration screen, then hit
  **Play Again** to reset.

## Tuning

A few constants near the top of the `<script>` in `index.html` control
difficulty:

- `CHAIR_COUNT` — number of chairs (must stay even).
- `TOUCH_DIST` — how close chair centers must be to count as touching.
- `ANGLE_TOL` / `DOT_TOL` — how forgiving the back-to-back angle check is.

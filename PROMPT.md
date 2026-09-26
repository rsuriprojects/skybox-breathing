# Prompt: "Skybox" — a box breathing app

Build a single-page box breathing web app (one `index.html`, no build step) that feels
calm, airy, and beautiful — like looking up at an open sky.

## Core
- Four phases: **Breathe in → Hold → Breathe out → Hold**.
- A **square in the center** with a glowing dot that travels around its edges — one side per
  phase — leaving a light trail so you can see where you are in the cycle.
- Inside the square, a soft "breath" shape that **expands on inhale, rests on hold, shrinks on exhale**.
- Big phase label + seconds countdown in the middle.

## Adjustable timing
- A slider per phase (2–12 s), plus a **"link all sides"** toggle so one slider moves all four.
- Presets: **Gentle 3·3·3·3**, **Classic 4·4·4·4**, **Deep 5·5·5·5**, **Unwind 4·4·6·2**.
- Session length: 1 / 3 / 5 / 10 minutes or open-ended. Always ends on a complete cycle.
- Timing changes apply live, even mid-session.

## Look & feel
- **Sky themes:** Day (blue sky), Dawn, Dusk, Night (with twinkling stars).
  Soft gradient backgrounds with slowly drifting blurred clouds.
- Frosted-glass control panel.
- **Fonts: never Arial.** Use *Fraunces* (soft serif) for headings and numbers, and
  *Manrope* for UI text.
- Smooth animation (requestAnimationFrame, time-accurate, no drift).

## Extras
- Optional soft chime at each phase change (Web Audio, no files) and phone vibration.
- Keyboard: **Space** = start/pause, **Esc** = stop.
- **Focus mode:** controls fade out while breathing; the square and sky stay.
- Cycle counter + session progress bar; a gentle "well done" summary at the end.
- Remembers your settings (localStorage, with a fallback if it isn't available).
- Respects `prefers-reduced-motion`; works on phone screens.

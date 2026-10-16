# Jessica Vega · Window to Lanterns

Personal site for Jessica Vega (Senior Software Engineer / AI Engineer / Product).

A single self-contained page (`index.html`). Behind the content, a scroll-driven Three.js scene
looks out of a cabin window at dusk over a Cascades lake: a raymarched landscape (terrain, forest,
a lakeside hamlet, a softened volcanic peak, lake reflections) rendered as a full-screen shader,
with paper sky lanterns rising from the hamlet as you scroll.

- Three.js r128 is loaded from cdnjs; everything else is inline and procedural (no image assets).
- Render quality adapts to the device; the scene renders on demand and falls back to a CSS
  gradient when WebGL is unavailable.
- Accessibility: skip link, landmarks, readable panels over every frame, keyboard focus states,
  a Pause motion button, and `prefers-reduced-motion` support (ambient motion stops; the
  scroll story remains).
- Diagnostics: open the page with `#perf` for a frame-time / lantern readout, or `#perfnd`
  to also turn off depth testing on the lanterns.

To view locally, open `index.html` in a browser (it needs network access for Three.js and fonts).

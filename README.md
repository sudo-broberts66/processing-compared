# Two Ways to Process

A full-screen, interactive 3D tabletop for high school students. It follows one sentence from a teacher through two models standing side by side, a cutaway human head and an AI agent machine, in six matched stages:

1. Take it in
2. Pay attention
3. Hold it
4. Connect it
5. Save it
6. Bring it back

The five details in the sentence travel through both models as labelled blocks. Four switches cause forgetting (a phone buzz, no review or sleep, a flooded context window, a session that ends without notes); lost details drop into a "Forgotten" tray, and at stage 6 each model answers from whatever is left.

## Use it

Open `index.html` in any modern browser. There is no build step.

- A short welcome card opens first; press **Start**. The **i** button brings it back, along with notes on where the comparison breaks down.
- **Next / Back**, the numbered step buttons, or the left and right arrow keys change step. Both models move together, and the camera reframes for each step.
- **Drag** to look around, **scroll or pinch** to zoom, **shift-drag** (or two fingers) to pan. The target button at top right recentres.
- **Tap a part** or its label for a short definition.
- The switches under each model, or the matching objects on the table (phone, alarm clock, paper stack, strapped notebook), turn forgetting on and off. Flipping one never changes the step: an amber dot marks the step where it will take effect, and if you are already past that step the view updates in place.
- On a phone held upright, the view shows one model at a time; use the two tabs to swap.

## Files

- `index.html`: the whole page.
- `vendor/three.min.js`: Three.js r128 (MIT, see `vendor/three.LICENSE`). The page loads it from cdnjs first and falls back to this copy, so it also works with no internet.

Fonts load from Google Fonts when online and fall back to system fonts offline. If a device cannot provide 3D graphics, the page shows the six stages as text instead.

The earlier flat, scrolling version is in the git history.

To host it, enable GitHub Pages for this repository and serve from the root.

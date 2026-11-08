# Dense terrain editor responsiveness — issue #780

Actual production Godot Metal captures with five local human profiles. No generative media.

- `before-editor.png`: main baseline, one accepted river added to 12 legal river/fissure lines.
- `after-editor.png`: same accepted layout on the candidate; geometry is preserved.
- `mixed-terrain.png`: 24 initial lines plus accepted river, fissure, dune and pit edits.
- `five-player-race.png`: normal garage-to-race handoff retains all 26 authored lines and five cars; simulation advances beyond countdown.
- `comparison.gif`: baseline left, candidate right, input aligned. The candidate holds its clean completed view while baseline continues. Fixed-timestep MovieCapture; visual comparison, never ordinary FPS or a wall-clock benchmark. This 1280×360,10fps,64-color preview has less text, color and motion fidelity than the retained 2560×720,30fps MP4.

Measured uncontended hidden native runs: editor entry 36.980→6.965 seconds; accepted river replacement view 50.783→6.115 seconds. JSON and full validation inventory live in the private implementation PR. Windows/NVIDIA, physical controllers and live Steam remain unverified. Extreme construction is not instantaneous and this does not claim universally hitch-free rendering.

Each exact PNG and final animation sample was individually inspected before publication. Links are pinned to the media commit to preserve existing references.

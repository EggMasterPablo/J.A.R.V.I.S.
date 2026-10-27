# J.A.R.V.I.S. Zero API Edition (v0.3)

A self-contained browser-based JARVIS-style HUD. No API key, server, package install, or paid AI provider is required.

## Run it

1. Open `index.html` in a modern browser.
2. For the best headset/WebXR chances, host the file on an HTTPS static host. It still works as a normal local page for most features.
3. Press **MIC** and allow microphone access if your browser supports speech recognition, or type commands in the console.

## Commands

- `help`
- `what time is it` / `what is today's date`
- `system status`
- `calculate 24 times 7`
- `set a timer for 2 minutes` / `cancel timer`
- `start stopwatch` / `pause stopwatch` / `reset stopwatch`
- `remember buy milk` / `read notes` / `clear notes`
- `add task finish homework` / `list tasks` / `complete task 1`
- `tell me a joke` / `random fact`
- `open Google`, `open YouTube`, `open Wikipedia`, `open Maps`
- `search web for ...`
- `change theme to amber`, `change theme to violet`, `change theme to cyan`
- `toggle grid`, `voice off`, `voice on`, `fullscreen`

Notes and tasks are saved in the browser's local storage and stay on that device/browser unless its site data is cleared. Use **Export Notes** to save a JSON copy.

## Important limitations

- This version intentionally has no generative AI API. It uses a local command engine and a small built-in fact/joke set, so it cannot freely answer arbitrary questions like a full AI model.
- Speech recognition support varies by browser. The Web Speech API is not universally supported, and some browsers send recognition audio to their own online service. Text-to-speech uses the browser/device voice system.
- WebXR support depends on the headset and browser. The XR button checks support and requests an immersive-AR session; it does not yet place a complete world-anchored 3D HUD in the room.
- This is a prototype, not a native headset app and not a full movie-style JARVIS.

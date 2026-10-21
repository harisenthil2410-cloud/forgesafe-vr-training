# ForgeSafe VR — Industrial Workforce Training

A browser-based 3D factory safety training demo built with HTML, CSS, JavaScript, and Three.js.

## Features
- Interactive 3D factory scene
- Four hazards: oil spill, loose electrical cable, missing PPE, unstable boxes
- Clickable hazard markers and checklist
- Safety instructions and action guidance
- Four-question quiz with immediate feedback
- Progress indicator and score
- Keyboard movement (WASD / arrow keys) and mouse-drag camera look

## Run locally
1. Extract the ZIP.
2. Open `index.html` in a modern browser with internet access.
3. If the browser blocks JavaScript modules when opening a local file, use a local static server:
   - Install Python 3 if needed.
   - Open a terminal in this folder.
   - Run `python -m http.server 8000`
   - Visit `http://localhost:8000`

Three.js is loaded from jsDelivr, so internet access is required.

## Deploy to GitHub Pages
1. Sign in to GitHub and create a new public repository, e.g. `forgesafe-vr-training`.
2. Upload `index.html` to the repository root (the top level, not inside another folder).
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose branch **main** and folder **/(root)**, then click **Save**.
6. Wait for GitHub Pages to finish publishing. The public address will look like:
   `https://YOUR-USERNAME.github.io/forgesafe-vr-training/`
7. Open the address in a private/incognito window or another device to test public access.

## Testing checklist
- Click Enter training floor.
- Select each hazard from the list and from the 3D markers.
- Click Identify hazard, then Safety action.
- Move with WASD and rotate the view by dragging on the scene.
- Open Safety quiz, answer all four questions, and confirm the result appears.
- Use Reset session and repeat.

## Notes
- This is an educational prototype, not certified safety instruction.
- Scores are held in the current page session and are not sent to a server or shared between devices.
- Three.js is loaded from a public CDN; the first load requires internet access.
- WebXR headset mode is not implemented in this first version; this is a browser-based 3D simulation, not a claim of full headset VR.

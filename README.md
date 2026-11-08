# Pinth

Control a 3D particle cloud with your hand, using your webcam. Runs entirely in the browser.

**Live demo:** https://pinth.vercel.app

## Controls

- 🖐 **Move your hand** to move the particles
- ✊ **Close your fist** to collapse them, 🖐 **open your hand** to expand
- 👌 **Pinch** to switch shape

## How it works

[MediaPipe Tasks Vision](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker) tracks your hand landmarks from the webcam, and [three.js](https://threejs.org) renders the particles. Video is processed on your device and isn't uploaded anywhere.

## Run it locally

It's a single `index.html` with no build step. The browser needs a secure context for webcam access, so serve it over localhost rather than opening the file directly:

```bash
git clone https://github.com/Saad5643/pinth.git
cd pinth
npx serve .
```

Open the URL it prints and allow camera access.

## Contributing

Ideas for new shapes and gestures are welcome. Open an issue or send a pull request.

## Licence

[MIT](LICENSE)

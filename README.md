# Basket Ball — Sun Temple

A lightweight browser extension that adds a fun, arcade-style "Basket Ball" game themed around the Sun Temple. Playable directly within the browser extension popup or as an in-page overlay (depending on the extension settings).

## About the game

Basket Ball — Sun Temple is a casual, arcade game where the player shoots baskets while avoiding obstacles and collecting power-ups. The Sun Temple theme gives the game a bright, colorful aesthetic with golds and deep oranges, and the soundtrack (if included) evokes an adventurous, upbeat atmosphere.

Features:
- Simple, pick-up-and-play gameplay
- Score tracking
- Power-ups and obstacles for increasing challenge
- Lightweight and optimized for browser extensions

## Clone the repository

To get a local copy of the project, run:

```bash
git clone https://github.com/mildannerofc/Basket-Ball-SunTemple.git
cd Basket-Ball-SunTemple
```

## Install as a Chrome (or Chromium-based) extension (Developer / unpacked)

1. Open Chrome or any Chromium-based browser (e.g., Microsoft Edge, Brave, Vivaldi).
2. Go to chrome://extensions/ (or use the browser menu > Extensions).
3. Enable "Developer mode" (toggle in the top-right).
4. Click "Load unpacked" and select the folder containing this repository (the folder that has the extension's `manifest.json`).
5. The extension should appear in your extensions list and its icon will be visible in the toolbar.
6. Click the icon to open the popup and start the game.

Notes:
- If the extension uses external resources or a build step (e.g., bundling or compiling assets), run the build step before loading the unpacked extension. Common build commands:

```bash
# If the project uses npm/yarn
npm install
npm run build
# or
yarn install
yarn build
```

- After building, point "Load unpacked" to the build or `dist` directory (if the repo has one).

## Install on Firefox (temporary loading)

Firefox uses a different process for temporary extension loading during development:

1. Open Firefox and navigate to about:debugging#/runtime/this-firefox.
2. Click "Load Temporary Add-on...".
3. In the file picker, select the extension's `manifest.json` file from the repository folder (or the packed `.xpi` if you have one).
4. The extension will be loaded temporarily; it will disappear when Firefox is restarted unless packaged and installed permanently.

For publishing to Firefox Add-ons, see Mozilla's developer documentation: https://extensionworkshop.com/

## Install on Microsoft Edge (Chromium-based)

Microsoft Edge follows the Chromium extension workflow:
1. Open edge://extensions/
2. Enable "Developer mode" (toggle bottom-left).
3. Click "Load unpacked" and choose the folder containing `manifest.json`.

## Building a distributable (.zip or .crx/.xpi)

- For Chrome Web Store publishing, you typically zip the extension files (the directory contents) and upload to the Developer Dashboard.
- For Firefox, package as an .xpi for distribution in addons.mozilla.org (AMO).

Refer to the Chrome and Firefox developer docs for packaging rules and required metadata.

## Usage

- Click the extension icon in the browser toolbar to open the game popup.
- Use the on-screen controls or keyboard (if supported) to shoot baskets and collect points.
- Check the repository's code or docs for configuration options (sound, difficulty, control mappings).

## Development notes

If you plan to modify the extension:
1. Follow the clone and build steps above.
2. Keep the manifest version updated and test changes by reloading the unpacked extension.
3. Use the browser console (popup devtools or extension background/service worker logs) to debug runtime issues.

## Contributing

Contributions are welcome. Please open an issue with a clear description of the bug or feature request, and submit a pull request with your changes.

## License

Specify the project license here (e.g., MIT). If no license is provided, add one or confirm which license you want.

---

If you want, I can:
- Customize this README with screenshots, badges, or specific build commands found in the repository.
- Add packaging and publishing instructions tailored to exact manifest version (v2 or v3) used in this repo.
- Create a CHANGELOG or CONTRIBUTING guide.

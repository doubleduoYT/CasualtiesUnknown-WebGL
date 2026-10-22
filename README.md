# Casualties Unknown Mobile — WebGL

Browser build version `7.0.1-mobile-v12.4.2`.

**Play:** https://doubleduoyt.github.io/CasualtiesUnknown-WebGL/ (available after the first Pages deployment completes).

The first load downloads about 394 MiB. A desktop browser with WebGL and a stable connection is recommended. Device compatibility and memory limits vary. Native UDP/LAN multiplayer is disabled in the WebGL build.

## Build and deployment

The verified Unity HTML5 build is distributed as `CasualtiesUnknown-WebGL-release.zip` in release `v12.4.2-webgl`. It contains the launch page, Unity loader, data, WebAssembly, symbols, template resources, and StreamingAssets. The Unity editor project is not included.

GitHub Actions downloads the archive, verifies its SHA-256, and deploys its contents to GitHub Pages, serving all runtime resources from one origin. Deployment runs when the workflow is updated on `main` or when **Deploy WebGL** is started manually from Actions.

SHA-256: `1ef0271e7f6aba39c7d72536f47de8b7e1d97c34e8b16315b4732d520fd6abbb`

For local execution, extract the archive and serve it over HTTP, for example `python -m http.server 8000 --bind 127.0.0.1`, then visit http://127.0.0.1:8000/.

# Casualties Unknown Mobile — WebGL

Browser build version `7.0.1-mobile-v12.4.2`.

**Deployment pending:** release archive upload and GitHub Pages activation are not complete yet.

Planned play URL: https://doubleduoYT.github.io/CasualtiesUnknown-WebGL/

The first load downloads approximately 394 MiB. A desktop browser with WebGL and a stable connection is recommended. Device compatibility and memory limits vary. Native UDP/LAN multiplayer is disabled in the WebGL build.

## Build and deployment

The verified Unity HTML5 build is packaged as `CasualtiesUnknown-WebGL-release.zip`. Upload it to release tag `v12.4.2-webgl`. It contains the launch page, Unity loader, data, WebAssembly, symbols, template resources, and StreamingAssets. The Unity editor project is not included.

Set Settings → Pages → Source to GitHub Actions. Publishing the release triggers `.github/workflows/pages.yml`; it can also be run manually. The workflow downloads the archive, verifies SHA-256, and deploys its contents to GitHub Pages, serving all runtime resources from the same origin.

SHA-256: `1ef0271e7f6aba39c7d72536f47de8b7e1d97c34e8b16315b4732d520fd6abbb`

For local execution, extract the archive and serve it over HTTP, for example `python -m http.server 8000 --bind 127.0.0.1`, then visit http://127.0.0.1:8000/.

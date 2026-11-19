# SkyAlert Weather

A responsive weather app using the free Open-Meteo geocoding and forecast APIs. No API key is required.

## Run the website

1. Extract the ZIP file.
2. Open the `weather` folder.
3. For basic testing, open `index.html` in a modern browser. Weather search requires an internet connection.
4. For PWA installation and offline app-shell caching, serve the folder from `localhost` or HTTPS. For example, if Python is installed, open a terminal in this folder and run:

   ```bash
   python -m http.server 8000
   ```

   Then visit `http://localhost:8000` in Chrome or Edge.

## Install as a desktop app

1. Open the hosted HTTPS website or the localhost address above in Chrome or Microsoft Edge.
2. Use the **Install app** button in the header when it appears, or choose the browser's **Install SkyAlert** / **Apps → Install this site as an app** option.
3. SkyAlert then opens in its own desktop window and can be pinned to the taskbar or dock.

The PWA caches the interface files so the app shell can open offline. Live weather and city search still require internet access. PWA installation is supported by modern Chromium browsers; opening the HTML directly with `file://` does not enable installation.

## Features

- Search worldwide cities, with quick city suggestions
- Current temperature, feels-like temperature, humidity, wind and precipitation
- Five-day high/low forecast
- Dark + Cyan (default), Dark and Light themes; theme choice is saved
- Responsive mobile/tablet/desktop layout
- Request cancellation to prevent stale search results
- Installable PWA and cached app shell

## Project files

- `index.html` — accessible page structure
- `style.css` — responsive design system and themes
- `script.js` — API requests, rendering, theme and install interactions
- `manifest.webmanifest` — desktop/PWA metadata
- `service-worker.js` — app-shell caching
- `icons/` — install icons

Weather data: [Open-Meteo](https://open-meteo.com/).

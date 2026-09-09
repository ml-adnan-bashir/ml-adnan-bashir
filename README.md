# Adnan Bashir — Interactive Portfolio

Open **index.html** for the personal website and **projects.html** for all eight selected projects. The dark, peach, and muted-blue palette is retained from the first version.

## What changed

- The signal responds to the pointer within a bounded radius. Clicking or tapping sends a ripple through nearby lines.
- Scrolling transforms the broad hero wave into two persistent fields along the page edges. Interaction remains local and subtle in the side fields.
- Motion can be paused from the header. Reduced-motion preferences start the field paused; the ripple button is also available to keyboard users when motion is enabled.
- More detail in the biography, research entries, and current teaching sections.
- A separate eight-project collection, with four featured on the homepage. Each project opens in a new tab so the portfolio stays available.

## Upload to GitHub Pages

Upload the **contents** of this ZIP to your repository, keeping the folder structure:

- index.html
- projects.html
- portfolio.css
- signal.js
- projects-data.json
- apps/ (all eight subfolders)
- .nojekyll

The README is optional for hosting. Upload extracted files, not the ZIP itself. Keep a copy or Git commit of your previous homepage before replacing index.html and projects.html. The portfolio uses portfolio.css, so your existing styles.css and unrelated project pages can stay in place.

For your main personal site, use the repository **ml-adnan-bashir.github.io**. In repository Settings → Pages, select **Deploy from a branch**, **main**, and **/ (root)**. The site address will be https://ml-adnan-bashir.github.io/ when GitHub completes deployment. The files also support project sites in a subdirectory: all internal links are relative. No backend, package installation, build step, or API key is required for the portfolio.

## Selected projects

| Project | Source from your archive | Main purpose |
|---|---|---|
| RAFTAR | speedtest.html | Download/upload speed and latency |
| ZARB | zarb.html | Tap-tempo BPM, history, and averages |
| Boundary & State Lab | bns.html | Time-series boundaries, states, and feature evidence |
| NET Practice Simulator | net_latest.html | Timed practice, grading, saved progress, and review |
| Urdu Word Cloud | death.html | Urdu typography, palettes, and animated layout |
| Enterprise Workspace | ERM.html | Tasks, planning, roles, and approvals |
| Cantt Events | ce.html | Hall bookings, a simulated fleet, and reports |
| Tilt Scale | scale.html | A calibrated phone-orientation experiment |

Only one assessment app is included. net_latest.html was selected for its complete grading and review workflow, five difficulty levels, resume support, and exports. The separate benchmark/checker versions and overlapping SegStream feature-selection page were not included.

## Project requirements

The portfolio and signal use no external libraries. Individual apps retain these requirements:

- RAFTAR transfers test data to/from Cloudflare speed-test endpoints. It requires internet and consumes data during tests. Failed measurements now show an error/retry state rather than a completed zero-speed result. The missing optional portrait uses the app's original inline avatar.
- ZARB measures the tempo of your taps, not audio files. The missing optional background-image pack has been omitted; the gauge themes and other settings remain.
- The SegStream lab embeds its dataset, analysis results, equations, and fonts. It needs a modern browser supporting DecompressionStream. It is the largest bundled app, around 16 MB uncompressed. Its source-package download is disabled by its existing offline initialization.
- The NET simulator loads KaTeX 0.16.10 from jsDelivr for math rendering.
- The Urdu word cloud embeds its Urdu fonts.
- Enterprise Workspace uses browser-local demonstration records. It has no backend or live enterprise connection.
- Cantt Events uses demonstration fleet data and browser-local bookings. It loads Leaflet 1.9.4, Chart.js 4.4.0, and jsPDF 2.5.1 from public CDNs, plus map tiles and optional fonts/photos.
- Tilt Scale is a physical-computing experiment, requiring a compatible phone, sensor permission, a balance setup, and a known calibration weight. Open it over HTTPS on GitHub Pages for sensor access.
- Several apps optionally load Google Fonts; system font fallbacks remain available.

## Editing

Biography, research, and course text: index.html.
Project cards: projects.html and the featured cards in index.html.
Colors and layout: portfolio.css.
Signal motion and interaction: signal.js.
The projects-data.json file is an editable inventory; pages are pre-rendered HTML and do not fetch it at runtime. If you change the inventory, update the corresponding HTML cards too.

The research descriptions do not claim publication status or benchmark results. Course themes are introductory summaries, not official syllabi. Add verified publication, CV, contact, and course-material links when ready.

## Validation

Section links, local portfolio assets, selected app entrypoints, and JavaScript parsing were checked. The signal received a simulated-event smoke check for pointer/ripple changes, scroll positioning, pause, and reduced-motion behavior. No live network speed test, device sensor measurement, or browser visual test was performed.

Original signal artwork and portfolio design, with appreciation for https://openai.com/index/gpt-6-astra/ . Independent personal website; no OpenAI affiliation or endorsement.

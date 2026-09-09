# Adnan Bashir — Portfolio + Website Builder

## Start here

**Open index-builder.html to edit your website.** It is a standalone file: no server, installation, account, or API key is needed. The builder starts with your current portfolio and its original color palette.

Open **index.html** to view the website, or **projects.html** to view the eight-project collection.

## Change colors and content

1. In **Colors**, choose one of eight palettes or adjust individual colors. Both signal colors, text, accents, the main background, and the teaching panel are editable.
2. In **Content**, edit your name, introduction, biography, research, courses, project-page introduction, and footer. Headings support line breaks; list fields use one item per line.
3. In **Projects**, edit project titles, descriptions, notes, and links. Choose whether to include each project and whether to feature it on the homepage. Move projects up or down, or add and remove cards.
4. Use the homepage/projects and desktop/tablet/mobile selectors above the live preview. Scroll and move the pointer inside the preview to interact with the signal. External app links open from the exported website.

**Original ember** always restores the original colors. The **Original website** entry in Versions restores the original content and colors together.

## Save now, edit later

- Your draft saves automatically in the current browser.
- **Save version** creates a named snapshot. Enter an optional name in the Versions tab, or use the automatic name. Up to 20 snapshots are retained; the original design is always available separately.
- Restoring a version or opening a design saves the current draft into Versions first.
- **Export → Editable design · JSON** downloads a portable backup of the current content, colors, and project settings.
- Later, open index-builder.html and click **Open design** to choose your JSON file. You can also open an index.html or projects.html previously exported by this builder: both contain the complete editable design.
- Browser storage belongs to that browser and can be cleared. Keep a downloaded JSON copy when you want to preserve a design across computers or browser resets.
- If browser storage is blocked or full, the editor reports it and leaves your current work available for download. If a restore-point save fails, the earlier stored draft is preserved; subsequent edits are labeled session-only until a save succeeds. Incomplete drafts can be saved and restored, while website exports require valid project links.

The included **portfolio-design.json** is a backup of the current starting design. Open design supports this builder's design format and its exported HTML pages; it is not an importer for arbitrary websites.

## Publish changes on GitHub Pages

For your first upload, extract this complete ZIP and upload its contents to the repository. Keep the **apps/** folder structure.

For later edits, choose **Export → Website pages ZIP** in the builder. It downloads:

- index.html — your updated homepage
- projects.html — your matching project collection
- portfolio-design.json — editable design backup
- .nojekyll
- READ-ME.txt

Replace the two HTML pages in your existing repository, and **keep your existing apps/ folder**. The builder's update ZIP contains the website pages and settings; it does not repackage the app files. Those eight apps are included in this complete portfolio package. When you add a new project card, upload its app or point the card at an existing external URL.

The exported homepage and projects page contain their own CSS and interactive signal code. They do not need a separate stylesheet or signal.js. Updating a palette in the builder keeps both pages consistent when you export them together. The editor does not change the styling inside the eight independent apps.

Keep index-builder.html and your design JSON wherever you prefer to edit; neither is required for the public website. Your previous unrelated styles.css and other project pages can stay in the repository.

For the main personal site, use **ml-adnan-bashir.github.io**. In repository Settings → Pages, select **Deploy from a branch**, **main**, and **/ (root)**. The address will be https://ml-adnan-bashir.github.io/ when GitHub finishes deployment. All internal project links are relative, so subdirectory project sites are also supported.

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

## Validation

Checked standalone HTML and JSON export/reopen round trips, including Urdu, quotes, angle brackets, and literal script-closing text. Checked independent version snapshots, history limits, storage-failure handling, invalid import rejection, URL validation, all eight palettes, selected-project counts, local links, and inline JavaScript parsing. No browser visual test, live network speed test, or phone-sensor measurement was performed.

The signal retains pointer bending, click/tap ripples, scroll-to-side fields, a pause control, and reduced-motion support. The homepage and projects collection use the same saved palette.

Research descriptions do not claim publication status or benchmark results. Course themes are introductory summaries, not official syllabi.

Original portfolio and signal design, with appreciation for https://openai.com/index/gpt-6-astra/ . Independent personal website; no OpenAI affiliation or endorsement.

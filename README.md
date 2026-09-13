# William Steinley - Portfolio site

Source for https://woodsy-will.github.io/, a portfolio and resume for GIS forester and forestry GIS analyst roles: one main page plus an interactive Leaflet map.

## What is on the main page

- **Header**: Gold Run, California; "GIS Forester / Forestry GIS Analyst · M.S. Forestry"; links to the resume PDF, the projects section, GitHub and email.
- **Projects**: two cards, each written as problem, data, method, result and limits.
  - *Mohawk Valley West Slope: LiDAR-based harvest-unit planning* - a demonstration on public data: LiDAR terrain and canopy products, 24 demonstration units, a skyline corridor screen, an 11x17 unit map series and simulated-cruise review sheets. A hero image and five thumbnails link to full-size JPEGs; a button opens the interactive map; the source and deliverables are at [plumas-lidar-harvest-planning](https://github.com/woodsy-will/plumas-lidar-harvest-planning) and its release.
  - *Forest Inventory Analyzer* - a Rust command-line and web cruise compiler, at [forest-inventory-analyzer-rust](https://github.com/woodsy-will/forest-inventory-analyzer-rust) with a Windows installer and macOS and Linux binaries on its v0.2.0 release.
- **About**: three paragraphs on National Forest project work, LiDAR and inventory experience, and what the two projects are.
- **Professional Resume**: experience, education, certifications and qualifications, and research, with a PDF download.
- **Technical Skills**: forestry and field operations, GIS and spatial science, programming and data.
- **Get In Touch**: email and GitHub.

## Files

| Path | Purpose |
|---|---|
| `index.html` | The main page. No templates, no build step. |
| `styles.css` | Design tokens, light and dark themes, responsive layout, print styles. |
| `projects/resume/William_Steinley_Resume.pdf` | Two-page resume served by the site (no phone number). |
| `projects/plumas-lidar-harvest-planning/*.jpg` | Six gallery previews rendered by the project's own scripts, plus `*_thumb.jpg` copies for the strip. |
| `projects/plumas-lidar-harvest-planning/map/index.html` | Interactive Leaflet map on USGS basemaps: units, corridors, landings, exclusion zones, streams, contours, yarding class and simulated plots. |
| `projects/plumas-lidar-harvest-planning/map/data/` | GeoJSON layers in WGS84 exported from the project GeoPackage, and the yarding-class PNG overlay with its bounds. |
| `robots.txt`, `sitemap.xml` | Crawl directives and the sitemap for the main page, the map page and the resume PDF. |

## Working on it

- Plain HTML, CSS and one Leaflet script, so any static preview works. A headless browser screenshot is enough to check layout:
  `msedge --headless=new --screenshot=out.png --window-size=1280,2400 index.html`
- The map page fetches GeoJSON, which browsers block from `file://`. Serve the repo root with `python -m http.server` to test it locally.
- Keep the main page free of inline styles; every class is defined in `styles.css`.
- The resume PDF is exported from the resume document, then copied here. The gallery JPEGs are copied from the project repository's `output/previews` folder after each render, so the site never holds an image the project cannot reproduce.
- Every project shown is built from public data with the author's own code. No employer or client material is used.

## License

Page text and layout: all rights reserved. Gallery images and map data are CC BY 4.0 under the project repository's `LICENSE-MAPS-DATA.md`.

## Hosting

GitHub Pages from the `main` branch root. A push to `main` rebuilds the site within a minute.

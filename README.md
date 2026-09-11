# William Steinley - Portfolio site

Source for https://woodsy-will.github.io/, a single-page portfolio and resume for forestry GIS analyst roles.

## What is on the page

- **Header**: Gold Run, California; Forester, GIS Analyst, M.S. Forestry; links to the resume PDF, the projects section and GitHub.
- **About**: two short paragraphs on National Forest project work, LiDAR and inventory experience, and availability.
- **Professional Resume**: experience, education, certifications and qualifications, and research, with a PDF download.
- **GIS Projects**: two cards.
  - *Mohawk Valley West Slope: LiDAR-based harvest-unit planning* - a self-directed rebuild on public data of harvest-planning workflows: LiDAR terrain and canopy products, harvest-unit layout, cable-yarding feasibility, an 11x17 unit map series and field-data review sheets. Six preview images link to the full-size JPEGs; the source and deliverables are at [plumas-lidar-harvest-planning](https://github.com/woodsy-will/plumas-lidar-harvest-planning) and its v1.0 release.
  - *Forest Inventory Analyzer* - a Rust command-line and web tool for cruise data, at [forest-inventory-analyzer-rust](https://github.com/woodsy-will/forest-inventory-analyzer-rust) with installers on its v0.2.0 release.
- **Technical Skills**: forestry and field operations, GIS and spatial science, programming and data.
- **Get In Touch**: email and GitHub.

## Files

| Path | Purpose |
|---|---|
| `index.html` | The whole page. No templates, no build step. |
| `styles.css` | Design tokens, light and dark themes, responsive layout, print styles. |
| `projects/resume/William_Steinley_Resume.pdf` | Two-page resume served by the site (no phone number). |
| `projects/plumas-lidar-harvest-planning/*.jpg` | Six gallery previews rendered by the project's own scripts. |
| `robots.txt`, `sitemap.xml` | Crawl directives and the sitemap for the page and the resume PDF. |

## Working on it

- Plain HTML and CSS, so any static preview works. A headless browser screenshot is enough to check layout:
  `msedge --headless=new --screenshot=out.png --window-size=1280,2400 index.html`
- Keep the page free of inline styles; every class is defined in `styles.css`.
- The resume PDF is exported from the resume document, then copied here. The gallery JPEGs are copied from the project repository's `output/previews` folder after each render, so the site never holds an image the project cannot reproduce.
- Every project shown is built from public data with the author's own code. No employer or client material is used.

## Hosting

GitHub Pages from the `main` branch root. A push to `main` rebuilds the site within a minute.

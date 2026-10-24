# GISDS project instructions

Read README.md and GISDS.md before changing the current catalogue. Cartography_Database_Sources.md is the preserved original catalogue; leave it unchanged unless the user explicitly requests otherwise.

- GISDS is an independent catalogue repository within Ecological Information and a reference for any user. Use audience-neutral language, including “Example use”; avoid assuming a student or instructor context.
- Keep GISDS.md limited to one continuous Markdown source table with seven columns: ID, Resource, Information available, Coverage, Accessibility, Example use, Reuse / limitations. Do not insert blank lines between source rows, including the final row.
- Keep README.md as the concise Overview; retain detailed usage guidance, dataset metadata conventions, interpretation notes, provenance, review dates and historical versions in RESEARCH_NOTES.md. Keep maintenance instructions in AGENTS.md.
- Preserve existing source IDs, research content, academic attribution and provenance. Extend an existing provider entry when adding its viewer or product links; do not duplicate it.
- Distinguish platforms from datasets, analytical data from rendered imagery, and observations from classifications, models and inference.
- Verify provider documentation before changing current capabilities, access requirements or reuse conditions; record review dates and uncertainties in README.md.
- Keep dataset-specific resolution, dates, CRS, processing and licence metadata explicit in separate dataset records; record the field conventions in README.md.
- Use stable filenames and record catalogue version information in README.md and revisions in Git.
- Check that all source rows have seven cells, IDs are unique, and all rows form a single table before saving.
- Do not duplicate other projects' authoritative inventories or implement database integrations without a scoped request.
- Do not select a licence or publish further changes without user authorisation.

## Overview diagram maintenance

- Keep the editable labels, relationships, palette and fixed layout in `assets/diagrams/gisds_overview.mmd`; regenerate with `python3 assets/diagrams/render_gisds_overview.py`. The renderer supports this diagram's Mermaid subset only and requires no third-party packages.
- Maintain source and SVG together. Regenerate twice and compare output bytes; retain SVG title, description, viewBox, source checksum and README alternative text/full-size link. Never edit SVG labels independently.
- Treat the illustration as a documented overview, not a new classification, implemented service or claim of scientific validation. Preserve all records, codes and original documentation.
- Use repository-relative asset paths. Pinned-source website publication must separately approve, allowlist and checksum the SVG; do not run the renderer during website builds or advance publication pins as part of diagram maintenance.

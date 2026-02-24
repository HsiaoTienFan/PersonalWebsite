# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static personal portfolio website for Daniel Fan (Data Scientist, Engineer, Martial Artist, Magician). Hosted on GitHub Pages at https://hsiaotienfan.github.io/PersonalWebsite/.

## Architecture

- **Single-page static site** using Bootstrap 3 with jQuery
- **Entry point**: `index.html` - contains all page sections (Home, About, Skills, Experience, Work, Contact)
- **Styles**: SASS compiled to `css/layout.min.css` - source files in `sass/` directory
- **JavaScript**: Custom layout logic in `js/layout.js` (handles scroll effects, navigation, carousel, popups)
- **Vendor libraries**: jQuery, Bootstrap 3, WOW.js (animations), Masonry (grid layout), Parallax

## SASS Structure

Main stylesheet: `sass/layout.scss` imports:
- `_mixins.scss`, `_variables.scss` - shared utilities
- `base/` - base styles
- `components/` - buttons, progress bars, social icons
- `gui/` - promo block, service cards, work/portfolio items
- `layout/` - header, footer
- `plugins/` - back-to-top, Bootstrap component overrides
- `utils/` - colors, helpers

## Development

No build tools configured. Edit files directly:
- HTML changes: `index.html`
- Style changes: Edit SASS files, compile to CSS manually
- Minified files (`.min.js`, `.min.css`) need manual regeneration after edits

## Deployment

- GitHub Pages serves from `master` branch
- Custom domain configured via `CNAME` file

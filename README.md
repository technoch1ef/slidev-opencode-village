# OpenCode Village — Slide Deck

A [Slidev](https://sli.dev/) presentation on orchestrating AI agents for software development using the OpenCode Village workflow.

## Prerequisites

- Node.js (v18+)

## Install

```bash
npm install
```

## Usage

### Development (live reload)

```bash
npm run dev
```

Opens the slide deck in your browser with hot-reload on edits to `slides.md`.

### Build static site

```bash
npm run build
```

Outputs a deployable SPA to `dist/`.

### Export to PDF

```bash
npm run export
```

Requires Playwright Chromium (installed as a dev dependency).

## Project Structure

```
slides.md       # Main slide content (edit this)
style.css       # Custom styles
vite.config.ts  # Vite configuration
public/         # Static assets (images, etc.)
lib/            # Custom components/utilities
```

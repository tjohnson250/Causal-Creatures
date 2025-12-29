# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Quarto blog focused on causal inference methodology, statistical thinking, and related topics in R. The blog is titled "Causality and Other Curious Creatures" and is authored by Todd R. Johnson, a professor of Biomedical Informatics.

## Architecture

**Quarto Website Structure:**
- `_quarto.yml`: Main configuration file defining the website structure, theme (cosmo), and navigation
- `index.qmd`: Homepage with a listing of all blog posts sorted by date (descending)
- `about.qmd`: Author bio and profile page using the Jolla template
- `posts/`: Directory containing individual blog posts, organized by date (format: YYYY-MM-DD-post-name/)
- `styles.css`: Custom CSS for the site
- `_site/`: Generated output directory (not tracked in git)
- `_freeze/`: Quarto's computation cache directory

**Post Structure:**
Each blog post lives in its own directory under `posts/` with an `index.qmd` file containing:
- YAML frontmatter with: title, author, date, categories, description, draft status
- Markdown content with R code chunks as needed

## Common Commands

**Preview the site locally:**
```bash
quarto preview
```

**Render the entire site:**
```bash
quarto render
```

**Render a specific post:**
```bash
quarto render posts/YYYY-MM-DD-post-name/index.qmd
```

**Publish to GitHub Pages (if configured):**
```bash
quarto publish gh-pages
```

## Key Configuration Details

- **Theme**: Cosmo (from _quarto.yml:19)
- **Code display**: Code folding disabled, code tools enabled (from _quarto.yml:22-23)
- **Post listing**: Configured for chronological display with categories, no UI filters (from index.qmd:3-9)
- **Navigation**: About page and social links (GitHub, Twitter) in navbar (from _quarto.yml:7-13)

## Content Focus

The blog explores causal inference, statistical methodology, teaching, academia, and occasionally political topics. Posts include prose, visualizations, and code examples, with an emphasis on step-by-step explanations and simulations.

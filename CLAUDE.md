# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based personal blog hosted on GitHub Pages at www.netcat.blog. The blog focuses on cats and computer networks, with technical posts about networking topics (SDN, B4, etc.).

## Architecture

**Jekyll Static Site with Minima Theme:**
- Uses the `minima` theme (specified in `_config.yml`)
- Standard Jekyll directory structure with `_posts/` for blog content
- Blog posts follow Jekyll naming convention: `_posts/YYYY-MM-DD-title.md`
- Posts use YAML frontmatter with `title:` and `date:` fields

**Content Organization:**
- `index.md` - Homepage with cat ASCII art and welcome message
- `_posts/` - Blog posts about networking and project ideas
- `images/` - Image assets referenced in posts
- `CNAME` - Custom domain configuration (www.netcat.blog)

**Frontmatter Format:**
All posts must include:
```yaml
---
title: "Post Title"
date: YYYY-MM-DD
---
```

## GitHub Pages Deployment

This repository is configured for automatic GitHub Pages deployment:
- Pages is enabled in repository settings
- Builds from the `main` branch
- Custom domain: www.netcat.blog (configured via CNAME file)
- Changes pushed to main branch automatically trigger a rebuild

GitHub Pages automatically builds and deploys the site - no manual build steps required.

## Local Development

**Testing locally (if needed):**
```bash
bundle install
bundle exec jekyll serve
```
Site will be available at http://127.0.0.1:4000

Note: This repository appears to be from a GitHub Skills course template. The README.md contains tutorial instructions rather than project documentation.

## Content Guidelines

**Blog Post Creation:**
1. Create new file in `_posts/` directory
2. Name it `YYYY-MM-DD-title.md` (hyphens between words in title)
3. Add frontmatter with title and date
4. Write content in Markdown
5. Commit to main branch to publish

**Image References:**
- Store images in `images/` directory
- Reference in posts using relative paths: `![alt](../images/filename.png)`

## Theme

Uses Jekyll's `minima` theme which provides default styling and layout. The theme can be customized but currently uses defaults.

## Coding Style

**Comments:**
- Use comments sparingly
- Only add comments when logic isn't self-evident
- Prefer clear, self-documenting code over explanatory comments

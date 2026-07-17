# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.0] - 2026-07-17

Initial release of **Slidev Theme Squircle** — a presentation theme built around large rounded (squircle) content frames on a solid brand background.

### Added

#### Design

- Squircle frame system — white content cards with large border radius on a solid brand-colored background
- Five switchable color palettes via `themeConfig.color`:
  - `teal` (default) — deep emerald
  - `cobalt` — deep cobalt blue
  - `rose` — warm terracotta / coral
  - `indigo` — muted creative violet
  - `charcoal` — formal cool gray
- Semantic `--color-primary-*` tokens shared across layouts and components
- Vertical accent bar on framed `<Label>` / `frame-header` headings (blockquote and cards use the same bar style)
- Cover / closing top labels render as white pill badges
- Soft inset panel utility (`.soft-panel`) for secondary content blocks
- CSS custom property system for spacing, typography, radius, and color scales

#### Layouts

- **Title & structure:** `cover`, `closing`, `title`, `title-center`, `title-sandwich`, `intro`, `section`, `section-frame`, `section-index`, `section-index-center`, `section-subtitle`, `toc`, `agenda`
- **Content:** `panel`, `frame-panel`, `quote`, `profile` (with optional `heading`, `::name::`, `::aside::`), `cols`, `cards`, `table`, `comparison`
- **Data & metrics:** `stats`, `timeline`, `steps-layout`, `process-flow`
- **Team:** `team`, `team-border`
- **Image:** `image-left`, `image-right`, `image-full`

#### Components

- `<Label>` — corner / header label with accent bar; positions include `top-center`
- `<Note>` — muted corner annotation
- `<PageNumber>` — current page number (optional `showTotal`)
- `<Underline>` — primary-colored underline emphasis
- `<Highlight>` — marker stroke; `variant`: `primary` (default), `blue` (alias), `amber`
- `<Badge>` — inline pill label; `variant`: `solid`, `soft`, `outline`
- `<Icon>` — Lucide icon via `lucide-static`
- `<Divider>` — horizontal rule; `variant` and `spacing` props
- `<QA>` — question-and-answer pair
- `<NoteBlock>` — framed note; `type`: `info`, `warn`, `alert`
- `<FactRow>` — label–value metadata row
- `<Kbd>` — keyboard key UI with optional Lucide icon

#### Typography & tooling

- Default font: [Gen Interface JP](https://gen.typesetting.jp/); switchable to Inter + Noto Sans JP via `themeConfig.font`
- Ellipsis glyph routing via `themeConfig.ellipsisFont` (`cjk` | `latin`)
- CJK opening punctuation alignment for block and line starts
- Task list checkbox styles with rounded corners
- Rounded table corners on the `table` layout
- Example deck (`example.md`) as a theme preview
- Cloudflare Workers deploy support (`wrangler.jsonc`)
- Prettier configuration and GitHub Actions npm publish workflow
- GitHub issue and pull request templates

[Unreleased]: https://github.com/minagishl/slidev-theme-squircle/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/minagishl/slidev-theme-squircle/releases/tag/v0.1.0

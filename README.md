# sofast

A classic, personal-web theme for [padat](https://github.com/racktrace/padat).
Serif text, terracotta links, light and dark mode from the OS. CSS only, zero JavaScript.

## Requirements

- A site built from padat v1.0.1 or newer. sofast only styles padat's HTML through its theme contract; it ships no templates.

## Install

Put sofast next to your site and point Hugo to it:

    # hugo.toml of your site
    theme = 'sofast'
    themesDir = '..'

Or place it inside your site at `themes/sofast` and use only `theme = 'sofast'`.

padat loads `assets/css/theme.css` automatically after its own `base.css`.

## What it styles

- Header with site title left and menu right; active page underlined (no layout shift)
- Article meta, tags, related pages, newer/older navigation
- Code blocks with a language label strip and a calm five-tone syntax palette
- Callouts with a colored edge per type
- Tables framed with horizontal rules, still scrollable on small screens
- Table of contents as a collapsible box
- Block images framed and centered at natural size
- YouTube thumbnails cropped to 16:9 with a play button
- Footer with joined search control and copyright
- Sticky footer on short pages

## Customize

All colors and the corner radius are CSS variables at the top of `theme.css`
(`--bg`, `--fg`, `--muted`, `--link`, `--visited`, `--rule`, `--code-bg`, `--radius`, `--syn-*`),
each with a light and a dark value.

## Weight

About 8.4 KB of CSS on top of padat. A padat home page with sofast is about 11 KB in total.

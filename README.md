# Drupal 25th Anniversary Timeline

A Hugo-powered timeline celebrating 25 years of Drupal innovation and community achievements.

## Features

- Interactive timeline design inspired by modern anniversary pages
- Drupal-themed color scheme and branding
- Responsive design for mobile and desktop
- Timeline events sourced from JSON data
- Evolution of Druplicon graphics theme
- Priority-based event highlighting

## Setup

1. **Install Hugo**:
   ```bash
   # macOS
   brew install hugo
   
   # Or download from https://github.com/gohugoio/hugo/releases
   ```

2. **Add Druplicon Images**:
   Place these images in `static/images/`:
   - `druplicon-2001.png` - Original Druplicon
   - `druplicon-2009.png` - Refined design  
   - `druplicon-2016.png` - Modern design
   - `druplicon-2024.png` - Current design
   
   Get official assets from: https://www.drupal.org/about/media-kit/logos

3. **Build and Serve**:
   ```bash
   cd drupal25-timeline
   hugo server -D
   ```
   
   Visit: http://localhost:1313

## Data Source

Timeline events are automatically pulled from:
https://raw.githubusercontent.com/weitzman/drupal-timeline/refs/heads/main/drupal-timeline.json

Note: The JSON file was renamed to `drupal_timeline.json` (with underscores) for Hugo compatibility.

## Customization

- Modify colors in `static/css/timeline.css` (CSS variables at top)
- Update timeline layout in `layouts/_default/timeline.html`
- Adjust content in `content/_index.md`

## Build for Production

```bash
hugo --minify
```

The built site will be in the `public/` directory.
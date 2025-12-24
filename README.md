# Drupal 25th Anniversary Timeline

A Hugo-powered timeline celebrating 25 years of Drupal innovation and community achievements. Timeline events sourced from JSON data. See https://weitzman.github.io/drupal25-timeline/


## Setup

1. **Install Hugo**:
   ```bash
   # macOS
   brew install hugo
   
   # Or download from https://github.com/gohugoio/hugo/releases
   ```


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

## Build for Production

```bash
hugo --minify
```

The built site will be in the `public/` directory.

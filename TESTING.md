# Testing the Solution Pattern Locally

## Quick Start

1. **Install dependencies**:
   ```bash
   cd solution-pattern-app-connect-ai
   npm install
   ```

2. **Build the site**:
   ```bash
   npm run build
   ```

3. **View the output**:
   ```bash
   open gh-pages/index.html
   # Or on Linux:
   # xdg-open gh-pages/index.html
   ```

## Development Mode

For live preview during development:

```bash
npm run dev
```

Then open `gh-pages/index.html` in your browser and refresh after changes.

## What Gets Generated

The build process creates:
- `gh-pages/` directory with the complete static site
- `gh-pages/solution-pattern-app-connect-ai/index.html` - main entry point
- All pages, assets, and navigation

## Troubleshooting

**Error: "Cannot find module '@antora/cli'"**
- Run `npm install` first

**Error: "start_page not found"**
- Check `documentation/antora.yml` has correct component name
- Verify `site.yml` references the correct start page

**Navigation not showing**
- Check `documentation/modules/ROOT/nav.adoc` exists
- Verify all xref links match actual section anchors

**Images not loading**
- Ensure images are in `documentation/modules/ROOT/assets/images/`
- Check `:imagesdir:` is set in .adoc files

## File Structure

```
solution-pattern-app-connect-ai/
├── site.yml              # Production build config
├── dev-site.yml          # Development build config
├── package.json          # Node dependencies
├── lib/                  # Antora extensions
│   ├── tab-block.js
│   └── remote-include-processor.js
├── supplemental-ui/      # UI customizations
└── documentation/
    ├── antora.yml        # Component config
    └── modules/ROOT/
        ├── nav.adoc
        ├── pages/
        └── assets/images/
```

## Next Steps

After verifying the build works:
1. Review content for technical accuracy
2. Add any missing diagrams
3. Update YouTube video link in 03-demo.adoc
4. Test all cross-reference links
5. Push to GitHub for GitHub Pages deployment

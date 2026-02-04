# AGENTS.md - Guidelines for AI Coding Agents

This is a Jekyll-based personal website using GitHub Pages and the Minimal Mistakes theme.

## Build Commands

### Serve the site locally
```bash
bundle exec jekyll serve
```
Site will be available at http://127.0.0.1:4000

### Build for production
```bash
bundle exec jekyll build
```
Output goes to `_site/` directory.

### Install dependencies
```bash
bundle install
```

### Clean build artifacts
```bash
bundle exec jekyll clean
```

## Project Structure

- `_config.yml` - Main Jekyll configuration
- `_data/` - YAML data files (navigation, projects, jobs, certifications, apps)
- `_pages/` - Page content (about, portfolio, resume, etc.)
- `_posts/` - Blog posts (if any)
- `assets/` - CSS, images, JavaScript
- `_site/` - Generated static site (do not edit)

## Code Style Guidelines

### YAML Data Files (`_data/*.yml`)
- Use double quotes for all strings
- Maintain consistent ordering across files
- Use clear, descriptive keys
- No trailing commas
- Alphabetical sorting within sections where appropriate

### Markdown Files (`_pages/`, `_posts/`)
- Use front matter with `layout: page` or `layout: post`
- Use standard markdown syntax
- Keep line width reasonable (80-100 characters)
- Use ATX-style headings (`## Heading`)

### Configuration (`_config.yml`)
- Follow alphabetical order within sections
- Use consistent indentation (2 spaces)
- Comment out unused settings rather than removing
- Keep site settings separate from build settings

### GitHub Pages Constraints
- Use only plugins supported by GitHub Pages
- No custom Ruby code in `_plugins/`
- Build time is limited; keep site lean
- Use `remote_theme` instead of `theme` for Minimal Mistakes

## Naming Conventions

- **Pages**: kebab-case (`about-me.md`, `portfolio.md`)
- **Posts**: `YYYY-MM-DD-title.md` format
- **Branches**: feature/descriptive-name (for any development)
- **Commits**: imperative mood, descriptive summary

## Error Handling

- Check `bundle exec jekyll build` for build errors
- Verify YAML syntax with `bundle exec jekyll doctor`
- Port 4000 must be free to serve locally
- Ensure all plugins are in Gemfile before adding to `_config.yml`

## Adding New Content

### Add a new page
1. Create file in `_pages/` with front matter
2. Add to navigation in `_data/navigation.yml` if needed
3. Test locally before committing

### Add to projects/jobs/etc
1. Edit corresponding file in `_data/`
2. Follow existing structure and ordering
3. Use consistent date formats

### Modify configuration
1. Edit `_config.yml`
2. Restart jekyll serve for changes to take effect
3. Test build with `bundle exec jekyll build`

## Common Issues

- **Port in use**: Kill process on port 4000 with `lsof -ti:4000 | xargs kill`
- **Bundle install fails**: Ensure Ruby version compatibility
- **Theme not loading**: Verify `remote_theme` version in config
- **Pagination errors**: Ensure index.html exists for pagination template

## Notes

- This is a static site - no runtime dependencies
- Changes to `Gemfile` require `bundle install`
- The `.devcontainer/` directory configures VS Code dev container
- No tests exist for this static site project

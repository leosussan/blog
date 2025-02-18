# [leosussan.com](https//leosussan.com)

Personal blog and website built with Hugo, using the m10c theme. This site is automatically deployed to GitHub Pages.

## Prerequisites

- Hugo Extended v0.143.1
- Go v1.24.0

## Local Development

1. Install `asdf`. See [installation instructions](https://asdf-vm.com/#/core-manage-asdf-vm?id=install-asdf-vm).
2. Install the required versions of Hugo and Go.
```bash
# Adds plugins from .tool-versions file 
cut -d' ' -f1 .tool-versions | xargs -n 1 asdf plugin add
asdf install
```
3. Start the Hugo development server:
```bash
hugo server -D
```

The site will be available at `http://localhost:1313/`

## Project Structure

- `content/` - Contains all the site content
  - `about.md` - About page
  - Posts will be added to the `content/` directory
- `static/` - Static assets
- `hugo.toml` - Site configuration
- `.github/workflows/hugo.yml` - GitHub Actions workflow for automated deployment

## Deployment

The site is automatically deployed to GitHub Pages when new release is published.

The deployment process is handled by GitHub Actions using the workflow defined in `.github/workflows/hugo.yml`.

## Theme

This site uses the [m10c theme](https://github.com/vaga/hugo-theme-m10c) with custom configuration.
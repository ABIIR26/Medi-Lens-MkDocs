# GitHub Pages Deployment


We use **GitHub Actions** to automate the deployment of this documentation.

### Workflow Configuration
The `.github/workflows/docs.yml` file handles:
1. **Environment Setup:** Installing Python and MkDocs dependencies.
2. **Build:** Compiling Markdown into a static site via `mkdocs build`.
3. **Deploy:** Pushing the `site/` folder to the `gh-pages` branch.

### Manual Build
```bash
pip install mkdocs-material mkdocs-minify-plugin
mkdocs build


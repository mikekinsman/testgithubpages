# GitHub Pages Configuration Demo

A comprehensive demonstration repository showcasing various GitHub Pages configuration options and their impacts.

## 🎯 Purpose

This repository serves as a practical guide to understanding and implementing different GitHub Pages configurations. It demonstrates:

- Different deployment sources (root, /docs, gh-pages branch, GitHub Actions)
- Jekyll configuration options
- Custom domain setup
- Theme configuration
- URL and permalink structures
- Static vs dynamic content deployment

## 📚 Contents

### Main Demo Page
- **[index.html](index.html)** - Comprehensive overview of all GitHub Pages configuration options
- Live examples and code snippets
- Best practices and common scenarios

### Documentation Examples (in /docs folder)
- **[docs/index.html](docs/index.html)** - Demonstrates deployment from /docs folder
- **[docs/jekyll-example.html](docs/jekyll-example.html)** - Jekyll configuration guide
- **[docs/custom-domain.html](docs/custom-domain.html)** - Custom domain setup instructions

### Configuration Files
- **[_config.yml](_config.yml)** - Jekyll configuration with detailed comments
- Demonstrates theme selection, plugins, permalinks, and more

## 🚀 Deployment Options Demonstrated

### 1. Root Directory Deployment
Deploy directly from the repository root (main branch `/`)
- Best for: Simple sites, landing pages
- Configuration: Settings → Pages → main → / (root)

### 2. /docs Folder Deployment
Deploy from the `/docs` folder (main branch `/docs`)
- Best for: Projects with code + documentation
- Configuration: Settings → Pages → main → /docs
- **This repository uses this method**

### 3. gh-pages Branch
Deploy from a dedicated gh-pages branch
- Best for: Separating deployment from development
- Configuration: Settings → Pages → gh-pages → / (root)

### 4. GitHub Actions
Custom build and deployment workflow
- Best for: Complex builds (React, Vue, custom generators)
- Configuration: Settings → Pages → GitHub Actions

## 🎨 Jekyll Features Demonstrated

The `_config.yml` file shows how to configure:
- Site metadata (title, description, author)
- Theme selection
- URL and baseurl settings
- Plugins (SEO, feed, sitemap)
- Permalink structures
- Collections and defaults
- Exclusions and inclusions

## 🌐 Custom Domain Configuration

The repository includes comprehensive documentation on:
- Apex domain setup (example.com)
- Subdomain setup (www.example.com)
- DNS record configuration
- HTTPS/SSL setup
- Troubleshooting common issues

## 📖 How to Use This Repository

### View the Live Demo
Once GitHub Pages is enabled for this repository, visit:
- Main demo: `https://username.github.io/testgithubpages/`
- Docs demo: `https://username.github.io/testgithubpages/docs/`

### Explore the Code
1. Browse the HTML files to see different styling and content approaches
2. Check `_config.yml` for Jekyll configuration examples
3. Look at the directory structure for organizational patterns

### Try It Yourself
1. Fork this repository
2. Enable GitHub Pages in Settings → Pages
3. Choose a deployment source (root, /docs, or gh-pages)
4. Experiment with different configurations
5. View your site at `https://yourusername.github.io/testgithubpages/`

## 🛠️ Local Development

To test Jekyll locally:

```bash
# Install dependencies
gem install bundler jekyll

# Create Gemfile (if not exists)
bundle init
bundle add github-pages

# Install gems
bundle install

# Serve locally
bundle exec jekyll serve

# View at http://localhost:4000
```

## 📋 Configuration Examples Included

- ✅ Multiple deployment sources
- ✅ Jekyll configuration with themes
- ✅ Custom domain setup
- ✅ Permalink structures
- ✅ Plugin configuration
- ✅ Front matter examples
- ✅ Responsive design patterns
- ✅ Navigation between pages
- ✅ Code syntax highlighting examples

## 🔗 Useful Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Supported Jekyll Themes](https://pages.github.com/themes/)
- [Custom Domain Configuration](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## 📝 License

MIT License - See [LICENSE](LICENSE) file for details

## 👤 Author

Mike Kinsman

---

**Note**: This is a demonstration repository. The configurations and examples are meant for educational purposes to help understand GitHub Pages capabilities.

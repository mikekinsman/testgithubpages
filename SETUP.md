# How to Enable GitHub Pages for This Repository

This guide will help you enable GitHub Pages and view the demonstration site.

## Quick Start

1. **Go to Repository Settings**
   - Navigate to your repository on GitHub
   - Click on "Settings" tab
   - Scroll down to "Pages" in the left sidebar

2. **Configure GitHub Pages Source**
   
   You have several options to demonstrate:

   ### Option A: Deploy from /docs (Recommended for this demo)
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/docs**
   - Click **Save**
   
   This will serve:
   - Main site: `https://yourusername.github.io/testgithubpages/docs/`

   ### Option B: Deploy from root
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
   - Click **Save**
   
   This will serve:
   - Main site: `https://yourusername.github.io/testgithubpages/`

   ### Option C: Deploy with GitHub Actions
   - Source: **GitHub Actions**
   - The workflow in `.github/workflows/deploy-pages.yml` will run automatically

3. **Wait for Deployment**
   - GitHub Pages will build and deploy your site (usually takes 1-2 minutes)
   - You'll see a green checkmark when deployment is complete
   - The site URL will be displayed at the top of the Pages settings

4. **Visit Your Site**
   - Click on the URL shown in Settings → Pages
   - Or navigate to: `https://yourusername.github.io/testgithubpages/`

## What to Explore

Once your site is live, explore these pages:

- **Main Demo**: Comprehensive overview of all configuration options
- **Docs Example**: Demonstration of /docs folder deployment
- **Jekyll Example**: Guide to Jekyll configuration
- **Custom Domain**: Instructions for custom domain setup

## Testing Different Configurations

To try different deployment options:

1. **Switch between root and /docs**:
   - Go to Settings → Pages
   - Change the Folder from / to /docs (or vice versa)
   - Save and wait for redeployment

2. **Try GitHub Actions**:
   - Change Source to "GitHub Actions"
   - Push a commit to trigger the workflow
   - Check the Actions tab to see the deployment progress

3. **Test a custom domain**:
   - Follow the instructions in `docs/custom-domain.html`
   - Add a CNAME file with your domain
   - Configure DNS records at your domain provider

## Troubleshooting

### Site not showing up
- Wait 2-3 minutes after configuration
- Check the Actions tab for any failed workflows
- Ensure the source branch and folder contain an `index.html` file

### 404 errors
- Verify the correct folder is selected in settings
- Check that file paths in HTML are correct
- Custom 404 page should show if a page doesn't exist

### Changes not appearing
- GitHub Pages may cache for a few minutes
- Try clearing browser cache or use incognito mode
- Check that changes are committed and pushed to the correct branch

## Local Testing

To test the site locally before deploying:

```bash
# For Jekyll sites
bundle install
bundle exec jekyll serve

# Visit http://localhost:4000
```

For plain HTML:
```bash
# Use any local server, e.g.:
python -m http.server 8000
# or
npx http-server

# Visit http://localhost:8000
```

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll on GitHub Pages](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)
- [Custom Domains](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## Support

If you encounter issues:
1. Check the repository's Actions tab for deployment logs
2. Review the GitHub Pages documentation
3. Ensure your repository is public (or you have GitHub Pro for private repos)
4. Verify that GitHub Pages is enabled for your account/organization

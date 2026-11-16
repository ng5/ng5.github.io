# Ng5 Solutions Ltd

A Hugo company website for IT consulting in financial services, with Home, Services, About, and Contact pages. No JavaScript or external dependencies.

## Preview

Run `/usr/bin/hugo server` and open http://localhost:1313.

## Build

Run `/usr/bin/hugo --minify` and deploy the generated `public/` directory.

## Edit

- `hugo.toml`: company details, base URL, and public contact email. Until an email is set, the Contact page says contact details are coming soon.
- `content/`: Services, About, and Contact text.
- `layouts/home.html`: home page content.
- `layouts/baseof.html`: shared navigation and footer.
- `static/style.css`: responsive styling.

Service descriptions are starter copy; review them against the company's actual offering before publishing. No qualifications, clients, or regulatory status are claimed.

## GitHub Pages deployment

This repository includes `.github/workflows/pages.yml`. Every push to `main` builds the site with Hugo 0.170.0 and deploys `public/` as a Pages artifact. Generated files stay out of Git.

One-time setup:

1. Push this repository to GitHub.
2. Open **Settings → Pages → Build and deployment** and select **GitHub Actions** as the source.
3. Set **Custom domain** to `ng5solutions.co.uk` in Pages settings, and configure your DNS using GitHub's instructions. A custom domain must be configured in Pages settings; `baseURL` alone does not configure hosting.
4. Open **Actions → Build and deploy Hugo to GitHub Pages → Run workflow** to deploy the current `main` branch if needed.
5. Enable **Enforce HTTPS** when GitHub makes it available.

The workflow uses the Pages URL supplied by GitHub, including the configured custom domain or repository subpath. Subsequent pushes to `main` deploy automatically. No second repository or generated-code branch is needed.

References: https://gohugo.io/host-and-deploy/deploy-to-github-pages/ and https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

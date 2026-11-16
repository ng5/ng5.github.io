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

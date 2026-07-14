# Elastic Alerting Resources

A GitHub Pages site hosting publicly available web pages, diagrams, and
references related to Elastic alerting.

**Live site:** https://elastic.github.io/alerting/

## Adding new resources

1. Create your HTML (or HTML + JS) page anywhere in this repository, e.g.
   `diagrams/my-diagram.html` or `guides/my-guide.html`.
2. Add a link to the new page in `index.html` so visitors can discover it.
3. Open a pull request — once merged to `main` the
   [GitHub Pages workflow](.github/workflows/deploy-pages.yml) publishes the
   site automatically.

## Repository layout

```
.
├── index.html          # Landing page — lists all available resources
├── .nojekyll           # Disables Jekyll so raw HTML/JS is served as-is
├── .github/
│   └── workflows/
│       └── deploy-pages.yml  # Deploys the site to GitHub Pages on every push to main
└── README.md
```

## Local preview

Open `index.html` directly in a browser, or use any static file server:

```bash
npx serve .
# then visit http://localhost:3000
```

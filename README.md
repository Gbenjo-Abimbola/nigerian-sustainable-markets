# Nigerian Sustainable Markets Initiative — website

Static site for GitHub Pages. No build step, no dependencies.

## Files

| File | Purpose |
|---|---|
| `index.html` | Homepage: hero performance chart, headline results, research themes |
| `research.html` | Publications list (working paper, quarterly note, forthcoming) |
| `esg-20-index.html` | The index: results, attribution, limitations, roadmap |
| `methodology.html` | Universe, selection, weighting, rebalancing, robustness, limits |
| `about.html` | Positioning, independence statement, research lead |
| `contact.html` | Contact routes and what people can request |
| `assets/style.css` | All styling for every page |
| `papers/` | Drop the white paper PDF here |
| `.nojekyll` | Stops GitHub Pages running Jekyll over the files |

## Deploying

1. Copy these files into the root of the repository (`nigerian-sustainable-markets`).
2. Add the white paper as `papers/ngx-esg-20-executive-edition.pdf`.
3. Commit and push to `main`.
4. Repo → Settings → Pages → Source: *Deploy from a branch*, Branch: `main`, folder `/ (root)`.
5. Live at `https://<username>.github.io/nigerian-sustainable-markets/`.

## Custom domain

Add a file named `CNAME` in the repo root containing one line, e.g.
`nigeriansustainablemarkets.org`, then point a CNAME record at
`<username>.github.io` in your registrar's DNS. Enable "Enforce HTTPS" in
Settings → Pages once the certificate is issued.

## Things to change before launch

- Chart on the homepage is hand-plotted from the paper's year-end values. Replace
  the `<polyline points="...">` values with the real monthly series when you have it.
- LinkedIn links point to `https://www.linkedin.com/` — swap in the real page.
- Email addresses assume `@nigeriansustainablemarkets.org`. Change if the domain differs.
- Sector counts on `esg-20-index.html` are placeholders consistent with 9 banking names.
  Replace with the actual breakdown, or publish the full constituent list.

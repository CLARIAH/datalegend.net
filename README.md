# datalegend.net

Website of dataLegend: Linked Data tooling and research for economic, social and demographic history within [CLARIAH](https://www.clariah.nl). Built with [Quarto](https://quarto.org) and published on GitHub Pages.

## Editing

Every page is a Markdown file (`*.qmd`). Edit one on GitHub (the "Edit this page" link on each page goes there) or locally, then open a pull request. Merging to `main` publishes the site automatically.

| File | Page |
|------|------|
| `index.qmd` | Home |
| `tools.qmd` | Tools |
| `research.qmd` | Research / case studies |
| `publications.qmd` | Publications |
| `presentations.qmd` | Presentations |
| `teaching.qmd` | Teaching |
| `team.qmd` | Team |
| `contact.qmd` | Contact |

Images live in `images/`. Styling is in `styles/`, and navigation in `_quarto.yml`. Search for `TODO` to find content that still needs checking.

## Local preview

```bash
quarto preview
```

## First-time setup on GitHub

1. Push this repository to GitHub.
2. Run the publish workflow once (Actions → Publish site). It creates the `gh-pages` branch.
3. In Settings → Pages, set the source to "Deploy from a branch", branch `gh-pages`, folder `/`.
4. In Settings → Pages → Custom domain, enter `datalegend.net` and enable "Enforce HTTPS" once the certificate is issued.

## DNS (for whoever manages datalegend.net)

Point the apex domain to GitHub Pages:

```
datalegend.net.      A     185.199.108.153
datalegend.net.      A     185.199.109.153
datalegend.net.      A     185.199.110.153
datalegend.net.      A     185.199.111.153
www.datalegend.net.  CNAME clariah.github.io.
```

Keep the existing `druid.datalegend.net` and `cattle.datalegend.net` records as they are.

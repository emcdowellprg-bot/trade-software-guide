# Best Software for Trades

Independent guides to software for small service businesses: HVAC, plumbing, lawn care, cleaning, dog grooming, pressure washing, and similar trades. The site is a Jekyll project that GitHub Pages builds from the repository. There is no separate build step and no JavaScript framework.

There are no affiliate links yet. Links in the guides go to vendors' own pages.

## Layout

| Path | What it is |
| --- | --- |
| `_config.yml` | Site title, the GitHub Pages URL, and the plugins (SEO tag and sitemap). |
| `_layouts/` | Header, footer, home page, and guide page. |
| `assets/css/site.css` | The only stylesheet. |
| `index.md` | Home page. Explains the site and lists every published guide. |
| `about.md` | Independence, how tools are evaluated, affiliate disclosure. |
| `guides/*.md` | One guide per file. Front matter: `title`, `description`, `trade`, `last_updated`. |
| `docs/page-template.md` | The outline for a new guide. Not published. |
| `robots.txt` | Points crawlers at the generated sitemap. |

`jekyll-sitemap` writes `/sitemap.xml` when GitHub Pages builds the site. `jekyll-seo-tag` writes the title and meta description from each page's front matter.

A guide shows up on the home page when its front matter includes `trade`. Set `last_updated` to the date the page, and the prices on it, were checked (`YYYY-MM-DD`).

The published URL for the first guide is:

`/guides/jobber-vs-housecall-pro-small-hvac/`

On the default GitHub Pages project site that is:

`https://emcdowellprg-bot.github.io/trade-software-guide/guides/jobber-vs-housecall-pro-small-hvac/`

`_config.yml` sets `baseurl` to `/trade-software-guide` so links and CSS work at that address. For a custom domain, or for a user site served at the domain root, set `baseurl` to `""` and set `url` to the full origin (`https://example.com`).

## Add a guide

1. Copy `docs/page-template.md` to `guides/your-slug.md`.
2. Replace the instructions with the guide. Keep the front matter fields.
3. Follow the section order in the template: intent, who it's for, quick answer, comparison table, per-tool notes, pricing with a checked-on date and a source link, what to watch out for, FAQ, sources. Mark anything you could not confirm.
4. Commit to `main`. The home page picks the new file up because `trade` is set. No other edit is required.

## Enable GitHub Pages

Do this in the GitHub website. Nothing in this repository turns Pages on by itself.

1. Open the repository on GitHub.
2. Go to **Settings**, then **Pages** (under "Code and automation").
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Set **Branch** to `main` and the folder to `/ (root)`.
5. Save.

GitHub builds the site with Jekyll. The first build can take a few minutes. When it finishes, the Pages settings show the URL, which for this repository is `https://emcdowellprg-bot.github.io/trade-software-guide/`.

The plugins in `_config.yml` are on GitHub's supported list. You do not install them, and you do not run a build, for the live site.

## Optional local preview

Ruby and Bundler are only for previewing on your own machine.

```bash
bundle install
bundle exec jekyll serve
```

Open the local URL Jekyll prints. The `Gemfile` pins the `github-pages` gem so the preview matches GitHub's Jekyll. GitHub's branch deploy does not use the Gemfile.

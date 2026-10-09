# sasingh07.github.io

A static Jekyll portfolio intended for GitHub Pages. All website source is at the **repository root**; no build output needs to be committed.

## Before publishing

1. Update the résumé-based text in `index.md`, `about.md`, and `experience.md` as your background changes. Markdown pages have YAML front matter between the `---` lines; keep that block in place.
2. Edit `_config.yml`: set `title` and `description` to your real preferred wording and put a public email address in `email` if desired. A mailto link exposes the address publicly and requires the visitor to have an email app configured. Leave `email: ""` to keep the placeholder and omit the link.
3. Edit `_data/navigation.yml` for menu labels or paths; edit `_includes/header.html` and `_includes/footer.html` for shared chrome; edit `assets/css/style.css` for the theme.
4. If your GitHub username changes, update `url` and `github_username`. Your displayed name is set in `author.name` and in the Home page heading. Update `linkedin_url` to change the LinkedIn link. For a user site the GitHub repository must be named `sasingh07.github.io` under the `sasingh07` account.

Uploaded source documents in `attached_assets/` are excluded from the Jekyll output and ignored by Git so the full résumé and phone number are not published as website assets.

## Publish using GitHub Pages

Push **this repository root** to a GitHub repository named `sasingh07.github.io`. In the repository's **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)`. GitHub Pages runs Jekyll automatically; do not upload `_site` or configure an Actions build. The `_config.yml` `url` is the user-site URL and `baseurl` is intentionally empty. Internal site URLs use Jekyll's `relative_url` filter.

The `github-pages` gem in `Gemfile` is for matching the GitHub Pages Jekyll environment when previewing locally. `jekyll-seo-tag` emits page metadata; `jekyll-sitemap` emits `/sitemap.xml`. Both are supported by GitHub Pages. The SVG favicon is in `assets/favicon.svg`.

## Preview locally

Install Ruby and Bundler, then run from the repository root:

```sh
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000/`. If your environment already supplies the `github-pages` gem, `jekyll serve` also works. Configuration changes require restarting the local server.

## Check quality

Once the site is serving, open Chrome DevTools → **Lighthouse**, select **Navigation** and run **Performance**, **Accessibility**, **Best Practices**, and **SEO** for the home page and each subpage. Aim for at least 90 in each category; repeat in an incognito window without extensions and test the published site again. Check at 375px and 1280px widths, the light and dark OS preferences, keyboard navigation, and all links. Scores vary by browser and hosting environment, so do not treat an unrun audit as a pass.

## Structure

- `index.md`, `about.md`, `experience.md`, `contact.md` — content
- `_layouts/default.html` — semantic page shell and SEO tag
- `_includes/` — shared header/footer
- `_data/navigation.yml` — navigation labels/URLs
- `assets/css/style.css`, `assets/favicon.svg` — visual assets
- `_config.yml`, `Gemfile` — Jekyll/GitHub Pages configuration

There is no JavaScript, backend, database, tracking script, or third-party font request.

## Design conventions

The approved refinement is documented in `Change1.md`, which is excluded from published output. Keep the site single-column and use the existing CSS custom properties for the navy/blue light and dark palettes. Color schemes follow the visitor's system preference.

Use the shared section, date, and role styles when updating pages rather than inline CSS. Preserve semantic heading order and descriptive links. Financial figures in work highlights must retain their context: portfolio size is not an investment return, and committee approval of a pricing strategy is not a realized transaction.
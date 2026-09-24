# sasingh07.github.io

This project is a GitHub Pages Jekyll user site. Keep the actual publishable site at repository root, not in an artifact or generated output folder.

## Content and structure
- Markdown pages with YAML front matter are at root; navigation is in `_data/navigation.yml`.
- Shared shell lives in `_layouts/default.html`, `_includes/header.html`, and `_includes/footer.html`.
- CSS and favicon live under `assets/`.
- Preserve `url: "https://sasingh07.github.io"` and `baseurl: ""` in `_config.yml` for the user site; use `relative_url` for internal paths.
- Never invent biography, work history, employers, metrics, or projects. Leave visible placeholders where source material has not been supplied.
- No backend, Node app, React/Vite app, or nested website. No third-party tracking.

## Run
- `jekyll build` checks the static output in `_site/`.
- `jekyll serve --host 0.0.0.0 --port 5000` previews locally in this environment.
- GitHub Pages deploys from branch `main`, folder `/ (root)`, with no manual build.
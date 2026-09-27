# RTBX site

One-page Hugo site for rtbx.io, built from `doc/RTBX.IO.pdf`.

## Structure

- `web/` — Hugo site source (config, content, data, layouts, CSS).
- `doc/` — source material.
- `.github/workflows/hugo.yml` — builds and deploys `web/` to GitHub Pages on every push to `main`.

## Local development

```
cd web
hugo server
```

## Deploying

Push to `main`. The workflow builds the site and publishes it to GitHub Pages automatically.

One-time setup in the repo's GitHub settings: **Settings → Pages → Build and deployment → Source: GitHub Actions**.

The build sets `baseURL` from the Pages URL automatically, so it works both for a `<user>.github.io` repo and for a project repo served at `<user>.github.io/<repo>/`.

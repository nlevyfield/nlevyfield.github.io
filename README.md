# Sunflower Strategies LLC

Website for [sunflowerstrategies.la](https://sunflowerstrategies.la), built with [Hugo](https://gohugo.io) and the [Ananke](https://github.com/theNewDynamic/gohugo-theme-ananke) theme.

## Edit content

All text (tagline, services, bio, testimonials) lives in `content/_index.md`.
Email, LinkedIn, and menu links live in `hugo.toml`.
Images live in `static/images/`; styling in `static/css/custom.css`.

## Preview locally

```bash
pixi global install hugo
git submodule update --init
hugo server
```

Open http://localhost:1313.

## Deploy

Every push to `main` builds and publishes via `.github/workflows/deploy.yml`.
In the GitHub repo: **Settings → Pages → Source: GitHub Actions**.

## Custom domain

In **Settings → Pages → Custom domain**, enter `sunflowerstrategies.la`, then add DNS records at the registrar:

- `A` records for `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- `CNAME` for `www`: `nlevyfield.github.io`

# Dongchu Xie's Academic Website

Source code for <https://dongchuxie8-source.github.io/>, built with
[Hugo Blox](https://hugoblox.com/) and deployed with GitHub Actions.

## Requirements

- Hugo Extended 0.162.0 (pinned in `hugoblox.yaml`)
- Node.js 22
- pnpm 10.14.0

## Local development

```bash
pnpm install
pnpm dev
```

Open <http://localhost:1313/>.

## Production build

```bash
pnpm install
pnpm build
```

The generated site is written to `public/`, which is intentionally excluded
from Git. GitHub Actions performs this build and deploys the artifact.

## Updating content

- Profile, education, experience, and awards: `data/authors/me.yaml`
- Homepage biography and news: `content/_index.md`
- Publications: `content/publications/<publication>/index.md`
- Navigation: `config/_default/menus.yaml`
- Site identity and SEO: `config/_default/params.yaml`
- CV: `static/uploads/Dongchu_Xie.pdf`

Each publication can include `cite.bib`, a `featured.png` image, and a local
PDF in its own folder.

## Deployment

Pushes to `main` trigger `.github/workflows/deploy.yml`. In the GitHub
repository, **Settings → Pages → Build and deployment → Source** must be set
to **GitHub Actions**.

Do not edit files in `public/` or previously generated HTML directly; they are
recreated on every build.

## Compatibility override

`layouts/_partials/functions/build_links.html` is a small compatibility
override for the pinned Hugo Blox module. It replaces URL-keyed
`Scratch.SetInMap` calls, which fail with Hugo 0.162.0, with flat Scratch keys.
Remove the override after a future Hugo Blox release includes the same fix.
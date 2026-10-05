# VESL website

The public website for **vesl.se** — VESL, Vascular Experimental Systems Lab.
Plain HTML/CSS with no build step.

```
index.html     Page content
styles.css     Look and layout (colours taken from the logo)
logo.svg       Logo
favicon.svg    Browser-tab icon
```

## Editing

1. Open `index.html` in a browser to preview. No tools need installing.
2. Edit `index.html` (content) and `styles.css` (look).
3. Text marked `TODO` in `index.html` is placeholder copy to replace.

## How changes go live

The site is hosted on **Cloudflare Pages**, connected to this repo:

- Anything merged into `main` is published to vesl.se automatically.
- Every pull request gets its own preview link, posted on the pull request, so the
  change can be reviewed in a browser before it is merged.

### Cloudflare Pages settings (one-time setup)

| Setting                | Value            |
|------------------------|------------------|
| Production branch      | `main`           |
| Framework preset       | None             |
| Build command          | *(leave empty)*  |
| Build output directory | `/`              |

Then add `vesl.se` and `www.vesl.se` as custom domains in the Pages project and
create the DNS records Cloudflare shows in one.com's DNS settings. Leave the MX
(email) records at one.com untouched.

## Collaborating

See [CONTRIBUTING.md](CONTRIBUTING.md).

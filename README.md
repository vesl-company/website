# VESL website

The public website for **[vesl.se](https://vesl.se)**: VESL, Vascular Experimental Systems Lab.
Plain HTML/CSS with no build step.

```
index.html     Page content
styles.css     Look and layout (colours taken from the logo)
logo.svg       Logo
favicon.svg    Browser-tab icon
CNAME          Custom domain (created by GitHub, do not delete)
```

## Editing

1. Open `index.html` in a browser to preview. No tools need installing.
2. Edit `index.html` (content) and `styles.css` (look).
3. Text marked `TODO` in `index.html` is placeholder copy to replace.

Small text changes can also be made directly on GitHub: open the file, click the
pencil icon, and choose "Create a new branch" when committing.

## How changes go live

The site is hosted on **GitHub Pages** from this repository:

- Anything merged into `main` is published to vesl.se automatically, usually
  within a minute or two.
- The progress of each publish is shown under the repository's **Actions** tab.
- There are no automatic preview links for pull requests. To check a change
  before merging, download the branch and open `index.html` locally.

### GitHub Pages settings (Settings → Pages)

| Setting        | Value                    |
|----------------|--------------------------|
| Source         | Deploy from a branch     |
| Branch         | `main`, folder `/ (root)`|
| Custom domain  | `vesl.se`                |
| Enforce HTTPS  | On                       |

### DNS (managed at one.com)

| Type  | Name  | Value                    |
|-------|-------|--------------------------|
| A     | `@`   | `185.199.108.153`        |
| A     | `@`   | `185.199.109.153`        |
| A     | `@`   | `185.199.110.153`        |
| A     | `@`   | `185.199.111.153`        |
| CNAME | `www` | `vesl-company.github.io` |

`www.vesl.se` redirects to `vesl.se`. The email (MX) records at one.com are separate
and must not be changed. Do not add wildcard records such as `*.vesl.se`.
The IP addresses are listed in
[GitHub's documentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).

## Collaborating

See [CONTRIBUTING.md](CONTRIBUTING.md).

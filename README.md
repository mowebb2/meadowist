# meadowist.dev

Resources for maintaining Seattle's urban forests and parklands.

## Overview

Static website hosting the meadowist project hub. Built with plain HTML + CSS — zero dependencies, no build step.

## Deployment

This site is deployed on **Cloudflare Pages** via GitHub integration. Pushing to the `main` branch automatically triggers a production deployment.

### Cloudflare Pages Setup (one-time)

1. Go to the [Cloudflare Dashboard](https://dash.cloudflare.com/) → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**.
2. Select the `mowebb2/meadowist` repository.
3. Configure the build settings:

   | Setting          | Value            |
   | ---------------- | ---------------- |
   | Production branch | `main`          |
   | Build command    | *(leave empty)*  |
   | Build output directory | `/` (root) |

   > **Note:** Since this is a static site with no framework and no build step, leave the build command empty and set the output directory to the repository root (`/`).

4. Click **Save and Deploy**.

### Custom Domain

To serve the site at `meadowist.dev`:

1. In the Cloudflare Pages project, go to **Custom domains** → **Set up a custom domain**.
2. Enter `meadowist.dev` and follow the prompts.
3. Ensure DNS records for `meadowist.dev` are managed by Cloudflare (or add the required CNAME record).

### Deploying Updates

Simply push to `main`:

```bash
git add .
git commit -m "Update site"
git push origin main
```

Cloudflare Pages will automatically build and deploy the new version.

### Preview Deployments

Any pull request opened against `main` will automatically generate a **preview deployment** with a unique URL, so changes can be reviewed before merging.

## Project Structure

```
.
├── index.html          # Home page
├── style.css           # Styles (green nature theme)
├── _headers            # Cloudflare Pages custom headers
├── _redirects          # Cloudflare Pages redirects
├── meadowist.png       # Site logo
├── meadowist-small.png # Small site logo
└── gsp-events.png      # Work Party Notifier project logo
```

## Related Projects

- **Work Party Notifier** (`gsp-events.meadowist.dev`) — Cloudflare Worker app that monitors the Green City Partnerships calendar and emails subscribers when new volunteer events match their keywords.
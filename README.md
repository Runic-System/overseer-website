# Overseer website

Public support and privacy pages for Overseer, an independent Android companion for Seerr. This repository contains only the static website.

## Publishing

In repository **Settings → Pages**, choose **Deploy from a branch**, then **main** and **/(root)**, and save. The site requires no build step or dependencies. `.nojekyll` disables Jekyll processing.

Default home: https://runic-system.github.io/overseer-website/

Privacy policy: https://runic-system.github.io/overseer-website/privacy/

## Maintaining the site

- Edit `index.html` for the homepage and support contact.
- Edit `privacy/index.html` for the policy; update its effective date when practices change.
- Shared responsive styling is in `assets/site.css`.
- Pages use relative links so they also work with an optional custom domain.
- Keep this repository limited to public website content. Do not add credentials, personal server information, private application source, or unsigned/test APKs.

No scripts, analytics, remote fonts, embedded media, or third-party assets are included. GitHub Pages processes visitors' network information as described in the published policy.

## Optional custom domain

The GitHub-provided address works without any DNS changes. To later use `overseer.runicsystems.net`, first verify the domain in GitHub, set the custom domain in Pages settings, then add the subdomain's CNAME at the DNS provider pointing to `runic-system.github.io` (no path). Preserve existing mail-related DNS records. Enable HTTPS after GitHub provisions the certificate.

See [GitHub's custom-domain instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).

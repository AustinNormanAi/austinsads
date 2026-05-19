# Austin's Ads Portfolio

Static GitHub Pages portfolio for `austinsads.com`.

## Deploy

1. Create a new GitHub repo, for example `austinsads`.
2. Upload `index.html`, `CNAME`, and `.nojekyll`.
3. In GitHub, open `Settings -> Pages`.
4. Set the source to the `main` branch root.
5. In `Settings -> Pages`, add the custom domain `austinsads.com`.
6. In Squarespace DNS, point the domain to GitHub Pages using GitHub's current Pages DNS records.

## DNS records for Squarespace

For the apex/root domain `austinsads.com`, add these `A` records with host/name `@`:

```text
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Optional IPv6 `AAAA` records with host/name `@`:

```text
2606:50c0:8000::153
2606:50c0:8001::153
2606:50c0:8002::153
2606:50c0:8003::153
```

For `www.austinsads.com`, add a `CNAME` record:

```text
www -> YOUR-GITHUB-USERNAME.github.io
```

After GitHub detects the DNS, turn on `Enforce HTTPS` in the repo's Pages settings. DNS changes can take up to 24 hours to propagate.

## Edit

The whole site is in `index.html`. Search for `mailto:a@austinsads.com` and replace it with the best contact email if needed.

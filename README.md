# workwithsushmita.com

Portfolio site for Sushmita Mishra, Amazon Ads and retail media consultant.
It's a single static page (`index.html`) hosted on GitHub Pages.

## Files

- `index.html`: the whole site, with styles included.
- `CNAME`: tells GitHub Pages to serve the site at workwithsushmita.com. Keep it in the repo.

## Publish on GitHub Pages

1. On GitHub, create a new **public** repository, for example `portfolio`.
2. Click **Add file > Upload files**, drag in `index.html`, `CNAME` and `README.md`, and commit to the `main` branch.
3. Open **Settings > Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, choose `main` and `/ (root)`, and save.
4. In the same page, **Custom domain** should already show `workwithsushmita.com` (from the CNAME file). If not, type it and save.

## Point the domain to GitHub

In the DNS settings where you bought the domain, add these records.
Remove any existing A records for `@` first, such as a parking page.

| Type  | Host / Name | Value                       |
|-------|-------------|-----------------------------|
| A     | @           | 185.199.108.153             |
| A     | @           | 185.199.109.153             |
| A     | @           | 185.199.110.153             |
| A     | @           | 185.199.111.153             |
| CNAME | www         | YOUR-GITHUB-USERNAME.github.io |

Replace `YOUR-GITHUB-USERNAME` with your GitHub username.

DNS changes can take from a few minutes up to 24–48 hours.

## Turn on HTTPS

Once GitHub shows the DNS check as successful in **Settings > Pages**,
tick **Enforce HTTPS**. The certificate can take up to an hour to appear.

## Recommended: verify the domain

In your GitHub account (not the repo), go to **Settings > Pages > Add a domain**
and follow the steps to add a TXT record. This stops anyone else from using
your domain on GitHub Pages.

## Updating the site

Edit `index.html` on GitHub (pencil icon) and commit. The live site updates within a minute or two.

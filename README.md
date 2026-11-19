# Alice Huang — Photography

One-page website for Alice Huang, a freelance wedding and portrait photographer.

It's plain HTML and CSS with no build step. Open `index.html` in a browser, or serve the folder from any static host (GitHub Pages, Netlify, etc.).

## Deploy to Vercel

The site is static, so there's nothing to build.

1. In Vercel, choose **Add New → Project** and import this GitHub repo.
2. Leave **Framework Preset** as **Other**, with no build command and the output directory left as the default.
3. Click **Deploy**. Each push to `main` redeploys automatically, and pull requests get preview links.

Or from the command line: `npx vercel` for a preview, `npx vercel --prod` for production.

`vercel.json` turns on clean URLs, caches images for a year and adds basic security headers. If you replace a photo, give the new file a new name so visitors don't get the cached old one.

## Structure

- `index.html`: the whole page: hero, portfolio grid, about, contact
- `images/`: portfolio photos
- `vercel.json`: Vercel hosting config (URLs, caching, headers)

## Still to fill in

- `[your city]` in the about section
- `[you@yourdomain.com]` in the contact block (both the link text and the `mailto:`)
- Five portfolio placeholders. To add a photo, replace a placeholder `<figure>` with the same markup as the first tile: `class="tile photo"` and an `<img>` with alt text.

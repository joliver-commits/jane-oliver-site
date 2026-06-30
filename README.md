# Jane Oliver — personal site

Plain HTML/CSS, no build step. Three files do all the work:

```
index.html      page content
styles.css      design system (palette, type, layout)
assets/Jane_Oliver_CV.pdf   your CV, linked from the nav + contact section
```

## Edit the content

Open `index.html` in any text editor. Each section is commented with its
purpose (about / research / contact). Swap text directly — no templating
syntax to worry about. To swap your CV, just replace
`assets/Jane_Oliver_CV.pdf` with an updated file of the same name (or update
the two `href` links in `index.html` if you rename it).

## Host it free — GitHub Pages (recommended)

1. Create a new GitHub repo, e.g. `jane-oliver-site`.
2. Upload these three items (`index.html`, `styles.css`, `assets/`) to the
   repo root — drag-and-drop works fine on github.com, or:
   ```
   git init
   git add .
   git commit -m "first version of site"
   git branch -M main
   git remote add origin https://github.com/<you>/jane-oliver-site.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Branch: main → / (root) → Save**.
4. Your site goes live at `https://<you>.github.io/jane-oliver-site/`
   within a minute or two.
5. (Optional) Add a custom domain under the same Pages settings later.

## Host it free — Netlify (drag-and-drop alternative)

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag the whole project folder onto the page.
3. Netlify gives you a live URL immediately; you can rename the subdomain
   or attach a custom domain from the site settings.

## Updating later

Edit the files, then either `git push` again (GitHub Pages redeploys
automatically) or re-drag the folder onto Netlify Drop.

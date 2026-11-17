# Isabela Lico – website

## What is in this folder
- `index.html` – the whole website (design + code)
- `data/articles.json` – **your articles** (the editing form changes this file)
- `images/` – your photos and the Odds & Ends logo (new article images go to `images/uploads/`)
- `.pages.yml` – tells Pages CMS what the "Articles" form looks like
- `.nojekyll` – tells GitHub to publish the files exactly as they are

## One-time setup (about 20 minutes)
1. **Create a GitHub account** at github.com (free). Turn on two-step verification when it asks.
2. **Create a repository:** the "+" at the top right → *New repository*. Name it e.g. `isabela-lico-site`, set it to **Public**, tick *Add a README file*, then *Create*.
3. **Upload the files:** in the repository click *Add file → Upload files* and drag in `index.html`, the `data` folder and the `images` folder. Click *Commit changes*.
4. **Add the two hidden files** (Mac and Windows hide files that start with a dot, so create them on GitHub instead):
   - *Add file → Create new file*, name it `.pages.yml`, paste the contents of `pages.yml.txt`, commit.
   - *Add file → Create new file*, name it `.nojekyll`, leave it empty, commit.
5. **Turn the site on:** *Settings → Pages* → Source: *Deploy from a branch* → branch `main`, folder `/ (root)` → Save. After a minute or two GitHub shows your site's address.
6. **Use your own domain:** still in *Settings → Pages*, type your domain under *Custom domain* and save. GitHub then shows exactly which records to add at the company where you bought the domain (DNS settings). When GitHub's check turns green, tick *Enforce HTTPS*.

## Adding an article (every time after that)
1. Go to **app.pagescms.org** and sign in with GitHub. The first time, install the Pages CMS GitHub app on your account and pick this repository.
2. Open **Articles**, add a new entry, fill in the form (upload the image there too) and save.
3. Wait a minute or two, then refresh your website.

## Changing the design
Send the changes to Claude. You will get a new `index.html`; replace the old one in the repository (*Add file → Upload files*, same name) and your articles stay untouched.

## Opening the site on your own computer
Double-clicking `index.html` will show an empty site, because browsers block loading `data/articles.json` from a local file. Look at your live site instead.

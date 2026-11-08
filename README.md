# Come Expecting International website

The website for Evangelist Luigi Marcelino Daniele and Come Expecting International.

## What's in this folder

- `index.html` is the whole website: every page, the styles, and the code.
- `images/` holds the photos. The site uses these exact file names, so keep the folder and names as they are.

## Put it online with GitHub Pages

A computer is easiest for this.

1. On GitHub, create a new repository (for example `come-expecting-international`) and make it **Public**.
2. On the repository page, choose **Add file → Upload files**. Drag in `index.html`, `README.md`, and the whole `images` folder, then click **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment," set the source to **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder, and click **Save**.
4. After a minute or two, the site will be live at `https://YOUR-USERNAME.github.io/come-expecting-international/`.

## Use comeexpectinginternational.com

1. In **Settings → Pages → Custom domain**, type `comeexpectinginternational.com` and click **Save**.
2. Where the domain was bought (GoDaddy, Namecheap, Squarespace, etc.), open the DNS settings and add:
   - Four **A** records for `@` pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, and `185.199.111.153`
   - One **CNAME** record for `www` pointing to `YOUR-USERNAME.github.io`
3. Once GitHub confirms the domain (this can take up to a day), turn on **Enforce HTTPS**.

If the domain's email is set up with the same company, leave the existing email (MX) records alone. Only add the records above.

## Things to finish

- **Forms (booking, contact, newsletter):** they're in preview mode and don't send anywhere yet. Create free forms at formspree.io (have them deliver to LuigiandGiovannia@comeexpectinginternational.com), then paste each form's link into `FORM_ENDPOINTS` near the bottom of `index.html`.
- **Upcoming events:** search `index.html` for "When a meeting is booked" for a ready-made example to copy for each new event.
- **Impact numbers:** search for `data-count` to update the meals, salvations, and feeding events (they appear on the home page and the Give page), and update the "as of" date next to them.
- **Giving:** the "Support us" button on the Give page goes to the ministry's Stripe link.

## Editing later

Click `index.html` on GitHub, then the pencil icon to edit. After you commit, the live site updates within a minute or two.

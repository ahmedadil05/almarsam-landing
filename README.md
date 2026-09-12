# Al-Marsam — temporary landing page

A single, self-contained page to put Al-Marsam online *today*, while the
full booking site (see the main `almarsam` project) gets finished and
deployed. No backend, no build step — just one HTML file.

## Before you deploy — 2 things to fill in

1. **Payment link.** Create a Payment Link from your Tap Payments dashboard
   (no code needed — Tap supports this natively), then open `index.html`,
   find the `Book & Pay` button, and replace `href="#"` with your real link.
2. **Photos.** The gallery section has 4 placeholder tiles. Replace them
   with `<img src="your-photo.jpg">` once you have real studio/work photos
   to show — drop the image files in this same folder.

## Deploy for free with GitHub Pages

1. Create a new **public** GitHub repository (e.g. `almarsam-landing`).
2. Upload `index.html` and `logo.jpg` to it (drag-and-drop works fine on
   github.com, or `git push` if you're comfortable with git).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`,
   branch `main`, folder `/ (root)`. Save.
5. GitHub gives you a live URL in a minute or two, typically:
   `https://<your-username>.github.io/almarsam-landing/`
6. (Optional) Point your own domain at it later via the same Pages settings.

That's it — no server, no hosting cost, and it updates automatically every
time you push a change to the repo.

## Instagram booking bot (separate step, not part of this page)

For DM automation on Instagram (e.g. someone messages "book" and gets your
booking/payment link automatically), don't build this custom — use a
no-code tool that runs on Instagram's official API:

- **ManyChat** — free tier (25 active contacts), most widely used
- Set up a keyword trigger (e.g. "book") that auto-replies with your Tap
  Payment Link or a link to this landing page

Avoid any tool that asks for your Instagram password directly instead of
logging in through Meta's official connection — that's the kind of tool
that gets accounts restricted.

# NexGen Funnels — portfolio site

Static one-page portfolio for NexGen Funnels (Kiran, Website & Funnel Strategist). Plain HTML, CSS and JS with no build step, so it can be hosted anywhere that serves files.

## What's inside

| Path | What it is |
|---|---|
| `index.html` | The landing page |
| `project.html` | Live demo viewer: loads a live site in a desktop and mobile frame (`project.html?p=aara`) |
| `work/` | Recent Work images (1080 × 1080 originals from nexgenfunnels.com, resized) |
| `demos/`, `flowpilot-*.jpg` | Live demo thumbnails |
| `videos/` | Client testimonial videos and their poster images |
| `kiran.jpg` | About section portrait |
| `logo-mark.svg` | Favicon / logo mark |

## Common edits

- **CTA link (WhatsApp):** every "Book a Call" button uses `BOOKING_URL` near the bottom of `index.html` and `project.html` (currently `https://wa.me/919113290223`).
- **Live demos:** edit the `PROJECTS` list at the bottom of `project.html`. The key (e.g. `aara`) is what goes after `?p=` in the card link in `index.html`.

## Deploy to Hostinger with Git

1. In hPanel, open **Websites → Manage → Advanced → GIT**.
2. Under **Create a new repository**:
   - Repository: `https://github.com/<your-username>/nexgen-funnels-site.git`
   - Branch: `main`
   - Directory: leave **empty** so it deploys into `public_html`.
   Hostinger needs `public_html` to be empty first, so back up and remove any existing files there.
3. Click **Create**, then **Deploy**.
4. Optional: turn on **Auto Deployment**. Hostinger shows a webhook URL. Add it in GitHub under **Settings → Webhooks** (content type `application/json`) and every push to `main` then goes live automatically.

**Private repos:** Hostinger shows an SSH key on the same GIT page. Add it in GitHub under **Settings → Deploy keys**. Then use the SSH URL (`git@github.com:<your-username>/nexgen-funnels-site.git`) instead of the https one.

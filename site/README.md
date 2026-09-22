# WiCyS @ UCI — website

Static site. No build step: every file here is plain HTML/JS, served as-is.

## Deploy

**Netlify / Vercel / Cloudflare Pages** — drag this folder into the dashboard's deploy area, or point the project at the repo with:
- build command: *(none)*
- publish directory: `site`

**GitHub Pages** — push the contents of this folder to a repo, then Settings → Pages → deploy from branch, root.

Any static host works. To preview locally, run a server from this folder (`python3 -m http.server`) rather than opening the files directly, so the shared nav/footer load.

## Files

| File | Page |
|---|---|
| `index.html` | Home |
| `about.html` | About |
| `events.html` | Events |
| `project.html` | Cyber Project Competition |
| `join.html` | Get Involved |

`WiCySNav.dc.html`, `WiCySFooter.dc.html`, and `PixelSky.dc.html` are the shared nav, footer, and animated background — every page loads them, so keep them alongside the pages. `support.js` is the runtime; `images/` holds the logo and photos.

## Editing

Nav links, footer links, and the four application URLs live in the page files as ordinary HTML. Deadlines appear on `index.html` and `join.html`.

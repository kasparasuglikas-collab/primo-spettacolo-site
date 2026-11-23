# Primo Spettacolo – website

A bilingual (FR/EN) restaurant website in plain HTML, CSS and JavaScript. It needs no build step and no framework.

## Folder structure

```
primo-spettacolo-site/
├── index.html        ← the whole site: pages, styles and scripts
├── images/           ← home page and story photos
│   └── menu/         ← one photo per dish (1000×750)
└── README.md
```

## Open and preview in VS Code

1. Open VS Code → **File → Open Folder…** → choose `primo-spettacolo-site`.
2. Install the **Live Server** extension (by Ritwick Dey).
3. Right-click `index.html` → **Open with Live Server**. The site opens in your browser and reloads every time you save.

## Where to change things (all in `index.html`)

| What | Search for |
|---|---|
| Colours | `:root{` at the top of `<style>` (`--bg`, `--card`, `--accent`, `--marigold`) |
| Fonts | `fonts.googleapis.com` link and `--display` / `--body` |
| Opening hours | `var HOURS=` in the script (0 = Sunday … 6 = Saturday) |
| Menu: dishes, prices, photos | `var MENU = [` – each dish is `[name, French description, English description, vegetarian 1/0, price, photo file name]` |
| Address, phone, VAT | search `Vanderkindere`, `346 36 09`, `0443.350.574` |
| French / English text | every text appears twice: `<span class="fr">…</span><span class="en">…</span>` |
| Page links | `#home`, `#menu`, `#story`, `#book`, `#contact` |

## Booking form

The form only shows a confirmation message; nothing is sent yet. To receive bookings by email, create a free form at formspree.io and send the form data to it in the `bookForm` submit handler. You could also replace the form with a TheFork, Zenchef or Resengo booking widget.

## Put it online

1. **Netlify Drop** (free): go to app.netlify.com/drop and drag the whole folder in. You get a live link in seconds.
2. Buy a domain (e.g. `primospettacolo.be`) from a registrar such as Combell, One.com or OVH, then connect it in Netlify → *Domain settings*.
3. Add the site to Google Search Console and link it from the Google Business Profile.

## Photos – check before going public

- `images/menu/*` (except `carpaccio.jpg`): free Unsplash photos, OK for commercial use.
- `hero-tuscany.jpg`: an Adobe Stock **preview** with a faint watermark. Buy the licence or replace it.
- `antipasti.jpg`: an iStock **preview**. Buy the licence or replace it.
- `carpaccio.jpg`, `spaghetti-pomodoro.jpg`, `dolce-*.jpg`, `courtyard.jpg`, `evening.jpg`, `pasta-fresca.jpg` and the others the owner supplied: confirm the owner has the right to use them.
- The best option is the restaurant's own photos of its real dishes and terrace.

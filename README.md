# The Rugbones — RB WEBSITE

A lightweight single-file website (INDEX.html) serving as an EPK / promo landing page for The Rugbones.

## Project structure

- `INDEX.html` — single-page site with all content, styles and scripts. Uses Tailwind CDN and Google Fonts.
- `README.md` — this file.

> Note: This project is intentionally minimal and uses CDN-hosted dependencies (Tailwind CSS and Google Fonts) so no package manager is required to preview the site locally.

## Tech stack

- Plain HTML/CSS/JS
- Tailwind CSS (via CDN)
- Google Fonts: Monoton and Space Mono
- SVG icons embedded inline for social links and streaming platforms

## Quick preview (Windows / PowerShell)

Option A — Open directly (double-click)
- In File Explorer, double-click `INDEX.html` to open the page in your default browser.

Option B — From PowerShell (serve over a local HTTP server)

1. Open PowerShell in the project folder `c:\Users\RAJ\Desktop\RB WEBSITE`.
2. If you have Python 3 installed, run:

```powershell
# start a simple HTTP server on port 8000
python -m http.server 8000
```

3. Open the site in your browser:

```powershell
Start-Process "http://localhost:8000/"
```

Serving over HTTP is helpful if you later add features that require a server (fetch/XHR, service workers, etc.).

## Where to edit content

- The singles section is inside `INDEX.html` under the `SINGLES` comment (search for `<!-- SINGLES -->` or `KROME`, `ALL OF GODS MONEY`, `BRACELET`).
- Each single block contains the title, release date text and two icon links (Spotify + Apple Music). Update the `href` values on those anchor tags to point to per-track URLs if you prefer.
- The footer contains artist-level links for Spotify and Apple Music and social links for Instagram / TikTok.

Example snippet to replace (in `INDEX.html`):

```html
<!-- KROME -->
<a href="https://open.spotify.com/artist/therugbones" target="_blank" rel="noopener noreferrer">...</a>
<a href="https://music.apple.com/us/artist/the-rugbones/1691922711" target="_blank" rel="noopener noreferrer">...</a>
```

If you supply specific per-track URLs (Spotify track link and Apple Music song link), I can update these for you so each icon points directly to the song.

## Accessibility & small improvements you might want

- Add `aria-label` attributes to the icon links for screen-readers (I can add these if you'd like).
- Consider adding alt text to album images (currently placeholders) or replacing placeholders with real cover art.

## Contributing

1. Edit `INDEX.html` directly — it's a single-file site.
2. Commit and push your changes with your usual git workflow.

If you want me to make changes (replace placeholders, add small accessibility tweaks, or swap artist pages for exact track URLs), just tell me what to change and I'll update the file.

## License

This repository doesn't include a license file by default. If you'd like an open-source license added (MIT, Apache-2.0, etc.), tell me which one and I will add a `LICENSE` file.

## Contact

For press or additional info the site references the contact email:

`contact.ingoodco@gmail.com`

---

If you want, I can:
- Replace the artist-level links in the singles with exact per-track links (paste them here),
- Add `aria-label` attributes for the icon anchors, or
- Add a small CONTRIBUTING.md and a LICENSE file.

Which of those should I do next?
# nibblume-site

Landing, support and privacy pages for **Nibblume**, an iPhone game: a tiny lanternfish in black water. Hold Glow
to lure small fish, let go to hide from red eyes, eat to grow.

Live: https://nguyenvanlamm.github.io/nibblume-site/ · [support](https://nguyenvanlamm.github.io/nibblume-site/support.html) · [privacy](https://nguyenvanlamm.github.io/nibblume-site/privacy.html)

Plain static HTML and CSS, no build step and no JavaScript. GitHub Pages serves the `main` branch root directly
(no GitHub Actions). Bodoni Moda and IBM Plex Mono are self-hosted (SIL OFL 1.1, licences in `assets/fonts/`), so
the site makes no third-party requests. Screenshots come from the game's `test/shots_test.dart`.

Search and AI agents: `robots.txt`, `sitemap.xml`, `llms.txt`, a Markdown copy of each page (`*.html.md`, linked
from the page with `rel="alternate" type="text/markdown"`), JSON-LD in each `<head>`, and a 1200x630 share card
(`assets/img/share-card.jpg`, built from `assets/img/icon-512.png` and the site fonts). Keep the Markdown copies,
`llms.txt` and the JSON-LD in step with the pages when the copy or prices change.

Preview locally: `python3 -m http.server 8000` and open http://127.0.0.1:8000/.

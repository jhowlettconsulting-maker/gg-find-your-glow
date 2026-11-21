# Find Your Glow

Glow Getter Collective’s responsive “Find Your Glow” HTML widget.

Live widget: https://jhowlettconsulting-maker.github.io/gg-find-your-glow/

In Wix Studio, add an **Embed Site** element and use the live widget URL. Adjust its height at each breakpoint and preview the full quiz before publishing.

GitHub Pages serves the `main` branch from the repository root. `.nojekyll` keeps the HTML and bundled JavaScript unchanged during deployment.

## Files

- `gg-find-your-glow-responsive.html` — the supplied widget, exported from the open browser attachment.
- `index.html` — an identical copy for a static host’s default page.
- `widget-embed.css` — responsive iframe layout and narrow-screen adjustments, shared by both HTML pages.

Open either HTML file in a browser, or serve this folder with `python3 -m http.server 8000` and visit `http://localhost:8000`.

The HTML includes its JavaScript and base styles, with responsive overrides in `widget-embed.css`. Keep that stylesheet beside the HTML when hosting. Google Fonts requires internet access. Booking links and shade recommendations are preserved from the supplied source.

The browser extension’s body class and Codex overlay element were removed from the export. The top progress bar was removed at the owner's request. The quiz uses its iframe viewport and scrolls internally when the questions or results need more space.

Validated in Chrome at 300 × 580, 720 × 620, and 960 × 680, including the complete six-question flow, results, and restart on the narrowest size. Physical phones and other browsers have not been tested.

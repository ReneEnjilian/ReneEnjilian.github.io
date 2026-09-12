# René Enjilian — Portfolio

A working static website based on the approved portfolio design: warm off-white background, serif headings, a blue accent, and project illustrations.

Repository: [ReneEnjilian/ReneEnjilian.github.io](https://github.com/ReneEnjilian/ReneEnjilian.github.io). Intended site address: [reneenjilian.github.io](https://reneenjilian.github.io/).

The site uses ordinary HTML and one shared CSS file. There is no JavaScript, framework, package installation, or compilation step. Navigation and project pages work when you open the files directly in a browser.

## Preview

Open `index.html` in your browser. Keep the folder structure intact so the stylesheet and project links resolve.

For a local web server, run this command from the project folder:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

The fonts are loaded from Google Fonts. If that service is unavailable or you are offline, the site uses Georgia, Arial, and a system monospace fallback. Navigation and content continue to work.

## Where to edit

| File | Contents |
| --- | --- |
| `index.html` | Homepage introduction, project previews, and about section |
| `projects/kairos.html` | Kairos project page |
| `projects/systemds.html` | Apache SystemDS project page |
| `cv.html` | Short HTML overview of education and experience |
| `assets/css/styles.css` | Shared typography, colors, layout, and responsive styles |
| `.nojekyll` | Tells GitHub Pages to serve the static files without Jekyll processing |

Each HTML page is editable directly. The header and footer are repeated across four pages; update their links in all four when adding navigation items. Use relative links so the site works both at `username.github.io` and under `username.github.io/repository/`.

## Content status

This is the first implementation. The copy is an initial draft based on the project discussion. Review it before publishing.

- Kairos and SystemDS have real, separately addressable pages.
- The CV page is an HTML overview; it does not claim to download a PDF.
- Add the current CV PDF and its download link when available.
- The footer links to [ReneEnjilian on GitHub](https://github.com/ReneEnjilian). Email, thesis, and Kairos source links are awaiting the exact URLs.
- Writing is omitted until real articles are ready.
- Project graphics are conceptual illustrations, not benchmark results.

## Publish with GitHub Pages

1. Put these files at the repository root on a new branch, then open a pull request into `main`. Review and merge it when the site is ready to publish.
2. Open the repository's [Settings → Pages](https://github.com/ReneEnjilian/ReneEnjilian.github.io/settings/pages).
3. Set **Source** to **Deploy from a branch**, select **main** and **/(root)**, then save. If these settings are already selected, no change is needed.
4. Check the Pages deployment in the [Actions tab](https://github.com/ReneEnjilian/ReneEnjilian.github.io/actions), then visit [reneenjilian.github.io](https://reneenjilian.github.io/).

The files are already arranged at the repository root, including `.nojekyll` to skip Jekyll processing. Future changes merged into `main` will publish through the same Pages configuration. The pull request itself does not configure Pages.

GitHub references: [Creating a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) and [Configuring the publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Design and behavior

- The approved homepage layout and project illustrations are preserved.
- Shared styling adapts the layout for desktop and mobile screens.
- All navigation uses native links; browser back, opening in a new tab, and direct page URLs work normally.
- A skip link, visible keyboard focus, descriptive page titles, and reduced-motion support are included.
- The CV has print styling.

The copy is provisional. Review the content and add the current CV PDF and project links before treating the portfolio as final.

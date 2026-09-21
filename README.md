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
| `writing.html` | Index of technical articles; currently an empty state |
| `projects/kairos.html` | Kairos project page |
| `projects/systemds.html` | Apache SystemDS project page |
| `cv.html` | Redirects existing CV page links to the PDF |
| `assets/pdf/Rene_Enjilian_CV.pdf` | Current PDF CV; replace this file to update it |
| `assets/css/styles.css` | Shared typography, colors, layout, and responsive styles |
| `.nojekyll` | Tells GitHub Pages to serve the static files without Jekyll processing |

Each HTML page is editable directly. The header and footer are repeated across all pages; update their links in every page when adding navigation items. Use relative links so the site works both at `username.github.io` and under `username.github.io/repository/`.

## Content status

This is the first implementation. The copy is an initial draft based on the project discussion. Review it before publishing.

- Kairos and SystemDS have real, separately addressable pages.
- CV navigation links open `assets/pdf/Rene_Enjilian_CV.pdf` directly. The former `cv.html` page redirects to the PDF and includes a fallback link.
- The footer links to [ReneEnjilian on GitHub](https://github.com/ReneEnjilian). Email, thesis, and Kairos source links are awaiting the exact URLs.
- The Writing page is for technical articles and explanations. It has no published articles yet. When an article is ready, give it its own HTML page and add its title, publication date, short description, and link to the Writing index, replacing the empty-state message.
- Project graphics are conceptual illustrations, not benchmark results.

## Publish with GitHub Pages

1. Commit small, routine updates directly to `main`. Use a separate branch and pull request for major changes.
2. Open the repository's [Settings → Pages](https://github.com/ReneEnjilian/ReneEnjilian.github.io/settings/pages).
3. Set **Source** to **Deploy from a branch**, select **main** and **/(root)**, then save. If these settings are already selected, no change is needed.
4. Check the Pages deployment in the [Actions tab](https://github.com/ReneEnjilian/ReneEnjilian.github.io/actions), then visit [reneenjilian.github.io](https://reneenjilian.github.io/).

The files are already arranged at the repository root, including `.nojekyll` to skip Jekyll processing. Changes committed or merged into `main` will publish through the same Pages configuration.

GitHub references: [Creating a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) and [Configuring the publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Design and behavior

- The approved homepage layout and project illustrations are preserved.
- Shared styling adapts the layout for desktop and mobile screens.
- All navigation uses native links; browser back, opening in a new tab, and direct page URLs work normally.
- A skip link, visible keyboard focus, descriptive page titles, and reduced-motion support are included.
- Replace `assets/pdf/Rene_Enjilian_CV.pdf` to publish a new CV version without changing the navigation links.

The copy is provisional. Review the content and project links before treating the portfolio as final.

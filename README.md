# Boyi Zhang’s personal website

A responsive academic homepage built with plain HTML and CSS. No build step, JavaScript, external fonts, or package installation is required.

## Preview locally

From this folder, run:

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000. Stop the server with `Ctrl+C`.

## Publish on GitHub Pages

1. Commit and push these files to the `master` branch of `billycrapediem/billycrapediem.github.io` (or choose the branch you actually push to).
2. In the GitHub repository, open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**, choose `master` and **/(root)**, then save.
4. Leave **Custom domain** empty to use **https://billycrapediem.github.io/**. If `jonbarron.info` remains in that field from the original template, remove it in Settings. Removing the local `CNAME` file alone does not clear a domain already saved in GitHub.
5. Wait for the Pages deployment to finish; GitHub will show the published URL in the Pages settings.

The `.nojekyll` file tells GitHub Pages to serve the static site directly. All asset paths are relative, so the page also works under a repository subpath.

See [GitHub’s publishing-source instructions](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Update the content

- **`index.html`**: biography, research publications, hobbies, email, and social links.
- **`stylesheet.css`**: colors, typography, layout, and responsive breakpoints. Main design values are defined in `:root`.
- **`images/`**: portrait, research diagram, and favicons.

The biography includes HKUST supervisor Yangqiu Song and previous University of Rochester supervisor Hangfeng He. The original Rochester email is retained until a replacement address is provided.

The original version of this website was based on [Jon Barron’s website](https://jonbarron.info/).

The current layout takes inspiration from [Zeliang Zhang’s academic homepage](https://zhangaipi.github.io/): a short introduction, portrait, and simple research entries.

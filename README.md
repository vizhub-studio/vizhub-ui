# vizhub-ui — historical VizHub Bootstrap theme

This repository provides a custom **Bootstrap-derived stylesheet and UI assets** for an earlier VizHub interface. It is a styling package, not the current VizHub application's complete design system. Its checked-in source consists primarily of [`scss/`](scss/) and [`icons/`](icons/).

## Local build and inspection

The root `package.json` defines these commands:

```bash
npm install
npm run build     # Compile scss/vizhub-ui.scss to dist/vizhub-ui.css
npm run minify    # Minify the compiled CSS
npm run dev       # Serve this directory with http-server
```

Open `index.html` using the local server's printed address after compiling. `npm run dev` alone does **not** compile Sass; run `npm run build` first when testing stylesheet changes.

## Historical context and verification

- The [Sass entry point](scss/vizhub-ui.scss) imports theme partials and may depend on the package's Bootstrap tooling.
- There is **no automated test script** in the root manifest. Validate compiled output, browsers, accessibility contrast and affected pages manually.
- Consuming applications must verify compatible Bootstrap version and class names before adopting the CSS.
- [VizHub](https://vizhub.com/) is the current user-facing product. Historical screenshot colors and CSS here are not proof of current deployed UI.
- See [LICENSE](LICENSE) before redistributing the stylesheet or assets.

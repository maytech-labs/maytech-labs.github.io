# maytech-labs.github.io

[![License: REAL 1.0](https://img.shields.io/badge/License-REAL_1.0-blue.svg)](LICENSE.md)

The MayTech Labs website, served by GitHub Pages at <https://maytech-labs.github.io>.

Plain HTML and CSS, no build step. Preview locally:

```sh
python3 -m http.server
```

## Adding a project

1. In `index.html`, copy a `<a class="card">` block into the Tools or Learn & license section. Change the link, the preview in `.art` (and its color class, `a-blue`, `a-green`, `a-pink`, `a-orange`, `a-purple`, `a-teal`, or `a-indigo`), the name, the badge, the description, and the link text.
2. Keep the badge either `pre-release` or the latest release version, like `0.1.1`. `org-status` checks it.
3. Add the project to the table in [`.github/profile/README.md`](https://github.com/maytech-labs/.github/blob/main/profile/README.md).
4. Run `scripts/org-status.py` in the `.github` repo; it should report no drift for the new project.

If you change `style.css`, bump the `?v=` on its `<link>` so browsers don't use a cached copy.

## License

[REAL 1.0](LICENSE.md)

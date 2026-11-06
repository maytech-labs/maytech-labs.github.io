# maytech-labs.github.io

[![License: REAL 1.0](https://img.shields.io/badge/License-REAL_1.0-blue.svg)](LICENSE.md)

The MayTech Labs website, served by GitHub Pages at <https://maytech-labs.github.io>.

Plain HTML and CSS, no build step. Preview locally:

```sh
python3 -m http.server
```

## Adding a project

1. In `index.html`, copy a `<a class="card">` block into the Tools, Learn & license, or Fun section. Change the link, the preview in `.art` (and its color class, `a-blue`, `a-green`, `a-pink`, `a-orange`, `a-purple`, `a-teal`, `a-indigo`, or `a-peach`), the name, the badge, the description, and the link text.
2. Keep the badge either `pre-release` or the latest release version, like `0.1.1`. `org-status` checks it.
3. Add the project to the table in [`.github/profile/README.md`](https://github.com/maytech-labs/.github/blob/main/profile/README.md).
4. Run `scripts/org-status.py` in the `.github` repo; it should report no drift for the new project.

Fun is for toys, like termigatchi. While it holds only a few, its cards use `card wide`, which spans the row with the preview beside the text; drop `wide` once there are three or more.

## Adding a project page

Copy `tolarian-machine/index.html` into a new folder, like `my-project/index.html`, and point the project's card at `/my-project/`. Pages use root-relative paths (`/style.css`), so preview them through `python3 -m http.server`, not by opening the file. Set the `active` tab to the section the card lives in.

If you change `style.css`, bump the `?v=` on its `<link>` so browsers don't use a cached copy.

Ideas for the site that haven't shipped yet are in [`docs/ideas.md`](docs/ideas.md).

## License

[REAL 1.0](LICENSE.md)

Exception: the Junior lab (the made-up companies, their names, menus, slogans, and artwork) is not licensed under REAL 1.0. Copyright (c) 2026 MayTech Labs, all rights reserved. That covers the `barleys-tired-root-beer/`, `breadys/`, `burger-up/`, `h-diner/`, `tilde-house/`, and `old-fashioned-link-hotel/` pages, the Junior lab section of `index.html`, and the Junior lab styles in `style.css`.

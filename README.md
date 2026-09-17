# HereSphere Community Guide

An unofficial, community-maintained user guide for the [HereSphere](https://heresphere.com) VR video player.

HereSphere has little formal documentation. Most know-how lives in the developer's answers in the HereSphere Discord `#instructions` channel. This guide collects those answers into searchable pages.

**Read the guide:** https://USERNAME.github.io/heresphere-guide/

## How the site works

- Pages are Markdown files in `docs/`.
- The menu order is set in `mkdocs.yml` under `nav:`.
- Every push to `main` rebuilds the site with [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) through GitHub Actions and publishes it to the `gh-pages` branch.

## Editing a page

Open the page's `.md` file on GitHub, click the pencil icon, make your change, and commit. On the live site, the pencil icon at the top of each page links straight to that file.

To add a page, create a `.md` file in `docs/` and add it to `nav:` in `mkdocs.yml`.

## Previewing locally (optional)

```bash
pip install -r requirements.txt
mkdocs serve
```

Then open http://127.0.0.1:8000.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Open work is listed in [ROADMAP.md](ROADMAP.md).

## License

Content is licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). See `LICENSE`.

This project is not affiliated with or endorsed by the HereSphere developer.

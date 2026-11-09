# Project Guidelines

This repository builds the academic website at [damelo.net](https://damelo.net/). See [README.md](README.md) for the site overview and local preview/build commands.

## Posts

- Add posts under `content/post/`, following the neighboring dated directories and front matter.
- Preserve each post's related bibliography and CSL files when editing citations.
- Hugo ignores `.Rmd` and `.Rmarkdown` files (see `config.yaml`). When a post has both an R Markdown source and a rendered `index.html`, update the source and refresh the rendered HTML so the published page reflects the change.

## Code

- The homepage Code section is a portfolio of pages in `content/project/`; its layout is configured in `content/home/code.md`.
- Add or update one project per directory, following nearby `index.md` files. Keep titles, summaries, tags, dates, and project links accurate; keep any featured image in that project directory.

## Publications

- Publication records live in `content/publication/<name>/`; the homepage listing is configured in `content/home/publications.md`.
- Follow neighboring `index.md` front matter for authors, dates, venue, DOI, abstract, and publication type. Keep associated PDFs, citation files, and featured images with the record, and ensure links point to the correct files or external resources.
- The homepage currently displays up to five publications in descending date order. Edit the widget configuration only when the listing itself should change.

## Validation

- For content or template changes, preview the affected sections with `hugo server` and check a production build with `hugo --gc --minify` when Hugo `0.87.0` is available.
- Do not assume changes to ignored R Markdown files alone will change the generated site.

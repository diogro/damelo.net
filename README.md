# damelo.net

The source for Diogo Melo's academic website, published at [damelo.net](https://damelo.net/). The site is built with Hugo and the Wowchemy v5 modules declared in `go.mod`.

## Website content

The homepage is assembled from widgets configured in `content/home/`. The sections of interest are:

| Homepage section | Content directory | Homepage configuration |
| --- | --- | --- |
| Posts | `content/post/` | `content/home/posts.md` |
| Code | `content/project/` | `content/home/code.md` |
| Publications | `content/publication/` | `content/home/publications.md` |

The homepage currently lists up to five posts and five publications, ordered by descending date. The Code section is a portfolio of project pages.

### Posts

Add or update a post in its own directory under `content/post/`. Existing directory names commonly start with a date, followed by a topic. Post metadata such as the title, date, slug, categories, and author is stored in the document's YAML front matter.

Some posts use citations with a `references.bib` bibliography and a CSL style file. Keep those files with the post when editing its citations. Some older posts have both an R Markdown source (`index.Rmd` or `index.Rmarkdown`) and a rendered `index.html`. Hugo ignores R Markdown files as configured in `config.yaml`, so changes to an R Markdown source must be rendered to HTML to appear on the site.

### Code

Each item in the Code portfolio is a project page under `content/project/<name>/`, usually defined in `index.md`. Add a new project by creating a directory and page there. Follow the neighboring pages for front matter, including a title, short summary, tags, date, and relevant links such as `url_code`; add a `featured` image when useful.

### Publications

Each publication has a page under `content/publication/<name>/`, usually `index.md`. Its front matter contains the title, authors, date, publication venue, DOI, abstract, and publication type. Add supporting files such as a PDF, `cite.bib`, and a `featured` image in the same directory, and link to them using the conventions in existing records.

## Preview and build

The Netlify build configuration pins Hugo to version `0.87.0`. With that version available, run these commands from the repository root:

```sh
hugo server
hugo --gc --minify
```

The first command serves a local preview; the second runs a production-style build. Netlify's configured build command is `hugo --gc --minify -b $URL`; see `netlify.toml` for deployment settings.

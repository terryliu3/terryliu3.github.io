# terryliu3.github.io

Personal academic website of Tuo Liu, built with Jekyll and the [al-folio](https://github.com/alshedivat/al-folio) theme. Pushing to `master` runs `.github/workflows/deploy.yml`, which builds the site into the `gh-pages` branch.

## Where the content lives

| Page | File |
| --- | --- |
| About (home): bio, address | `_pages/about.md` |
| News on the home page | `_news/*.md` (one file per item) |
| Publications | `_bibliography/papers.bib` |
| CV page | `_data/cv.yml` |
| CV PDF download | `assets/pdf/Tuo_Liu_CV.pdf` |
| Teaching | `_pages/teaching.md` |
| Name, email, Google Scholar, footer | `_config.yml` |

`Tuo_Liu_CV.yaml` is the [RenderCV](https://rendercv.com) source for the PDF. It is excluded from the built site, so changes there must be copied into `_data/cv.yml` and `papers.bib` by hand.

### Publication fields

Besides the standard BibTeX fields, entries in `papers.bib` support:

- `abbr`: venue badge (colours and links in `_data/venues.yml`)
- `selected = {true}`: show on the home page
- `preprint = {true}`: list under "preprints" instead of "conference papers"
- `openreview`, `arxiv`, `pdf`, `code`, `slides`, `thesis`: link buttons
- `award`: highlighted line under the venue, e.g. a spotlight
- `abstract`, `bibtex_show = {true}`: "Abs" and "Bib" toggles

To add a profile photo, put it at `assets/img/prof_pic.jpg` and add `image: prof_pic.jpg` under `profile:` in `_pages/about.md`.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

# tnikas.github.io

Personal website of Themistoklis Nikas: https://tnikas.github.io

Built with Jekyll and served by GitHub Pages from the `main` branch. The design is a customized
version of the [Thinkspace](https://github.com/heiswayi/thinkspace) theme (MIT, see [LICENSE](LICENSE)).

## Updating the site

| What | Where |
| --- | --- |
| Intro text | `_includes/intro.html` |
| News | `_data/news.yml` (newest first is not required; items are sorted by date) |
| Publications | `publications.md` |
| Name, description, profile links (email, Scholar, GitHub, LinkedIn) | `_config.yml` |
| Photo | `assets/images/author.jpg` (keep it small; ~600px wide is plenty) |

## Updating the CV

The CV source is `cv/Themistoklis_Nikas_CV.tex`. Edit it, then rebuild the PDF that the
site's "CV" link serves:

```sh
latexmk -pdf -cd -outdir=build cv/Themistoklis_Nikas_CV.tex && cp cv/build/Themistoklis_Nikas_CV.pdf .
```

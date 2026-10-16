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

The CV's LaTeX source is not in this repository: it lives locally in the gitignored `cv/`
folder. After editing `cv/Themistoklis_Nikas_CV.tex`, rebuild the PDF that the site's "CV"
link serves, and commit only the PDF:

```sh
latexmk -pdf -cd -outdir=build cv/Themistoklis_Nikas_CV.tex && cp cv/build/Themistoklis_Nikas_CV.pdf .
```

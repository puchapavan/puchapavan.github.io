# Pucha Srinivasa Pavan: personal website

Live at **https://srinivas50505.github.io**. Built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll template and published by GitHub Actions to the `gh-pages` branch.

## How to update the site

You can do all of this in the browser on GitHub: open the file, click the pencil icon, edit, and click **Commit changes**. The site rebuilds in a few minutes.

| To change | Edit this file |
| --- | --- |
| Add a paper | `_bibliography/papers.bib`. Paste the BibTeX from Google Scholar, then add `abbr = {VENUE},` and `selected = {true},` to show it on the home page. Optional: `pdf = {link},` `code = {link},` `doi = {...},` |
| Add a news item | Create a file in `_news/` named like `2027-01-15-short-name.md` (copy an existing one and change the date and text) |
| Add a project | Create a file in `_projects/` (copy an existing one). `importance` sets the order |
| Bio and photo | `_pages/about.md` and `assets/img/prof_pic.jpg` |
| Experience, education, skills, certifications | `_data/cv.yml` |
| Email, Scholar, GitHub, LinkedIn links | `_data/socials.yml` |
| Site colours | `_sass/_themes.scss` (`--global-theme-color`) |

## Run it locally (optional)

```bash
bundle install
bundle exec jekyll serve   # then open http://localhost:4000
```

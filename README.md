# Abel Mesfin — personal website

Built with [al-folio](https://github.com/alshedivat/al-folio) (Jekyll), based on the layout of [alexzhang13.github.io](https://github.com/alexzhang13/alexzhang13.github.io).

## Edit content
- Home / bio: `_pages/about.md` (photo: `assets/img/profile.jpg`)
- Experience: `_pages/experience.md`
- Projects: `_pages/projects.md`
- Blog posts: `_posts/YYYY-MM-DD-title.md`
- Name, email, social links: `_config.yml`
- Papers (when you have them): `_bibliography/papers.bib`, then set `selected_papers: true` in `about.md`

## Run locally
```bash
LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8 bundle exec jekyll serve
```
Then open http://localhost:4000.

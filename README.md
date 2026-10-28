# St CORTEX Lab website

Source for <https://st-cortex-lab.github.io>, the website of **St CORTEX Lab (Smart Cognitive Robot Dexterity Lab)**, University of St Andrews.
GitHub Pages builds it with Jekyll on every push to `main`.

## Editing content

All content lives in `_data/`, so you never need to touch the HTML:

| What | File |
| --- | --- |
| Team members, alumni, past members | `_data/people.yml` (photos → `assets/img/people/`) |
| Home-page project tiles | `_data/projects.yml` (GIF/JPG/PNG → `assets/img/projects/`) |
| Research themes | `_data/research.yml` |
| News items | `_data/news.yml` (newest first, latest 5 shown) |
| Publications | `_data/publications.yml` |
| Lab name, address, email, Scholar, socials | `_config.yml` |
| Navigation | `_data/navigation.yml` |

Use square photos (at least 400×400 px) and 16:10 project media.

## University branding

Colours follow the St Andrews palette (`--sta-blue: #00539b`). The official University logo is **not** included because its use is governed by the University's brand guidelines. Once you have an approved asset, add it at `assets/img/uni-logo.svg` and uncomment the `<img>` slot in `_includes/header.html`.

## Local preview

```bash
bundle install
bundle exec jekyll serve      # http://localhost:4000
# or, without Ruby:
docker run --rm -p 4000:4000 -v "$PWD":/srv/jekyll jekyll/jekyll:4 jekyll serve
```

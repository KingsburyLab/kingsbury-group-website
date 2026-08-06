# Kingsbury Research Group Website

This repository contains the Kingsbury Research Group website built with [Hugo](https://gohugo.io/) and the [Beautiful Hugo](https://github.com/halogenica/beautifulhugo) theme.

## Local Development

Beautiful Hugo currently requires Hugo `0.146.2` or newer.

Clone the repository with its theme submodule:

```bash
git clone --recurse-submodules https://github.com/KingsburyLab/kingsbury-group-website.git
cd kingsbury-group-website
```

If the repository is already cloned, initialize the theme once:

```bash
git submodule update --init --recursive
```

Start the local development server:

```bash
hugo server
```

## Structure

- `hugo.toml`: active Beautiful Hugo configuration.
- `content/_index.md`: homepage content.
- `content/research/_index.md`: research overview and section page.
- `content/people/team.md`: team and alumni page.
- `content/gallery/` and `content/gallery-events/`: group photos and event galleries.
- `content/news/`: lab news.
- `content/publication/`: publication metadata and publication pages.
- `content/contact/index.md`: contact page.
- `content/training.md`: resources page.
- `static/img/` and `static/video/`: media served by Beautiful Hugo.
- `layouts/`: Kingsbury Lab layout overrides and custom page templates.

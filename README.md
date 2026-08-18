# Cal Poly Data Design Lab website template

A GitHub Pages/Jekyll static website template for the Cal Poly Data Design Lab at Cal Poly San Luis Obispo. Lab members, projects, navigation, and site-wide settings are edited in YAML files under `_data/` and rendered automatically by reusable layouts/includes.

## Edit content

- `_data/site_settings.yml` — lab name, tagline, email, location, footer text.
- `_data/navigation.yml` — top navigation links.
- `_data/people.yml` — affiliated faculty, students, and alumni.
- `_data/projects.yml` — ongoing and past research projects.
- `_data/events.yml` — recurring reading groups, upcoming events, colloquia, invited speakers, and past event archives.
- `index.md`, `people.md`, `projects.md`, `events.md`, `about.md`, `join.md` — editable page copy.

## Add images

Place headshots in `assets/img/people/` and update the `image` field in `_data/people.yml`. If an image is omitted, the people card automatically uses `assets/img/people/placeholder.svg`.

## Run locally

```sh
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.


## Styling

The base stylesheet at `assets/css/tufte.css` is vendored from the official Tufte CSS project at https://github.com/edwardtufte/tufte-css. Lab-specific layout, cards, colors, and responsive additions live in `assets/css/site.css`.

# Cal Poly Data Design Lab website template

A GitHub Pages/Jekyll static website template for the Cal Poly Data Design Lab at Cal Poly San Luis Obispo. Lab members, projects, navigation, and site-wide settings are edited in YAML files under `_data/` and rendered automatically by reusable layouts/includes.

## Edit content

- `_data/site_settings.yml` — lab name, tagline, email, location, footer text.
- `_data/navigation.yml` — top navigation links.
- `_data/people.yml` — affiliated faculty, students, and alumni.
- `_data/projects.yml` — ongoing and past research projects.
- `index.md`, `people.md`, `projects.md`, `about.md`, `join.md` — editable page copy, including the regular lab meeting details on the homepage.

## Add images

Place headshots in `assets/img/people/` and update the `image` field in `_data/people.yml`. If an image is omitted, the people card automatically uses `assets/img/people/placeholder.svg`.

## Run locally

```sh
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.


## Styling

The site stylesheet is consolidated in `assets/css/style.css`. It keeps a Tufte CSS-inspired academic layout and typography, but uses system font stacks instead of missing vendored webfont files.

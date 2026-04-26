# RLS Log — Help Center

Public help center, FAQ, and policies for the [RLS Log iOS app](https://apps.apple.com).

This repo is published with **GitHub Pages** at:

> https://icweb.github.io/rls-log-help/

## What's here

| Path | Purpose |
| --- | --- |
| `index.md` | Landing page with cards linking to the rest. |
| `faq.md` | Frequently asked questions. |
| `contact.md` | Support email + bug-report guidance. |
| `privacy.md` | Privacy policy (linked from the App Store and the in-app HealthKit consent sheet). |
| `terms.md` | Terms of use. |
| `_layouts/default.html` | Custom Jekyll layout — sticky header, footer, page header. |
| `assets/style.css` | Single-file theme. Light/dark via `prefers-color-scheme`. |
| `_config.yml` | Jekyll config: title, nav, baseurl, kramdown settings. |

## Local preview

```sh
bundle install
bundle exec jekyll serve
```

Then open <http://127.0.0.1:4000/rls-log-help/>.

A minimal `Gemfile` is enough:

```ruby
source "https://rubygems.org"
gem "github-pages", group: :jekyll_plugins
```

## Editing content

Each Markdown page has YAML front matter. The layout is applied automatically
to every Markdown file (configured in `_config.yml` under `defaults`), so you
don't have to repeat `layout: default`.

```markdown
---
title: Page Title
subtitle: Optional one-liner under the title.
---
```

The header nav is driven by the `nav:` array in `_config.yml`. Add an entry
there to add a new top-level link.

## Deploy

GitHub Pages builds automatically on push to `main`. The first time you push
this repo, enable Pages under **Settings → Pages → Source → Deploy from a
branch → main / (root)**.

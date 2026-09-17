# bsubraya.github.io

Personal academic website for **Bhagya M. Subrayan** — Postdoctoral Research
Associate, Steward Observatory, University of Arizona.

Built with plain [Jekyll](https://jekyllrb.com/) on a custom theme (no external
theme gem), served by GitHub Pages.

---

## Editing the site

Almost everything you'll want to change lives in three places.

| I want to change… | Edit this |
| --- | --- |
| My name, title, address, email, profile links | `_config.yml` |
| Which CV the "CV" button downloads | `cv_url:` in `_config.yml` |
| The top navigation menu | `_data/navigation.yml` |
| Page content | the matching file in `_pages/` |
| Colours, fonts, spacing | `_sass/_variables.scss` |
| A plot, figure or animation | `_data/gallery.yml` |
| A talk, or slides attached to one | `_data/talks.yml` |

### Pages

| URL | File |
| --- | --- |
| `/` | `_pages/about.md` |
| `/research/` | `_pages/research.md` |
| `/publications/` | `_pages/publications.md` |
| `/talks/` | `_pages/talks.md` |
| `/mentoring/` | `_pages/mentoring.md` |
| `/outreach/` | `_pages/outreach.md` |
| 404 page | `_pages/404.md` |

Each page starts with a YAML front-matter block. `title` is the big heading,
`eyebrow` is the small accent label above it, `lede` is the intro paragraph, and
`description` is what Google and link previews show — worth writing properly.

### Common edits

**Post a new CV.** Drop the PDF in `files/`, then point `cv_url` in
`_config.yml` at it. That single line updates the header button, the footer link
and every "download CV" reference on the site.

**Add a publication.** Open `_pages/publications.md`, copy an existing
`<li class="pub">` block, and paste it at the *top* of the relevant list. The
year renders in the left gutter from `<span class="pub__year">`, so there is
nothing to renumber. Published and unpublished papers use identical markup —
for unpublished work just write "submitted" or "in preparation" in the
`pub__meta` line.

**Add a news item.** In `_pages/about.md`, find the `News & highlights`
section and copy a `<li>` block to the top of the `<ul class="timeline">`.

**Add a research project.** In `_pages/research.md`, copy a
`<section class="project">` block. Add `project--flip` to the class to put the
figure on the right instead of the left; use `project project--noimage` for a
text-only entry. Give it a unique `id` if you want to link to it directly.

**Add a plot, figure or animation.** Put the file in `images/` (or `files/`
for video), then add a block to `_data/gallery.yml`. It appears in the
*Plots & animations* section at the bottom of the Research page. Set
`plate: true` for figures with a white background — that adds a light mat so
matplotlib output doesn't glare against the dark page. `.png`, `.jpg`, `.gif`,
`.svg`, `.mp4` and `.webm` all work; MP4s autoplay muted and loop. If the list
is empty the whole section disappears, so it's safe to leave it that way.

**Add a talk, or attach slides to one.** Edit `_data/talks.yml`. Newest at the
top. To share a deck, drop the PDF in `files/` and add a `slides:` line — a
"Slides" button appears next to that talk. `poster:` and `video:` work the
same way.

**Add a student.** In `_pages/mentoring.md`: featured students get a
`<div class="mentor">` block with a photo (or an initials tile if you don't
have one yet); shorter engagements go in the `<div class="rows__item">` list
under *Also mentored*. Institution headings are `<span class="group-label">`.

**Turn on the personal photo strip.** `_pages/about.md` has a commented-out
`<div class="photostrip">` near the bottom. Add 2–3 landscape photos to
`images/`, update the filenames and captions, and delete the `<!--` / `-->`
markers around it.

### Images

Keep new images under roughly 1600 px wide and 300 KB. Photos on the outreach
page are letterboxed rather than cropped, so portrait and landscape shots both
work. Every `<img>` needs an `alt` description.

---

## Building locally

```bash
bundle install
bundle exec jekyll serve
# → http://localhost:4000
```

GitHub Pages rebuilds automatically on push, so local building is optional — but
it is the fastest way to check a change before it goes live.

---

## Structure

```
_config.yml          site settings, profile links, CV path
_data/
  navigation.yml     top navigation menu
  gallery.yml        plots, figures and animations (Research page)
  talks.yml          talks, with optional slides / poster / recording
_includes/
  head.html          <head>: meta tags, Open Graph, schema.org, analytics
  header.html        sticky site header + nav
  footer.html        site footer
  profile-links.html the row of icon buttons in the hero
  gallery.html       renders _data/gallery.yml
  talk-list.html     renders _data/talks.yml
_layouts/
  default.html       page shell
  page.html          standard interior page (title band + content)
  home.html          bare shell, used by the home page
_pages/              all page content
_sass/
  _variables.scss    colours, fonts, breakpoints — start here for restyling
  _base.scss         reset and base typography
  _layout.scss       shell, header, footer
  _components.scss   hero, cards, projects, publications, timeline, etc.
assets/
  css/main.scss      imports the partials above
  js/main.js         mobile nav toggle (the only JavaScript on the site)
files/               CVs and data downloads
images/              photos and figures
```

## Notes

- Dark theme: warm near-black surfaces (`#0d0f14`) with an ember accent.
  All the colours live in `_sass/_variables.scss`.
- No theme gem, no JavaScript framework, one small script for the mobile menu.
- Fonts are Newsreader (headings) and Inter (body), loaded from Google Fonts.
- Colour contrast meets WCAG AA throughout; if you change
  `_sass/_variables.scss`, re-check any greys against their backgrounds.
- **White-background figures** need `plate: true` in `_data/gallery.yml`, or
  the class `project__figure--plate` when placed inline on the Research page.
  Without it a white plot glares against the dark background.
- Analytics is Google Analytics, configured via `google_analytics` in
  `_config.yml`. Remove that line to switch it off.

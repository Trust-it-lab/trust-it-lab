# How to edit this website

This site is built from plain text files in this repository. You do not need to
know how to code — you edit a text file, save it, and the website rebuilds
itself within a minute or two.

**The easiest way to edit:** open the file on github.com, click the pencil
(✏️) icon at the top right, make your change, and click "Commit changes" at the
bottom. That is all — no software to install.

---

## The one rule

Most files start with a block between two lines of `---`, like this:

```
---
title: "Something"
date: 2026-01-15
---

The text of the page goes here.
```

The part between the `---` lines is **settings**. Keep the `word:` labels
exactly as they are and only change what comes after the colon. Everything
below the second `---` is **the text that appears on the page**, and you can
write it normally.

Any setting you leave blank is simply not shown on the site. It is always safe
to leave something empty and fill it in later.

---

## Where each thing lives

| To change this | Edit this |
|---|---|
| The name in the browser tab and top-left corner | `_config.yml`, the `title:` and `name:` lines near the top |
| The photo, bio, email and links in the left sidebar | `_config.yml`, the `author:` section |
| The front page text | `_pages/about.md` |
| Which tabs appear in the menu, and their order | `_data/navigation.yml` |
| Publications | files in the `_publications/` folder |
| News | files in the `_news/` folder |
| Teaching | files in the `_teaching/` folder |
| Team members | files in the `_team/` folder |
| Talks | files in the `_talks/` folder |
| Blog posts | files in the `_posts/` folder |
| CV | `_pages/cv.md` |

The `_news/` and `_team/` folders each contain a `README.md` with more detailed
instructions for that section.

---

## Changing the profile photo

The current photo is `images/ShafkatIslam.jpg`. To change it, either replace
that file with a new one of the same name, or upload a new file to `images/`
and update the `avatar:` line in `_config.yml` to match its filename.

On github.com: go into the `images` folder, click "Add file" → "Upload files".
A square image looks best, since the photo is displayed in a circle.

---

## Adding a publication

1. Go to the `_publications/` folder and copy any file that is already there.
2. Name your copy after the publication date, like `2026-04-01-my-paper.md`.
3. Fill in the settings at the top:

```
---
title: "The title of the paper"
collection: publications
category: manuscripts
permalink: /publication/2026-04-01-my-paper
excerpt: 'One sentence describing the paper.'
date: 2026-04-01
venue: 'Name of the journal or conference'
paperurl: 'https://link-to-the-pdf'
citation: 'How you want the citation to read.'
---
```

`category:` decides which heading the paper appears under. The three available
categories are `books`, `manuscripts` (shown as "Journal Articles") and
`conferences` (shown as "Conference Papers"). You can rename these headings or
add more in `_config.yml`, under `publication_category`.

`permalink:` must be different for every publication — the simplest approach is
to make it match the filename, as above.

To host a PDF on the site, upload it to the `files/` folder and then link to it
as `/files/the-file-name.pdf`.

---

## Adding a news item

Copy a file in `_news/`, rename it `YYYY-MM-DD-short-name.md`, and edit the
date, title, and text. Newest items appear at the top automatically. For a
one-line announcement with no heading, add `hide_title: true` under the
`title:` line.

---

## Adding a teaching entry

Copy a file in `_teaching/` and edit the settings at the top:

```
---
title: "Name of the course"
collection: teaching
type: "Undergraduate course"
permalink: /teaching/2026-spring-course-name
venue: "University, Department"
date: 2026-01-01
location: "City, Country"
---
```

The `date:` is used to sort entries, so use the start date of the course.

---

## Adding a team member

The Team page is a bulleted list of names. Copy a file in `_team/`, rename it,
and change the `name` and `order` lines. See `_team/README.md`.

---

## Removing a tab from the menu

Open `_data/navigation.yml` and delete (or comment out with `#`) the two lines
for that tab. Removing it from the menu does not delete the page — the content
stays in the repository and can be put back at any time.

---

## Things to clean up before sharing the site publicly

The template's example content has been removed. Two placeholder files remain,
kept deliberately as patterns to copy — replace them with real content:

- `_publications/2009-10-01-paper-title-number-1.md`
- `_teaching/2014-spring-teaching-1.md`

Still to fill in:

- `_pages/about.md` — the front page is still the template's own documentation
- `_pages/cv.md` — the headings are there, the content is not
- `_config.yml` — the `bio`, `location`, `employer`, `email` and the
  Google Scholar / ORCID links in the `author:` section

The Talks, Portfolio and Blog Posts tabs are empty: the pages and their
headings are in place, and entries appear as soon as files are added to
`_talks/`, `_portfolio/` and `_posts/`.

---

## If something breaks

Nothing is ever lost — every change is saved in the repository's history and can
be undone. On github.com, open the file, click "History", and you can view or
restore any earlier version.

The most common cause of a broken build is a typo in the settings block: a
missing `"` quote mark, or a line that lost its `:` colon. If the site stops
updating, look at the last file you edited.

---
# This file is documentation only - it is not shown on the website
# (the leading underscore in the filename below keeps items hidden, see note).
published: false
---

# How to add a news item

1. Copy the file `0000-00-00-example.md` in this folder.
2. Rename your copy using the date of the news, in the format
   `YYYY-MM-DD-a-short-name.md` — for example `2026-03-14-new-grant.md`.
3. Open your copy and edit the `date`, the `title`, and the text below the
   `---` line.
4. Save/commit. The item appears at the top of the News page automatically.

Nothing else needs to be edited — the News page finds these files on its own.

Items are sorted newest-first by the `date` field, so the date inside the file
is what matters for ordering (the filename is just for tidiness).

If you want an item with no heading — just a date and a line of text — add
`hide_title: true` below the `title:` line. (Jekyll fills in a title from the
filename when you leave one out, so this is how you switch it off.)

To remove a news item, delete its file.

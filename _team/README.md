---
# This file is documentation only - it is not shown on the website
published: false
---

# How to add or edit a team member

The Team page is a simple bulleted list of names. Each person is one file in
this folder, containing just two lines:

```
---
name: "Their Name"
order: 7
---
```

**To add someone:** copy any file here, rename it (for example `07-jane-doe.md`),
and change the `name` and `order`.

**To edit someone:** open their file and change the `name`.

**To remove someone:** delete their file.

`order` decides where they appear in the list — smaller numbers come first.
Renumbering is not required when you add someone; just give them a number
higher than the last person's.

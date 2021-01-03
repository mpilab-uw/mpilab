---
# Course title, summary, and position.
linktitle: Training and On-boarding for URAs
summary: test
weight: 1

# Page metadata.
title: Overview
date: "2018-09-09T00:00:00Z"
lastmod: "2018-09-09T00:00:00Z"
draft: false  # Is this a draft? true/false
toc: true  # Show table of contents? true/false
type: docs  # Do not modify.

# Add menu entry to sidebar.
# - name: Declare this menu item as a parent with ID `name`.
# - weight: Position of link in menu.
menu:
  example:
    name: Overview
    weight: 1

    example:
      name: TEST
      weight: 1
---

## Flexibility

This feature can be used for publishing content such as:

* **Online courses**
* **Project or software documentation**
* **Tutorials**

The `courses` folder may be renamed. For example, we can rename it to `docs` for software/project documentation or `tutorials` for creating an online course.

## Delete tutorials

**To remove these pages, delete the `courses` folder and see below to delete the associated menu link.**

## Update site menu

After renaming or deleting the `courses` folder, you may wish to update any `[[main]]` menu links to it by editing your menu configuration at `config/_default/menus.toml`.

For example, if you delete this folder, you can remove the following from your menu configuration:

```toml
[[main]]
---
# Display name
title: <Name Student>

# Is this the primary user of the site?
superuser: false

# Role/position
role: MASc, PhD, USRA, URA, Postdoc, Researcher

# Organizations/Affiliations
organizations:
- name: University of Waterloo
  url: "www.uwaterloo.ca"

# Short bio (displayed in user profile at end of posts)
bio:

interests:
- <list topics of scientific interest>

education:
  courses:
  - course: M.A.Sc. in Mechanical Engineering
    institution:  University of Waterloo
    year: 2019
  - course: B.Sc. in Mechanical Engineering
    institution: University of Waterloo
    year: 2018

# Social/Academic Networking
# For available icons, see: https://sourcethemes.com/academic/docs/page-builder/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.
social:
- icon: envelope
  icon_pack: fas
  link: '<add as needed>'  # For a direct email link, use "mailto:test@example.org".
#- icon: twitter
#  icon_pack: fab
#  link: https://twitter.com/GeorgeCushen
#- icon: google-scholar
#  icon_pack: ai
#  link: https://scholar.google.co.uk/citations?user=sIwtMXoAAAAJ
#- icon: github
#  icon_pack: fab
#  link: https://github.com/gcushen

# Link to a PDF of your resume/CV from the About widget.
# To enable, copy your resume/CV to `static/files/cv.pdf` and uncomment the lines below.
# - icon: cv
#   icon_pack: ai
#   link: files/cv.pdf

# Enter email to display Gravatar (if Gravatar enabled in Config)
email: ""

# Highlight the author in author lists? (true/false)
highlight_name: false

# Organizational groups that you belong to (for People widget)
#   Set this to `[]` or comment out if you are not using People widget.
user_groups:
-
---

<Enter short bio, 2 or 3 lines. Please write out thesis/research/primary domain of interest>
```

Or, if you are creating a software documentation site, you can rename the `courses` folder to `docs` and update the associated *Courses* menu configuration to:

```toml
[[main]]
  name = "Docs"
  url = "docs/"
  weight = 50
```

## Update the docs menu

If you use the *docs* layout, note that the name of the menu in the front matter should be in the form `[menu.X]` where `X` is the folder name. Hence, if you rename the `courses/example/` folder, you should also rename the menu definitions in the front matter of files within `courses/example/` from `[menu.example]` to `[menu.<NewFolderName>]`.

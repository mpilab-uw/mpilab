---
title: Updatewebsite
linktitle: Tips for researchers
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
menu:
  example:
    parent: Training
    weight: 1

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 1
---
The MPILAB maintains a website to promote the research activities in the lab. It's everyones responsibility to maintain this information as up-to-date as possible. The website is maintained in a <a href="https://github.com/mpilab-uw/mpilab.git">github repository</a> and hosted on <a href="https://netlify.com">netlify.com</a>. The information for the team members are located '/mpilab/content/authors/' in a folder with name 'lastname_firstname'. In each folder


## Easy guide to update website
To update your website, please:
- cut-paste the following and modify accordingly and save as " _index.md "
- select a picture of yourself and save as " _index.md "
Send both " _index.md " and " _index.md " to JPH.

```toml
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

---
title: Useful tips
linktitle: Tips 1-2
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
menu:
  example:
    parent: Example Topic
    weight: 1

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 1
---

#Jupyter
To used Jupyter as a server, on the remote machine:
```toml
>>> jupyter notebook --no-browser --port=8888
```

On the local machine:
```toml
>>> ssh -N -f -L localhost:8888:localhost:8888 <username>@192.168.1.24
```

---
title: Example Page 1
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

In this tutorial, I'll share my top 10 tips for getting started with Academic:


Then to compile the code you need to go the the code directoy and run:
$ . sourceme.sh
Then go to the sim directory and run:
$ pc_setuprc
$ pc_build -f GNU-GCC_MPI

If you have all the required files, the file linking and compilation should be done successfully.

Then you can submit a job as in "Chan-Rings.sh"
if you run it on debug nodes, you can use the commands:
$ ./start.csh (To initialize)
$ ./run.csh (To run)
$ ./start_run.csh (to initialize and run)

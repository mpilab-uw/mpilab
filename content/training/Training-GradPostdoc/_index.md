---
# Course title, summary, and position.
linktitle: Training and On-boarding for URAs, Graduate Students and Postdocs
summary: Provides key information about on-boarding in the MPILAB at the University of Waterloo
weight: 1

# Page metadata.
title: On-boarding
date: "2018-09-09T00:00:00Z"
lastmod: "2018-09-09T00:00:00Z"
draft: false  # Is this a draft? true/false
toc: true  # Show table of contents? true/false
type: docs  # Do not modify.

# Add menu entry to sidebar.
# - name: Declare this menu item as a parent with ID `name`.
# - weight: Position of link in menu.
menu:
  Test_1:
    name: Training
    weight: 1
---

## Summary
This guide is meant to help you start your journey as a new  URA, USRA, grad student, or postdoc in the MPILAB at the University of Waterloo.


## Getting started
* **Follow the <a href="https://uwaterloo.ca/graduate-studies-postdoctoral-affairs/new-students">on-boarding</a> from UW (grad students/postdoc only)**
* **Website update:** download the <a href="https://www.dropbox.com/s/0h55d91qzyn22j3/_index.md?dl=0">template</a> fill-out the form (not in Word!) and upload the  completed form and mugshot <a href="https://www.dropbox.com/request/ZJrZzIxT4r91ewNBu7Tn">here</a>
* **Open a Compute Canada Account (only if needed)**: follow the detailed steps <a href="https://www.computecanada.ca/research-portal/account-management/apply-for-an-account/">here</a>. If you do open a Compute Canada account, you MUST follow the Compute Canada training.
* **Open a Gitlab account**: UW has an on-site Gitlab repository which is actively used. Request access <a href="https://git.uwaterloo.ca/users/sign_in">here</a>.
* **Open an Overleaf account**: UW has a site licence to Overleaf which is used for writing. Open an account <a href="https://www.overleaf.com">here</a>.
* **Familiarize yourself with the terminal**: Most of the work we do will be using the terminal. Need to get used to it. If you are a Mac/Linux user, the terminal is directly integrated. If you are a Windows users, you can use the <a href="https://docs.microsoft.com/en-us/windows/wsl/install-win10">Windows Subsystem for Linux</a> which provides you with a linux terminal. If you are new to the terminal,
<a href="https://ubuntu.com/tutorials/command-line-for-beginners#1-overview">take a 1h tutorial.</a>

## Communication
The main communication within the group is done through our google group. We also have an active Slack channel for quick discussions/questions. You can join both:
* **Slack channel:** mpilab-workspace.slack.com
* **Email group serve:** mpilab@googlegroups.com


## Research Tools
### Organization and writing
Familiarize yourself with a number of tools used to facilitate the research

* **Git**: A version management system. Each project will has a dedicated Git repository. The repository is used to store all related work for a project (reference papers, drafts, weekly reports, figures etc). Typically, numerical codes will be housed in their own repository. Raw results are not stored in the repo. It allows for multiple users and allows for a dated backup. Please ensure to push daily. <a href="http://rogerdudler.github.io/git-guide/To">learn more about git</a>.
* **Latex**: Latex is a standard typesetting standard used in scientific communication. To learn more about latex typesetting, <a href="https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes">take this 30 minute tutorial</a>.
* **Reference management**: To keep track of the references used for your research, a good reference management tool is helpful. These tools allow you to drag-and-drop pdfs to extract the meta-information (title, authors, etc.) and can be integrated into Overleaf. We primarily use  <a href="https://www.mendeley.com">Mendeley</a> although <a href="https://www.zotero.org">Zotero</a> is also used.
* **Vector graphics**: For illustrations and vector graphics, we use <a href="https://inkscape.org">Inkscape</a>. A short tutorial can be found <a href="https://inkscape.org/learn/tutorials/">here</a>.

### Coding
Coding is always just around the corner. Sometimes the coding involves extending open-source software, although most of the time its used for post-processing (e.g. figure generation).
* **<a href="https://docs.conda.io/en/latest/">Python</a>**: Python is our go-to tool. Even if most operating systems come with a pre-installed  version of python, it's advised to install the python via the Conda environment system. For figures, we generally rely on the <a href="https://anaconda.org/anaconda/matplotlib">matplotlib package</a> which is trivially installed with Conda.



### CFD solvers
We use a number of CFD tools. Some of these tools are in-house (see our UW git repo), some are open-source.

* **<a href="https://su2code.github.io">SU2</a>**: Unstructured CFD code. Our workhorse for industrial project and complex geometries.
* **<a href="https://www.openfoam.com">OpenFoam</a>**: Highly versatile CFD package for multi-physics problems.
* **<a href="http://pencil-code.nordita.org">Pencil code</a>**: Academic code used in our group for particle-laden turbulent flows.
* **Basilik**
* **<a href="https://palabos.unige.ch">Palabos</a>**: general-purpose computational fluid dynamics (CFD), with a kernel based on the lattice Boltzmann (LB) method. It is used in our group for porous flow simulations.
* **<a href="http://openpnm.org">OpenPNM</a>**: Although formally not a CFD solver, this tool permits pore network modeling for porous media flows.



### Visualization tools
For three-dimensional Visualizations, we primarily focus on two tools:
* **<a href="https://wci.llnl.gov/simulation/computer-codes/visit">VisIt</a>**
* **<a href="https://www.paraview.org">Paraview</a>**


### Grid generation
For mesh generation, we use the following tools depending on the task:
* **<a href="https://cfd.direct/openfoam/user-guide/v6-blockmesh/">BlockMesh</a>**: BlockMesh is a meshing tool for structured grids which is part of the OpenFoam framework. It provides the highest level of user control. It may also be the most challenging for complex geometries.
* **<a href="https://gmsh.info">Gmsh</a>**: Permits structured and unstructured mesh generation. It's an open source tool and can be downloaded locally. Outputs are compatible with SU2, OpenFoam and other tools.
* **<a href="https://www.pointwise.com">Pointwise</a>**: the group has an academic licence to this software. The licence can be accessed through our MME licence server on campus.



## Computer systems
Storage  NAS
Computer usage
Compute Canada
git repository

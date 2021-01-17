---
# Course title, summary, and position.
linktitle: Palabos
summary:  <a href="https://palabos.unige.ch"> downloaded here</a>
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
---

## Installing on Niagara
Git clone from the git repo:
```toml
git clone https://gitlab.com/unigespc/palabos.git
```
You will need to load the following modules:
```toml
module load cmake  gcc/9.2.0 openmpi/4.0.3
```
To run a sample tutorial case, simply:
```toml
$ cd palabos/examples/showCases/cavity2d/build
$ cmake ..
$ make
$ cd ..
$ ./cavity2d
```

## Understanding the code
The first starting point in understanding the code is in this article
<a href="https://reader.elsevier.com/reader/sd/pii/S0898122120301267?token=B5B25552F55F42F61ACD08A96EF4654600D5B4CCC04C05A210EF20F0DF475380AA064E3C3F1F8A9DCDFA3D310B0B979B">: Latt et all. Computers and Mathematics Applications (2021)</a>.

A good summary of the LB theory can be found here: <a href="https://www.youtube.com/watch?v=I82uCa7SHSQ"> youtube tutorial</a>

Some slightly more accessible documentation can be found in additional MASc theses such as : <a href="https://digitalcommons.lsu.edu/cgi/viewcontent.cgi?article=4219&context=gradschool_theses"> this </a>.

There is a Palabos wiki cite on <a href="https://www.cfd-online.com/Wiki/Palabos">CFD Online</a>.

To get your hands dirty, start by completing the <a href="https://palabos.unige.ch/get-started/palabos-tutorial/">tutorials</a>.



## Citation for work:
```toml
@article{Palabos2020,
    title = "Palabos: Parallel Lattice Boltzmann Solver",
    journal = "Computers & Mathematics with Applications",
    year = "2020",
    issn = "0898-1221",
    doi = "https://doi.org/10.1016/j.camwa.2020.03.022",
    author = "Jonas Latt and Orestis Malaspinas and Dimitrios Kontaxakis and Andrea Parmigiani and Daniel Lagrava and Federico Brogi and Mohamed Ben Belgacem and Yann Thorimbert and Sébastien Leclaire and Sha Li and Francesco Marson and Jonathan Lemus and Christos Kotsalos and Raphaël Conradin and Christophe Coreixas and Rémy Petkantchin and Franck Raynaud and Joël Beny and Bastien Chopard",
}
```

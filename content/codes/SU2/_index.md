---
# Course title, summary, and position.
linktitle: SU2
summary:  
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
    name: SU2
    weight: 1
---

## Using Code
Download the code. (This is for member only)
```toml
git clone https://github.com/su2code/SU2.git
```

On Niagara, you can load the following modules:
```shell
module purge
module load NiaEnv/2018a
module load intel/2018.2  intelmpi/2018.2 anaconda3/5.2.0
```

Installation is then straight forward
```shell
git clone https://github.com/su2code/SU2.git # Clone repository to HybridX
mkdir SU2_Build # Create build directory
cd SU2_Build # Enter build directory
./meson.py build --prefix ~/SU2_Build/ # Launch CMake to generate the build files
./ninja -C build install # Build (compile/link) the software with 8 processes in parallel
```

If you have not changed anything in the above inputs, you need to set the path to the library:
```shell
export SU2_RUN="<your_prefix>/bin"
export SU2_HOME="<your_prefix>/SU2/"
export PATH=$PATH:$SU2_RUN
export PYTHONPATH=$SU2_RUN:$PYTHONPATH
```

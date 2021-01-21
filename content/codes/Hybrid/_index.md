---
# Course title, summary, and position.
linktitle: HybridX
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
    name: Hybrid
    weight: 1
---

## Using Code
Download the code. (This is for member only)
```toml
git clone https://gitlab.com/HybridX.Suite/HybridX.git
```

On Niagara, you can load the following modules:
```shell
module load cmake intel/2019u4 intelmpi/2019u4 boost/1.70.0
```

For some reason, the links to the MPI library are not correctly found by the code, so we need to explicitly state them (the path will change if we change modules!):
```shell
export MPI_LIBRARY="/scinet/intel/2019u4/compilers_and_libraries_2019.4.243/linux/mpi/intel64/lib/"
export MPI_INCLUDE_PATH="/scinet/intel/2019u4/compilers_and_libraries_2019.4.243/linux/mpi/intel64/include/"
```
Installation is then straight forward
```shell
git clone https://gitlab.com/HybridX.Suite/HybridX.git # Clone repository to HybridX
mkdir HybridX_Build # Create build directory
cd HybridX_Build # Enter build directory
cmake ../HybridX # Launch CMake to generate the build files
gmake -j8 # Build (compile/link) the software with 8 processes in parallel
gmake install
```

If you have not changed anything in the above inputs, you need to set the path to the library:
```shell
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/home/j/jphickey/jphickey/HybridX_build/install/lib
```

Then please the full path to your binary when running:
```shell
mpirun -np 40 /home/j/jphickey/jphickey/HybridX_build/install/bin/Hybrid -i uniform3.input
```

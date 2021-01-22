---
# Course title, summary, and position.
linktitle: PencilCode
summary:  <a href="https://github.com/jmreppsUWGrad/2D-Nanothermite"> downloaded here</a>
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

## Using the pencil python scripts (Niagara)
To use the python scripts on Niagara, you can load the following modules (NiaEnv 2019b):
```toml
module load gcc/9.2.0 openmpi/4.0.3 python/3.8
```
To start a virtual environment and load the desired libraries, you need :
```toml
mkdir ~/.virtualenvs
cd ~/.virtualenvs
virtualenv --system-site-packages ~/.virtualenvs/pencil
```
Now that you have created a virtual environment, you can activate it:
```toml
source ~/.virtualenvs/pencil/bin/activate
```

To run the code, you need to set a couple things:
```toml
export PENCIL_HOME=~/pencil-code
source ./pencil-code/sourceme.sh
```

Now we can install the needed libraries:
```toml
pip install h5py
pip install plotly
pip install  tqdm
pip install  mpi4py
pip install vtk
```
Now, you can go to a




## Using Code
No, I didnt create a specific file to use pencil on niagara.
I am currently using gcc/9.2.0 and openmpi/4.0.3. (after the new update)

Please check the files in /scratch/theta_analysis/ for the new simulations.
In Summary, you need these files to run a simulation:
* run.in
* start.in
* print.in
* src/cparam.local
* src/Makefile.local
* data/ (empty directory)
* initial_condition/some_file.F (If you need to run specific IC, like in our case)

Then to compile the code you need to go the the code directoy and run:
* $ . sourceme.sh
Then go to the sim directory and run:
$ pc_setuprc
$ pc_build -f GNU-GCC_MPI

If you have all the required files, the file linking and compilation should be done successfully.

Then you can submit a job as in "Chan-Rings.sh"
if you run it on debug nodes, you can use the commands:
$ ./start.csh (To initialize)
$ ./run.csh (To run)
$ ./start_run.csh (to initialize and run)

Please let me know if it still fails.
For the new cases, they started running this afternoon, the queue time was one day!


## Installation on niagara
```toml
git clone https://github.com/pencil-code/pencil-code.git
cd pencil-code
. sourceme.sh
```

In the new environment, I did:
```toml
module load gcc/9.2.0
```

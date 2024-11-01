---
title: Installing
sidebar: mydoc_sidebar
permalink: installing.html
folder: mydoc
---

The Duke Computing Cluster(DCC)'s user manual can be found [here](https://oit-rc.pages.oit.duke.edu/rcsupportdocs/dcc/).

### Connecting

To connect to the DCC simply enter the following into a terminal with SSH installed:

```bash
username@dcc-login.oit.duke.edu
```

Replace `username` with your DukeID. This connects the current terminal to a login node.

DO NOT RUN SIMULATIONS ON THE LOGIN NODE.

The login node is shared by all users and intended for minor tasks only. To run intensive tasks, set up a job script as described in the user manual.

### Important directories

A file system overview can be [found here](https://oit-rc.pages.oit.duke.edu/rcsupportdocs/dcc/files/#overview).

Your home directory has limited storage. There is more storage in the labs folder, `/hpc/group/dolbowlab/`. Make a directory there with the name of you DukeID. Use this for storage.

Additionally, make a folder in the `/work/` directory with the same name.

### The dolbowlab Partition

Our lab owns a node on the DCC that is only accessible by lab members. It only has 78 cores so it can easily get clogged up if multiple lab members are using it. The reset of the DCC is still accessible the lab node is full.

### Installing RACCOON on the DCC

Normally on an HPC, you would use the [https://mooseframework.inl.gov/getting_started/installation/hpc_install_moose.html](instructions) to install MOOSE on an HPC. Due to some missing packages, RACCOON needs to be installed using the typical conda installation.

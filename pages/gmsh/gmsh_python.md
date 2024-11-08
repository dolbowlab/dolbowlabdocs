---
title: Python
tags: [getting_started]
summary: "Setting up using python"
sidebar: mydoc_sidebar
permalink: gmsh_python.html
folder: mydoc
---

## Installation

I recommend using conda to install the Python GMSH API

To install, first create a new conda env (assuming you have Conda installed)

```bash
conda create --name gmsh
conda activate gmsh
```

Now install the API

```bash
conda install conda-forge::python-gmsh 
```

## Usage

It recommened to read the tutorials found on the [GMSH manual](https://gmsh.info/doc/texinfo/gmsh.html#Gmsh-tutorial).
The python implementation of each tutorial can be found by clicking the python link under each tutorials name. 
![pylink](images/gmsh/pylink.png)

### Examples

In general your scripts will always start/end with 

```python
import gmsh
import os
import sys

gmsh.initialize()
gmsh.model.add("modelname")

# Code goes here

gmsh.write(
    "filename"
)


if "-nopopup" not in sys.argv:
    gmsh.fltk.run()

gmsh.finalize()
```

Important concepts
- [Size fields](https://gmsh.info/doc/texinfo/gmsh.html#t10)
- [Embedded geometry](https://gmsh.info/doc/texinfo/gmsh.html#t15)
- [Boolean Operations](https://gmsh.info/doc/texinfo/gmsh.html#t16)
- [Transfinite Meshes](https://gmsh.info/doc/texinfo/gmsh.html#t6)

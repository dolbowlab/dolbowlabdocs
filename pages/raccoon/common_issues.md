---
title: Common Issues
sidebar: mydoc_sidebar
permalink: common_issues.html
folder: raccoon
---

## Compilation errors and non-registered objects

It is common to run into issues with compilation after updating MOOSE/RACCOON or when swapping out submodules. 

Commonly, running a git clean will fix most issues. 

```bash
git submodule foreach --recursive git clean -xfd #cleans MOOSE and all of its submodules
git clean -xfd #cleans RACCOON
```

This will remove everything that is not tracked by git. **MAKE SURE YOU HAVE EVERYTHING YOU WANT TO KEEP COMMITED**. 

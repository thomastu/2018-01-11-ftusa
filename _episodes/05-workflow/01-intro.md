---
title: "Workflow"
teaching: 10
exercises: 5
questions:
- "How do we write code for operational use?"
objectives:
- "Integrate git flow with working objectives."
keypoints:
- "You can test code locally in an interactive environment like jupyter notebook"
- "Moving code to a version controlled python package enables sharing."
---

# Python Packaging

## The setup.py File

Putting a setup.py file will instruct the "pip" program to try and install your local package.  This will get installed with the specified 


```
from setuptools import setup

setup(
    name="my_package_name",
    version="1.0.0",
    install_requires=["pandas", "sqlalchemy", "mycli"],
)
```

## Installing Packages

The `pip install` syntax is given by `pip install <location_of_package>`.
You can install both local and remote packages.
Pip will try to find packages in the following order if not location protocol is specified : 

1.  PyPi
2.  Custom configured PyPi servers
2.  Your current working directory

```
pip install -e .
```

> ## Create and Install a Package
>
> 1. Create a setup.py file for your python package
> 2.  Install your package with pip
{: .challenge}

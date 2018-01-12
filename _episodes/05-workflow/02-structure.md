---
title: "Structuring Local Software"
teaching: 10
exercises: 5
questions:
- "What is the structure of a python package?"
- "What is the structure of a python script?"
objectives:
- "Separate analysis and process code"
- "Figure out the difference between a package and a script."
keypoints:
- "Python works well both interactively and with configured libraries."
---

# Cookiecutter Projects

Cookiecutter is a python program that enables you to quickly spin up projects from a preconfigured package.

- [cookiecutter](https://github.com/audreyr/cookiecutter)
- [Cookiecutter python](cookiecutter https://github.com/audreyr/cookiecutter-pypackage.git)

This will enable you to create a template project that can be imported in an interactive environment.

# Python Packages

A python package is simply a collection of python modules which can be used in other scripts or in an interactive environment.

## Submodules

Submodules are simply additional folders in your project which are made available with the "dot" syntax (e.g. `pandas.DataFrame.index`)

## Namespaces

How are package namespaces resolved?

# Python Scripts

A script is simply a single file which is meant to be run interactively in a shell.  It can be given to a progam such as crontab to run automatically, or passed around in version control for someone to run manually.
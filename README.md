# r-binder-template

A template repository for binderising one off R notebooks for workshops and training.

This repository is intended as a compact template for deploying one off
notebooks and training materials for customised workshops. Frequently run
tutorials and maintained notebooks might be better off in the
[interactive notebooks](https://github.com/SLCLADAL/interactive-notebooks) 
repository instead.


# Usage

1. Click the "Use this template" in the GitHub web UI to create a new repository
with these skeleton elements for binderisation.
2. Choose the R version and put it in runtime.txt in the format: `r-a.b.c-YYYY-MM-DD`
where a.b.c is the R version number and YYYY-MM-DD is a snapshot date for packages.
3. Specify R dependencies in install.R, using standard R installation syntax: `install.packages('dplyr')`
4. Specify systems dependencies in apt.txt, with one line per package and the required package name
5. Whack your notebook (either ipynb or Rmd) and associated small data files in the repo. 
	- For a single jupyter notebook this might just be at the root of the repo
	- You might want to put data files in a data subfolder
	- If you want to share a few notebooks in the same repo, it might be better to 
	  place in a notebooks subfolder 
6. Customise the readme and description as appropriate.



---
title: My Reproducible project workflow
date: 2020-03-10T10:13:37.014Z
template: post
---
I will first 

* introduces ways to organise files on your computer and to document your workflows.
* how to make your code more reproducible and readable
* how to write reproducible reports.
* the basics of version control.
* how to archive your code. 

## Organising projects for reproducibility

I embrace a one folder = one project mentality. Rstudio's "R projects" are excellent for encouraging this. This habit enables easy communication with other project stakeholders and for that reason it is so important.

Make sure to use ISO 8601 format (YYYY-MM-DD) to avoid confusion between differing local dating conventions.

Choose filenames so that alphabetical sorting will organise types of files for you: in the same way that ISO 8601 puts the most significant unit (year) first so that alphabetical = chronological.

Avoid using absolute paths and use only relative paths. An absolute path is one that gives the full address to a folder or file. A relative path gives the location of the file from the current working directory. 

For example:

```
# Absolute path -----------------------------
“C:/project_root_folder/data/species_dat.csv”

# Relative path ------
“data/species_dat.csv”
```

When working in R, RStudio projects can help aid portability of code. RStudio projects provide a self-contained coding environment to work in, and when opened, a \`.Rproj\` file sets the project working directory and saves the history and state of the project. RStudio projects can be created directly from the RStudio GUI and can be created in an existing folder, a new empty folder, or checked out from a version control repository 

## Programming

### Writing functions

how to define your own functions in R and in Python:

```
# Create a user-defined function in R:
square_number <- function(base){         square <- base*base         return(square)}# Calling a user-defined function in Rsquare_number(5)
```

```
# Create a user-defined function in Python:
def square_number(base):      
square = base*base      return(square)

# Calling a user-defined function in Python:
x_square = square_number(5)
```

### Show the packages used

With R, the simplest (but a useful and important) approach to document your dependencies is to report the output of `sessionInfo()` (or `devtools::session_info()`). Among other information, this will show all the packages and their versions that are loaded in the session you used to run your analysis. If someone wants to recreate your analysis, they will know which packages they will need to install.
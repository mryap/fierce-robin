---
title: My Reproducible project workflow in R
date: 2020-03-10T10:13:37.014Z
template: post
---
### Organising projects for reproducibility

I embrace a one folder = one project mentality. Rstudio's "R projects" are excellent for encouraging this. This habit enables easy communication with other project stakeholders and for that reason it is so important.

Make sure to use ISO 8601 format (YYYY-MM-DD) to avoid confusion between differing local dating conventions.

Choose filenames so that alphabetical sorting will organise types of files for you: in the same way that ISO 8601 puts the most significant unit (year) first so that alphabetical = chronological.

Avoid using absolute paths and use only relative paths
An absolute path is one that gives the full address to a folder or file. A relative path gives the location of the file from the current working directory. 
For example:
# Absolute path -----------------------------“C:/project_root_folder/data/species_dat.csv”
# Relative path ------“data/species_dat.csv”


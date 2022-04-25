This page is a fork of the [al-folio academic theme](https://github.com/alshedivat/al-folio). Follow general installation/development instructions there.

The table in home reads data from `_csv/table.csv`, modify that file for any updated information about the datasets.  
The papers page is generated automatically reading the `_bibliography/papers.bib` file. Papers can be added by adding a bibentry which includes a `language` key, so that it is added to the list of that language.
To add a new language, the languages array in the header of `_pages/publications.md` needs to be modified to include it.

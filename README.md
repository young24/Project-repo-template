# Project-repo-template
A template for project repositories

## Code folder
For the code folder, source files can be uploaded directly to GitHub. However, generated objects (e.g., .o), compressed objects (e.g., .zip) and large data files (e.g., .avi, .yaml) should not be placed in this folder, and they would not be uploaded to GitHub.

Test data files should be placed in the Data folder.

## Data folder
For the Data folder, all files will be uploaded as LFS objects. If you don't want some data being uploaded to GitHub, you can save them in the Working folder or save them on a server and put a link in the data folder.

## Docs folder
For the Docs folder, except for markdown files, all the files will be uploaded to GitHub with Git-LFS (large file storage)). You need to manually pull those files when you need them.
```
git lfs pull -I'PATH/FILENAME'
```

## Results folder
For the results folder, we designed this folder to only hold those finalized results for publications. Intermediate results such as analysis results should be placed in the Data folder which can auto-sync with server.
In this folder, binary files such as MS Office files will be uploaded to GitHub with Git-LFS (large file storage). You need to manually pull those files when you need them.
```
git lfs pull -I'PATH/FILENAME'
```

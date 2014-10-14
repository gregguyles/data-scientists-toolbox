# Git Notes: Week 2

## Creating a Repo
- Create Rep on GitHub GUI, OR
- Initialize the current directory as a git repo
    - `git init`
- Point local repo at the remote repo
    `git remote add origin https://<someURL>.git`
- If you create via GitHub GUI then clone the repo from GitHub
    `git cone https://<someURL>.git`

## Adding files to version control (do this before committing)
- Add all new files
    - `get add .`
- Updates tracing for all files that changed names or were deleted
    - `get add -u`
- Do both previous
    - `get add -add`

## Committing
- Commit and provide a useful description (-m) of what you did
    - `git commit -m "message"

## Pushing (from local repo to remote)
- `git push <remoteRepo> <branch>`
- `git push origin master`

## Branches - create a new repo of exisitng code
- create a new branch
    - `git checkout -b <branchName>`
- see what branch you are on
    - `git branch`
- switch back to master
    - `git checkout master`

## Pull Request - Git Hub feature, select via GUI
- Select "compare and pull request"
- Submits a request for your changes to be merged into the master
- The repo owner will decide to merge or not

## Markdown Notes
- Markdown files have the .md extension

\# Heading
\#\# Secondary heading
\#\#\# Tertiary

\* first item in list
\* second item
\* third item in list

## R packages
- CRAN or Bioconductor Project
- View available packages
    - 'a <- available.packages()'
- Install the "slidify" R package
    - `install.packages("slidify")`
- You can also install from RStudio
    - '''Tools > Install Packages'''

## Bioconductor install
- Install Bioconductore 
    -`source("http://bioconductor.org/biocLite.R")`
    - `biccLite()`
- Install a bioconductor package
    - biocLite(c("GenomicFeatures", "AnnotationDBi"))

## Loading R Packages
- function used to load packages
    - `library(<package_name>)`
- i.e. Load "ggplot2"
    - libary(ggplot2)
- Type `search()` to view the functions associated with the package
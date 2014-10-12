Git Notes:

Creat Rep on GitHub GUI
git init                # initilize the currnt Dir as a get repo
git remote add origin https://<someURL>.git         # point local repo at the remote repo

For Repon on GitHub GUI
git cone https://<someURL>.git              # copy a remote repo

# Adding to VC
get add .                   # add all new files
get add -u                # updates tracing for all files that changed names or were deleted
get add -add            # does both previous
# do this befoe committing

# Committing
git commit -m "message"         # where message is a usefull description of what you did

# Pushing (from local repo dir)
git Push        # push to remote

# Branches - create a new repo of exisitng code
git checkout -b branchname          # create new branch
git branch                                         # see what branch you are on
git checkout master                         # switch back to master

# Pull Requiest - Git Hub feature
select compare and pul request 
the auther will decide to merge or not 

# Markdown Notes

.md

# Heading
## Secondary heading
### Tertiary

* first itme in list
* second item
* third item in list

# R packages
* CRAN or Bioconductor Project
* 'a <- available.packages()''
Install the "slidify" R package
`install.packages("slidify")`
Can also install from RStudio
'''Tools > Inatall Packages'''

## Bioconductor install
### Install Bioconductore 
source("http://bioconductor.org/biocLite.R")
biccLite()

### Install a bioconductor package
biocLite(c("GenomicFeatures", "AnnotationDBi"))

### Loading R Packages
`libary()`          - function used to load packages
Load "ggplot2"
    libary(ggplot2)
The type `search()` to view the functions associted with the package
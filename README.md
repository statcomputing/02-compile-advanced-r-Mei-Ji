Assignment 2 requirement

Use git to clone the source of Hadley Wickham’s Advanced R Programming from his GitHub repository to a local space on your own computer. Build the book using RStudio. During the building process, you may see error messages due to missing tools on your computer. Read the error messages carefully and fix them, until you get the book built. You may need to install some R packages, some fonts, some latex packages, and some building tools for R packages. On Windows, some codes for parallel computing may not work and need to be swapped out. Document your computing environment (operating system, R/RStudio, Shell, etc.) and the problems you encountered, as well as how you solved them in an R Markdown file named README.Rmd. Push it to your homework GitHub repository so that it can help other students to build the book.

download R, RStudio
using git clone down adv-p, install packages bookdown,then follow the instruction built book.


Missing packages:
lobstr [install.packages("lobstr")]
emo [devtools::install_github("hadley/emo")] Notice: if you do not have devtools package before, install devtools packages first
sloop [install.packages("sloop")]
DBI [install.packages("DBI")]
RSQLite [install.packages("RSQLite")]
zeallot [install.packages("zeallot")]
dbplyr [install.packages("dbplyr")]
profvis [install.packages("profvis")]
bench [install.packages("bench")]
ggbeeswarm [install.packages("ggbeeswarm")]


unexpected question:

1: If I download bookdown through github, when I call install.package('bookdown') will go to a loop shows updating loaded packages.

solve: use code find the bookdown package and delete that package. then directly install package within Rstido

2; When I use git push, although the terminal shows everything up to date, the assigement page still only have readme.md file. After several tried I still not fixed this question. I can successful build book into gitbook and pdf book. However the website did not show. I have to upload every file I have. And some file are actually hiden which I can not upload.


result:
get _main.pdf

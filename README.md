# DynafluxR notebook

## Overview

DynafluxR is a software for dynamic metabolic flux analysis and is available from [this repository](https://github.com/MetaSys-LISBP/DynafluxR).

DynafluxR can be used as an R package that you can import directly, for instance in [R Markdown notebooks](https://rmarkdown.rstudio.com/lesson-10.html) or in your own software.

We showcase DynafluxR usage with step-by-step examples in a R Markdown notebook distributed via this repository. We also distribute an HTML file showing the [notebook’s output after execution](https://htmlpreview.github.io/?https://github.com/MetaSys-LISBP/DynafluxR_notebook/blob/main/html/notebook.html).

This R code perform all analyses detailed in the following publication:

> Estimating flux dynamics from time-course metabolite concentrations with dynafluxr.
>
> Sokol S., Dubiley S., Rouan P., Charlier C., Lippens G., Millard P. bioRxiv preprint, 2025, doi: [XXXX/XXXX](https://doi.org/XXXX/XXXX)

Details on the calculations can be found in the publication and in the Rmd notebook.

The code is open-source and available under [GPLv3 license](https://www.gnu.org/licenses/gpl-3.0.txt).

## Installation and usage

If not yet done, download and install [Rstudio](https://posit.co/downloads/).

Some required dependencies are specific to our notebook, not to DynafluxR itself.

`RColorBrewer`, `stringr`, and `vioplot` can be installed
by running the following command in the Rstudio console:

```bash
install.packages(c("RColorBrewer", "stringr", "vioplot"))
```

`CoRC` can be installed
using the following commands:

```bash
install.packages("remotes")
library(remotes)
remotes::install_github("jpahle/CoRC")
library(CoRC)
CoRC::getCopasi()
```

Additional information on CoRC installation and usage are available from the CoRC repository (https://github.com/jpahle/CoRC) and the associated publication (Föster et al., Bioinformatics, 2021, doi: [10.1093/bioinformatics/btab033](https://doi.org/10.1093/bioinformatics/btab033)).

## Usage

To run all analyses detailed in the publication and reproduce Figures 2 and 3:

- download the [GitHub repository tarball](https://github.com/MetaSys-LISBP/DynafluxR_notebook/archive/refs/heads/master.zip) and unpack it somewhere on your disk

- start RStudio

- open the file `./notebook.Rmd`

The notebook will open in Rstudio, in each cell you can read/modify/execute the code as well as read accompanying comments.

## Questions

If you have any question, please open a new *issue*
to [our GitHub issue tracker](https://github.com/MetaSys-LISBP/DynafluxR_notebook/issues) so we could discuss together.

## How to cite

Serguei Sokol, Svetlana Dubiley, Pauline Rouan, Cyril Charlier, Guy Lippens, Pierre Millard. Estimating flux dynamics from time-course metabolite concentrations with dynafluxr. bioRxiv preprint, 2025.

## Authors
Sergueï Sokol, Pierre Millard

## Contact
:email: sokol@insa-toulouse.fr, pierre.millard@insa-toulouse.fr
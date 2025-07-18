# Retrieving reaction rate dynamics from specie kinetics (dynafluxr results)

This is the result files produced by dynafluxr R package (v0.26.0) on 2025-06-10 21:38:47 +0200 (CEST).

The command to reproduce these results is:

`Rscript --vanilla -e 'dynafluxr::cli()' "-m" "C:/Users/millard/Documents/GIT/dynafluxr_notebook/repo/DynafluxR_notebook/toy_model/results/tmp/tmp_2.txt" "-s" "C:/Users/millard/Documents/GIT/dynafluxr_notebook/repo/DynafluxR_notebook/toy_model/network.txt"`

## File contents

 - `specie.pdf`: concentration plots (fitted by B-spline);
 - `ispecie.pdf`: estimated concentration plots vs Time (by integration of *S·v*);
 - `rate.pdf`: estimated rate plots (by solving least squares);
 - `flux.pdf`: estimated total fluxes (S*v) plots (by solving least squares);
 - `resid.pdf`: residuals *dm/dt - S·v* plots;
 - `specie.tsv`: concentration table;
 - `ispeci.tsv`: estimated concentration table;
 - `rate.tsv`: rate table;
 - `flux.tsv`: flux table;
 - `stats.tsv`: table with chi2 tests per compound;
 - `env.RData`: stored R list `res` such as returned by `dynafluxr::fdyn()`. It can be read in R session with `e=new.env(); load('C:/Users/millard/Documents/GIT/dynafluxr_notebook/repo/DynafluxR_notebook/toy_model/results/tmp/tmp_2/env.RData', envir=e)` and then used to retrieve e.g. integrated compounds as `icmpnd=e$res$isp(e$res$tpp)`;
 - `Readme.md`: this file;


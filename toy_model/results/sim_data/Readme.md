# Retrieving reaction rate dynamics from specie kinetics (dynafluxr results)

This is the result files produced by dynafluxr R package (v0.22.1) on 2025-02-21 15:13:28 +0100 (CET).

The command to reproduce these results is:

`Rscript --vanilla -e 'dynafluxr::cli()' "-m" "C:/Users/millard/Documents/GIT/dynafluxr/sup_data/toy_model/results/sim_data.txt" "-s" "C:/Users/millard/Documents/GIT/dynafluxr/sup_data/toy_model/network.txt"`

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
 - `env.RData`: stored R list `res` such as returned by `dynafluxr::fdyn()`. It can be read in R session with `e=new.env(); load('C:/Users/millard/Documents/GIT/dynafluxr/sup_data/toy_model/results/sim_data/env.RData', envir=e)` and then used to retrieve e.g. integrated compounds as `icmpnd=e$res$isp(e$res$tpp)`;
 - `Readme.md`: this file;


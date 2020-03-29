## Zika Virus Envelope escape from monoclonal antibodies

[Sourisseau _et al._, 2019](https://research.fhcrc.org/content/dam/stripe/bloom/labfiles/publications/Sourisseau2019.pdf) performed mutational antigenic profiling on the Envelope from MR766 Zika Virus to measure the effect of mutations on escape from two monoclonal antibodies.
Here we display those results.

The _differential selection_ statistic used in this analysis is explained in detail [here](https://jbloomlab.github.io/dms_tools2/diffsel.html).

For each monoclonal antibody, you can view the mean (across biological replicates) site- and mutation-level differential selection metrics.

The site-metrics (dot plot) include:

- **positive diffsel**: The sum of all positive differential selection values at a site (site level). This gives a sense to the total amount of escape/selective pressure at each site.
- **negative diffsel**: The sum of all negative differential selection values at a site (site level). This gives a sense for mutations that are depleted, rather than enriched, during serum selection relative to a non-selected control library.
- **max diffsel**: The value of the largest effect mutation (largest mutation differential selection) at each site (site level).
- **min diffsel**: The value of the smallest effect mutation (smallest mutation differential selection) at each site (site level).
- **abs diffsel**: The sum of the absolute value of each differential selection value at a site (site level).

The mutation-metrics (logoplot) include

- **diffsel**
- **pos diffsel**

See the [original paper](https://research.fhcrc.org/content/dam/stripe/bloom/labfiles/publications/Sourisseau2019.pdf) for more details; the data displayed here are available [here](https://github.com/jbloomlab/ZIKV_DMS_with_EvansLab).

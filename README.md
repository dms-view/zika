# Zika deep mutational scanning data sets visualized by `dms-view`

## Data sets

### Envelope

- Mutational tolerance of the Zika Virus Envelope protein from MR766 as measured by [Sourisseau _et al.,_ (2019)](https://research.fhcrc.org/content/dam/stripe/bloom/labfiles/publications/Sourisseau2019.pdf). [See here](https://dms-view.github.io/?markdown-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Fzika%2Fmaster%2Fdata%2FEnvelope%2FSourisseau2019%2FSourisseau2019_DMS.md&pdb-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Fzika%2Fmaster%2Fdata%2FEnvelope%2FSourisseau2019%2F5ire_C_E.pdb&data-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Fzika%2Fmaster%2Fdata%2FEnvelope%2FSourisseau2019%2FSourisseau2019_DMS.csv&condition=rescaled+preferences&site_metric=site_entropy&mutation_metric=mut_pref&selected_sites=R+99%2CG+100%2CW+101%2CG+102%2CN+103%2CG+104%2CC+105%2CG+106%2CL+107%2CF+108%2CG+109%2CQ+147%2CH+148%2CS+149%2CG+150%2CM+151%2CI+152%2CV+153%2CN+154%2CD+155%2CT+156%2CG+157%2CY+158%2CE+159%2CT+160%2CD+161) for a interactive dms-view visualization focusing on the conserved fusion loop and the hypervariable glycan loop. The raw data are [here](./data/Envelope/Sourisseau2019/).
- Mutational Antigenic Profiling of Zika Virus Envelope from two monoclonal antibodies measure by [Sourisseau _et al.,_ (2019)](https://research.fhcrc.org/content/dam/stripe/bloom/labfiles/publications/Sourisseau2019.pdf). [See here](https://dms-view.github.io/?markdown-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Fzika%2Fmaster%2Fdata%2FEnvelope%2FSourisseau2019%2FSourisseau2019_MAP.md&data-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Fzika%2Fmaster%2Fdata%2FEnvelope%2FSourisseau2019%2FSourisseau2019_MAP.csv&condition=ZKA64&site_metric=site_positive+diffsel&mutation_metric=mut_positive+diffsel&selected_sites=A+311%2CT+313%2CT+315%2CA+333%2CT+335%2CK+373&pdb-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Fzika%2Fmaster%2Fdata%2FEnvelope%2FSourisseau2019%2F5ire_C_E.pdb) for an interactive dms-view visualization focusing on the antibody ZKA64. The raw data are [here](./data/Envelope/Sourisseau2019/).

## Adding data sets

1. Make a new branch or a fork of this repository.

2. Navigate to the [./data/](data) directory and create a subdirectory for the appropriate protein and study.
Data are organized first by protein and then by study, with studies named by the first author and year, such as [./data/Envelope/Sourisseau2019/](data/Envelope/Sourisseau2019).

3. Within that subdirectory, add the three input files that are needed to visualize the data.
As described in the [`dms-view` docs](https://dms-view.github.io/docs/), these are a CSV file of the data, a protein structure PDB file, and a Markdown metadata file.
In general, you should name these with the CSV data file named according to the study name (e.g., [./data/Envelope/Sourisseau2019/Sourisseau2019_DMS.csv](data/Envelope/Sourisseau2019/Sourisseau2019_DMS.csv)), the PDB file simply being the PDB (e.g., [./data/Envelope/Sourisseau2019/5ire.pdb](./data/Envelope/Sourisseau2019/5ire.pdb)), and the Markdown metadata file also named according to the study name (e.g. [./data/Envelope/Sourisseau2019/Sourisseau2019_DMS.md](data/HA/Sourisseau2019/Sourisseau2019_DMS.md)).
In addition, you should add a README within the subdirectory explaining the origin of the files (e.g., [./data/Envelope/Sourisseau2019/README.md](./data/Envelope/Sourisseau2019/README.md)).
In some cases (such as if the same data is mapped to multiple protein structures) you may need to extend or modify this naming scheme.
If you need to process other rawer forms of the data (e.g., from paper supplements) into the final data file for `dms-view`, then include those rawer data and the processing scripts if possible, explaining in the subdirectory repo.

4. Make a pull request for your branch or fork to add the data.

5. In [this top-level README file](README.md) add a **short** description of the study and a link to an appropriate [dms-view](https://dms-view.github.io) view of the dataset.

6. Make a pull request for your branch or fork to add the link.

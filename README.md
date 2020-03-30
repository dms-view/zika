# Zika deep mutational scanning data sets visualized by `dms-view`

## Data sets

### Envelope

- Mutational tolerance of the Zika Virus Envelope protein from MR766 as measured by Sourisseau _et al.,_ (2019). [See here]() for a interactive dms-view visualization. The raw data are [here](./data/Envelope/Sourisseau2019/).


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

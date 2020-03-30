# Deep mutational scanning of MR766 Zika Envelope

The paper link is [Sourisseau _et al._, 2019](https://research.fhcrc.org/content/dam/stripe/bloom/labfiles/publications/Sourisseau2019.pdf).

The [5ire.pdb](5ire.pdb) ([pdb](https://www.rcsb.org/structure/5ire))protein structure, the [natural sequences](./E_alignment.fasta), and the data in the two `dms-view` datafiles ([Sourisseau2019_DMS.csv](Sourisseau2019_DMS.csv) and [Sourisseau2019_MAP.csv](Sourisseau2019_MAP.csv)) are from the [GitHub repo](https://github.com/jbloomlab/ZIKV_DMS_with_EvansLab) for the paper [Sourisseau _et al._, 2019](https://research.fhcrc.org/content/dam/stripe/bloom/labfiles/publications/Sourisseau2019.pdf).

The Jupyter notebook [build_data.ipynb](build_data.ipynb) reads in files from the [paper repo](https://github.com/jbloomlab/ZIKV_DMS_with_EvansLab) and creates a `dms-view` data file for the inherent mutational tolerance of the protein ([Sourisseau2019_DMS.csv](Sourisseau2019_DMS.csv)) and for the antibody mapping ([Sourisseau2019_MAP.csv](Sourisseau2019_MAP)).

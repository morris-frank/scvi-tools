<img src="https://github.com/YosefLab/scvi-tools/blob/master/docs/_static/scvi-tools-horizontal.svg?raw=true" width="400" alt="scvi-tools">

[![Stars](https://img.shields.io/github/stars/YosefLab/scvi-tools?logo=GitHub&color=yellow)](https://github.com/YosefLab/scvi-tools/stargazers)
[![PyPI](https://img.shields.io/pypi/v/scvi-tools.svg)](https://pypi.org/project/scvi-tools)
[![Documentation Status](https://readthedocs.org/projects/scvi/badge/?version=latest)](https://scvi.readthedocs.io/en/stable/?badge=stable)
![Build
Status](https://github.com/YosefLab/scvi-tools/workflows/scvi-tools/badge.svg)
[![Coverage](https://codecov.io/gh/YosefLab/scvi-tools/branch/master/graph/badge.svg)](https://codecov.io/gh/YosefLab/scvi-tools)
[![Code
Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
[![Downloads](https://pepy.tech/badge/scvi-tools)](https://pepy.tech/project/scvi-tools)
[![Join the chat at https://gitter.im/scvi-tools/development](https://badges.gitter.im/scvi-tools/development.svg)](https://gitter.im/scvi-tools/development?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[scvi-tools](https://scvi-tools.org/) (single-cell variational inference
tools) is a package for probabilistic modeling of single-cell omics
data, built on top of [PyTorch](https://pytorch.org) and
[AnnData](https://anndata.readthedocs.io/en/latest/).

# Available implementations of single-cell omics models

scvi-tools contains scalable implementations of several models that
facilitate a broad number of tasks across many omics, including:

-   [scVI](https://rdcu.be/bdHYQ) for analysis of single-cell RNA-seq
    data, as well as its improved differential expression
    [framework](https://www.biorxiv.org/content/biorxiv/early/2019/10/04/794289.full.pdf).
-   [scANVI](https://www.biorxiv.org/content/biorxiv/early/2019/01/29/532895.full.pdf)
    for cell annotation of scRNA-seq data using semi-labeled examples.
-   [totalVI](https://www.biorxiv.org/content/10.1101/2020.05.08.083337v1.full.pdf)
    for analysis of CITE-seq data.
-   [gimVI](https://arxiv.org/pdf/1905.02269.pdf) for imputation of
    missing genes in spatial transcriptomics from scRNA-seq data.
-   [AutoZI](https://www.biorxiv.org/content/biorxiv/early/2019/10/10/794875.full.pdf)
    for assessing gene-specific levels of zero-inflation in scRNA-seq
    data.
-   [LDVAE](https://www.biorxiv.org/content/10.1101/737601v1.full.pdf)
    for an interpretable linear factor model version of scVI.
-   [Stereoscope](https://www.nature.com/articles/s42003-020-01247-y)
    for deconvolution of spatial transcriptomics data.
-   DestVI for multi-resolution deconvolution 
    of spatial transcriptomics data.
-   peakVI for analysis of scATAC-seq data.
-   [scArches](https://www.biorxiv.org/content/10.1101/2020.07.16.205997v1)
    for transfer learning from one single-cell atlas to a query dataset
    (currently supports scVI, scANVI and TotalVI).
-   [CellAssign](https://www.nature.com/articles/s41592-019-0529-1) for
    reference-based annotation of scRNA-seq data.
-   [Solo](https://www.sciencedirect.com/science/article/pii/S2405471220301952) 
    for doublet detection in scRNA-seq data.

All these implementations have a high-level API that interacts with
[scanpy](http://scanpy.readthedocs.io/), standard save/load functions,
and support GPU acceleration.

# Fast prototyping of novel probabilistic models

scvi-tools contains the building blocks to prototype novel probablistic
models. These building blocks are powered by popular probabilistic and
machine learning frameworks such as [PyTorch
Lightning](https://www.pytorchlightning.ai/), and
[Pyro](https://pyro.ai/).

We recommend checking out the [skeleton
repository](https://github.com/YosefLab/scvi-tools-skeleton), as a
starting point for developing new models into scvi-tools.

# Basic installation

For conda, 
```
conda install scvi-tools -c bioconda -c conda-forge
```
and for pip,
```
pip install scvi-tools
```
Please be sure to install a version of [PyTorch](https://pytorch.org/) that is compatible with your GPU (if applicable).

# Resources

-   Tutorials, API reference, and installation guides are available in
    the [documentation](https://docs.scvi-tools.org/).
-   For discussion of usage, checkout out our
    [forum](https://discourse.scvi-tools.org).
-   Please use the issues here to submit bug reports.
-   If you\'d like to contribute, check out our [contributing
    guide](https://docs.scvi-tools.org/en/stable/contributing/index.html).
-   If you find a model useful for your research, please consider citing
    the corresponding publication (linked above).

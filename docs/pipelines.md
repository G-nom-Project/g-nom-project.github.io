G-nom supports and integrated various analyses, with planned expansion in future versions. Pre-made pipelines allow users to generate data for G-nom with minimal setup overhead.

## The Core pipeline
[![Nextflow](https://img.shields.io/badge/version-%E2%89%A524.04.2-green?style=flat&logo=nextflow&logoColor=white&color=%230DC09D&link=https%3A%2F%2Fnextflow.io)](https://www.nextflow.io/)
[![nf-core template version](https://img.shields.io/badge/nf--core_template-3.3.1-green?style=flat&logo=nfcore&logoColor=white&color=%2324B064&link=https%3A%2F%2Fnf-co.re)](https://github.com/nf-core/tools/releases/tag/3.3.1)
[![run with conda](http://img.shields.io/badge/run%20with-conda-3EB049?labelColor=000000&logo=anaconda)](https://docs.conda.io/en/latest/)

Steps to generate data for the G-nom core analyses are bundled in the [core pipeline](https://github.com/G-nom-Project/corepipeline). It currently includes the following tools:

| Tool | Available | Version | Notes |
| - | - | - | - |
| Repeatmasker  | ✅ | [4.1.7p1](https://bioconda.github.io/recipes/repeatmasker/README.html) | Databases for Repeatmasker must be downloaded separately. |
| BUSCO  | ✅ | [5.8.3](https://bioconda.github.io/recipes/busco/README.html) | Gene sets for BUSCO must be downloaded separately. |
| fCat | ❌ | - | Pending Bioconda Release |
| taXaminer | ❌ | - | Pending Publication |

The core pipeline is not executed by G-nom itself but designed to run in a separate HPC environment (it is generally advisable to isolate compute clusters from web-facing applications). The pipeline uses [nextflow](https://www.nextflow.io/) and is built on top of [nf-core](https://nf-co.re/). Nextflow supports all major HPC schedulers, including e.g. SLURM and LSF and can be set up in a few minutes. Nf-core provides a common style for the development of nextflow pipelines. The environments required to run the various tools are set up using conda. 

Further usage instructions can be found in the [repository](https://github.com/G-nom-Project/corepipeline). Please report issues in the pipeline repository rather then the main G-nom repository.

## Automatic import
Future versions of G-nom will include HTTP endpoints to automate the import of pipeline outputs. For progress, check the [issue](https://github.com/G-nom-Project/g-nom/issues/2) on Github.

# seqspec

![github version](https://img.shields.io/badge/Version-0.2.0-informational)
[![pypi version](https://img.shields.io/pypi/v/seqspec)](https://pypi.org/project/seqspec/0.2.0/)
![python versions](https://img.shields.io/pypi/pyversions/seqspec)
[![license](https://img.shields.io/pypi/l/seqspec)](LICENSE)

`seqspec` is a machine-readable YAML file format for genomic library sequence and structure. It was inspired by and builds off of the Teichmann Lab [Single Cell Genomics Library Structure](https://github.com/Teichlab/scg_lib_structs) by [Xi Chen](https://github.com/dbrg77).

Genomic library structure depends on both the assay and sequencer (and kit) used to generate and bind the assay-specific construct to the sequencing adapters to generate a sequencing library. Therefore, a `seqspec` is specific to both a genomics assay and sequencer.

A list of `seqspec` examples for multiple assays and sequencers can be found on [this website](https://igvf.github.io/seqspec/). Each `spec.yaml` describes the 5'->3' "Final library structure" for the assay and sequencer and can be extended to include sequencer-specific read annotations. Sequence specification files can be formatted with the `seqspec` command line tool.

The `seqspec` format and tool are described in this [publication](https://doi.org/10.1093/bioinformatics/btae168). If you use `seqspec` please cite

```
Ali Sina Booeshaghi, Xi Chen, Lior Pachter, A machine-readable specification for genomics assays, Bioinformatics, Volume 40, Issue 4, April 2024, btae168.
```

<img alt="image" src="/docs/seqspec.png">

```bash
# release
pip install seqspec

# development
pip install git+https://github.com/pachterlab/seqspec.git

# verify install
seqspec --help
```

Documentation:

- [ Learn about `seqspec` : `docs/DOCUMENTATION.md`](docs/DOCUMENTATION.md)
- [Write a `seqspec` : `docs/TUTORIAL.md`](docs/TUTORIAL.md)
- [Contribute a `seqspec` : `docs/CONTRIBUTING.md`](docs/CONTRIBUTING.md)
- [The `seqspec` specification : `docs/SPECIFICATION.md`](docs/SPECIFICATION.md)
- [YouTube video that introduces `seqspec`](https://youtu.be/NSj6Vpzy8tU)
- [_bioRxiv_ preprint that describes `seqspec`](https://doi.org/10.1101/2023.03.17.533215)

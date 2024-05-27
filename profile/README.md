# Bioinformatic and Data Analysis UniX Power Tools

Many BiDaUxPoTo tools can be found on the [molinerislab conda channel](https://anaconda.org/molinerislab)

## Conda Packages Creation

### Template Repo

The repository [conda_build_mockup](https://github.com/bidauxpoto/conda_build_mockup) can be used as a template for package construction. It contains:
- `src`:
  - put your scripts here
- `conda_recipe`
  - `build.sh` and `meta.yaml` to be manually updated
  - `makefile` with the general instructions for the package build and upload

### Dependencies
```
conda-build
anaconda-client
```

### Package build and upload
Move to the `conda_recipe` directory and follow this steps:

Create and activate `condaBuild` environment

```
conda create -n condaBuild conda-build
conda activate condaBuild
```

Build the package

```
make build
make upload
or
make upload_noarch
```

The packages will be included as part of the [Molineris Lab Organization](https://anaconda.org/molinerislab) on Anaconda.

To upload a package you need to be [added as a developer](https://anaconda.org/molinerislab/groups) of the organization by an owner. [Open an issue](https://github.com/bidauxpoto/conda_build_mockup/issues) to ask for access.

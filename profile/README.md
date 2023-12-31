# Bioinformatic and Data Analysis UniX Power Tools

## Conda Packages Creation

### Template Repo

The repository `conda_package_mockup` can be used as a template for package construction. It contains:
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
Move to the `conda_recipe` directory and run:

Activate the proper environment

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

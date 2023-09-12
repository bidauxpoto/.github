## Conda Packages Creation

The repository `conda_package_template` contains:
- `src`:
  - put your scripts here
- `conda_recipe`
  - `build.sh` and `meta.yaml` to be manually updated
  - `makefile` with the general instructions for the package build and upload

To build and upload the package run `make upload`.

The packages will be included as part of the [Molineris Lab Organization](https://anaconda.org/molinerislab) on Anaconda.

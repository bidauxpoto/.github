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
```
make package/name
make build
make upload
```

The packages will be included as part of the [Molineris Lab Organization](https://anaconda.org/molinerislab) on Anaconda.

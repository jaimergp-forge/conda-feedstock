About conda-feedstock
=====================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/conda-feedstock/blob/main/LICENSE.txt)

Home: https://conda.io

Package license: BSD-3-Clause

Summary: OS-agnostic, system-level binary package and environment manager.

Development: https://github.com/conda/conda

Documentation: https://docs.conda.io/projects/conda/en/stable/

Conda is an open source package management system and environment
management system for installing multiple versions of software packages
and their dependencies and switching easily between them. It works on
Linux, OS X and Windows, and was created for Python programs but can
package and distribute any software.


Current build status
====================


<table>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-conda-green.svg)](https://anaconda.org/napari/conda) | [![Conda Downloads](https://img.shields.io/conda/dn/napari/conda.svg)](https://anaconda.org/napari/conda) | [![Conda Version](https://img.shields.io/conda/vn/napari/conda.svg)](https://anaconda.org/napari/conda) | [![Conda Platforms](https://img.shields.io/conda/pn/napari/conda.svg)](https://anaconda.org/napari/conda) |

Installing conda
================

Installing `conda` from the `napari` channel can be achieved by adding `napari` to your channels with:

```
conda config --add channels napari
conda config --set channel_priority strict
```

Once the `napari` channel has been enabled, `conda` can be installed with `conda`:

```
conda install conda
```

or with `mamba`:

```
mamba install conda
```

It is possible to list all of the versions of `conda` available on your platform with `conda`:

```
conda search conda --channel napari
```

or with `mamba`:

```
mamba search conda --channel napari
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search conda --channel napari

# List packages depending on `conda`:
mamba repoquery whoneeds conda --channel napari

# List dependencies of `conda`:
mamba repoquery depends conda --channel napari
```




Updating conda-feedstock
========================

If you would like to improve the conda recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`napari` channel, whereupon the built conda packages will be available for
everybody to install and use from the `napari` channel.
Note that all branches in the conda-forge/conda-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@dbast](https://github.com/dbast/)
* [@isuruf](https://github.com/isuruf/)
* [@jakirkham](https://github.com/jakirkham/)
* [@jezdez](https://github.com/jezdez/)
* [@kenodegard](https://github.com/kenodegard/)
* [@mbargull](https://github.com/mbargull/)
* [@ocefpaf](https://github.com/ocefpaf/)


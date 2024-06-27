About tblis-feedstock
=====================

Feedstock license: [BSD-3-Clause](https://github.com/chillenb/tblis-feedstock/blob/main/LICENSE.txt)

Home: https://github.com/devinamatthews/tblis

Package license: BSD-3-Clause

Summary: Tensor-Based Library Instantiation Software

Development: https://github.com/devinamatthews/tblis

Documentation: https://github.com/devinamatthews/tblis/wiki

TBLIS is a library and framework for performing tensor operations,
especially tensor contraction, using native algorithms. In this context,
native means that TBLIS does not translate tensor operations into matrix
operations using the BLAS libraries. Instead, TBLIS uses the philosophy
(and certain low-level kernels) of the BLIS framework to implement tensor
contraction with essentially zero overhead compared to matrix
multiplication. TBLIS also aims to offer a convenient C++ interface for
tensors and tensor operations, as well as a stable C interface with high
portability.


Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/christopherhillenbrand/feedstock-builds/_build/latest?definitionId=None&branchName=main">
            <img src="https://dev.azure.com/christopherhillenbrand/feedstock-builds/_apis/build/status/tblis-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64</td>
              <td>
                <a href="https://dev.azure.com/christopherhillenbrand/feedstock-builds/_build/latest?definitionId=None&branchName=main">
                  <img src="https://dev.azure.com/christopherhillenbrand/feedstock-builds/_apis/build/status/tblis-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64</td>
              <td>
                <a href="https://dev.azure.com/christopherhillenbrand/feedstock-builds/_build/latest?definitionId=None&branchName=main">
                  <img src="https://dev.azure.com/christopherhillenbrand/feedstock-builds/_apis/build/status/tblis-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_64_" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-tblis-green.svg)](https://anaconda.org/chillenb/tblis) | [![Conda Downloads](https://img.shields.io/conda/dn/chillenb/tblis.svg)](https://anaconda.org/chillenb/tblis) | [![Conda Version](https://img.shields.io/conda/vn/chillenb/tblis.svg)](https://anaconda.org/chillenb/tblis) | [![Conda Platforms](https://img.shields.io/conda/pn/chillenb/tblis.svg)](https://anaconda.org/chillenb/tblis) |

Installing tblis
================

Installing `tblis` from the `chillenb/label/` channel can be achieved by adding `chillenb/label/` to your channels with:

```
conda config --add channels chillenb/label/
conda config --set channel_priority strict
```

Once the `chillenb/label/` channel has been enabled, `tblis` can be installed with `conda`:

```
conda install tblis
```

or with `mamba`:

```
mamba install tblis
```

It is possible to list all of the versions of `tblis` available on your platform with `conda`:

```
conda search tblis --channel chillenb/label/
```

or with `mamba`:

```
mamba search tblis --channel chillenb/label/
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search tblis --channel chillenb/label/

# List packages depending on `tblis`:
mamba repoquery whoneeds tblis --channel chillenb/label/

# List dependencies of `tblis`:
mamba repoquery depends tblis --channel chillenb/label/
```




Updating tblis-feedstock
========================

If you would like to improve the tblis recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`chillenb` channel, whereupon the built conda packages will be available for
everybody to install and use from the `chillenb` channel.
Note that all branches in the chillenb/tblis-feedstock are
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

* [@chillenb](https://github.com/chillenb/)


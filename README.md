About pyfai
===========

Home: https://github.com/silx-kit/pyFAI/

Package license: GPL-3

Feedstock license: [BSD-3-Clause](https://github.com/nsls-ii-forge/pyfai-feedstock/blob/master/LICENSE.txt)

Summary: Python implementation of fast azimuthal integration

Development: https://github.com/silx-kit/pyFAI/

Documentation: http://pythonhosted.org/pyFAI/

pyFAI is an azimuthal integration library that tries to be fast (as fast
as C and even more using OpenCL and GPU). It is based on histogramming of
the 2theta/Q positions of each (center of) pixel weighted by the intensity
of each pixel, but parallel version uses a SparseMatrix-DenseVector
multiplication. Neighboring output bins get also a contribution of pixels
next to the border thanks to pixel splitting. Finally pyFAI provides also
tools to calibrate the experimental setup using Debye-Scherrer rings of a
reference compound.


Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/nsls2forge/nsls2forge/_build/latest?definitionId=80&branchName=master">
            <img src="https://dev.azure.com/nsls2forge/nsls2forge/_apis/build/status/pyfai-feedstock?branchName=master">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64_python3.7</td>
              <td>
                <a href="https://dev.azure.com/nsls2forge/nsls2forge/_build/latest?definitionId=80&branchName=master">
                  <img src="https://dev.azure.com/nsls2forge/nsls2forge/_apis/build/status/pyfai-feedstock?branchName=master&jobName=linux&configuration=linux_64_python3.7" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_python3.8</td>
              <td>
                <a href="https://dev.azure.com/nsls2forge/nsls2forge/_build/latest?definitionId=80&branchName=master">
                  <img src="https://dev.azure.com/nsls2forge/nsls2forge/_apis/build/status/pyfai-feedstock?branchName=master&jobName=linux&configuration=linux_64_python3.8" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_python3.9</td>
              <td>
                <a href="https://dev.azure.com/nsls2forge/nsls2forge/_build/latest?definitionId=80&branchName=master">
                  <img src="https://dev.azure.com/nsls2forge/nsls2forge/_apis/build/status/pyfai-feedstock?branchName=master&jobName=linux&configuration=linux_64_python3.9" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64_python3.7</td>
              <td>
                <a href="https://dev.azure.com/nsls2forge/nsls2forge/_build/latest?definitionId=80&branchName=master">
                  <img src="https://dev.azure.com/nsls2forge/nsls2forge/_apis/build/status/pyfai-feedstock?branchName=master&jobName=osx&configuration=osx_64_python3.7" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64_python3.8</td>
              <td>
                <a href="https://dev.azure.com/nsls2forge/nsls2forge/_build/latest?definitionId=80&branchName=master">
                  <img src="https://dev.azure.com/nsls2forge/nsls2forge/_apis/build/status/pyfai-feedstock?branchName=master&jobName=osx&configuration=osx_64_python3.8" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64_python3.9</td>
              <td>
                <a href="https://dev.azure.com/nsls2forge/nsls2forge/_build/latest?definitionId=80&branchName=master">
                  <img src="https://dev.azure.com/nsls2forge/nsls2forge/_apis/build/status/pyfai-feedstock?branchName=master&jobName=osx&configuration=osx_64_python3.9" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_python3.7</td>
              <td>
                <a href="https://dev.azure.com/nsls2forge/nsls2forge/_build/latest?definitionId=80&branchName=master">
                  <img src="https://dev.azure.com/nsls2forge/nsls2forge/_apis/build/status/pyfai-feedstock?branchName=master&jobName=win&configuration=win_64_python3.7" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_python3.8</td>
              <td>
                <a href="https://dev.azure.com/nsls2forge/nsls2forge/_build/latest?definitionId=80&branchName=master">
                  <img src="https://dev.azure.com/nsls2forge/nsls2forge/_apis/build/status/pyfai-feedstock?branchName=master&jobName=win&configuration=win_64_python3.8" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_python3.9</td>
              <td>
                <a href="https://dev.azure.com/nsls2forge/nsls2forge/_build/latest?definitionId=80&branchName=master">
                  <img src="https://dev.azure.com/nsls2forge/nsls2forge/_apis/build/status/pyfai-feedstock?branchName=master&jobName=win&configuration=win_64_python3.9" alt="variant">
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
| [![Conda Recipe](https://img.shields.io/badge/recipe-pyfai-green.svg)](https://anaconda.org/nsls2forge/pyfai) | [![Conda Downloads](https://img.shields.io/conda/dn/nsls2forge/pyfai.svg)](https://anaconda.org/nsls2forge/pyfai) | [![Conda Version](https://img.shields.io/conda/vn/nsls2forge/pyfai.svg)](https://anaconda.org/nsls2forge/pyfai) | [![Conda Platforms](https://img.shields.io/conda/pn/nsls2forge/pyfai.svg)](https://anaconda.org/nsls2forge/pyfai) |

Installing pyfai
================

Installing `pyfai` from the `nsls2forge` channel can be achieved by adding `nsls2forge` to your channels with:

```
conda config --add channels nsls2forge
```

Once the `nsls2forge` channel has been enabled, `pyfai` can be installed with:

```
conda install pyfai
```

It is possible to list all of the versions of `pyfai` available on your platform with:

```
conda search pyfai --channel nsls2forge
```




Updating pyfai-feedstock
========================

If you would like to improve the pyfai recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`nsls2forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `nsls2forge` channel.
Note that all branches in the nsls-ii-forge/pyfai-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================



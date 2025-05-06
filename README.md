# TrinomialTest
[![CI](https://github.com/jrudar/TrinomialTest/actions/workflows/ci.yml/badge.svg)](https://github.com/jrudar/TrinomialTest/actions/workflows/ci.yml)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15353378.svg)](https://doi.org/10.5281/zenodo.15353378)

The trinomial test is a non-parametric statistical test for consistent differences between paired data or medians.

### Install
From PyPI:

```bash
pip install TrinomialTest
```

From source:

```bash
git clone https://github.com/jrudar/TrinomialTest.git
cd TrinomialTest
pip install .
# or create a virtual environment
python -m venv venv
source venv/bin/activate
pip install .
```

### Usage

```bash
import numpy as np
from TrinomialTest import TrinomialTest
X = np.asarray([1, 1, 1, 1, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3])
Y = np.asarray([2, 2, 2, 2, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3])
result = TrinomialTest(X, Y, alternative = "two-sided")

# p-value should be 0.0772262851453612
print(result.pvalue)
```

### Citation

Rudar, J., & Lung, O. (2025). TrinomialTest. Zenodo. https://doi.org/10.5281/zenodo.15353378

Bian, Guorui & McAleer, Michael & Wong, Wing-Keung, 2011. "A trinomial test for paired data when there are many ties," Mathematics and Computers in Simulation (MATCOM), Elsevier, vol. 81(6), pages 1153-1160.

Whitaker, D., Drew, B., & Barss, J. (2021) GridItemTools: Grid item tools. R package version 0.0.12. https://github.com/douglaswhitaker/GridItemTools  


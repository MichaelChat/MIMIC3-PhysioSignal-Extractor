# MIMIC3-PhysioSignal-Extractor

This project filters and extracts the header files for various physiological signals from the [MIMIC-III Waveform Database Matched Subset v1.0](https://physionet.org/content/mimic3wdb-matched/1.0/). In detail:

* Waveform records header containing **PPG** signals
* Numerics records header containing **ABP** signals ('ABP', 'ABP DIAS', 'ABP Dias', 'ABP MEAN', 'ABP Mean', 'ABP SYS', 'ABP Sys')
* Numerics records header containing **NBP** signals ('NBP', 'NBP DIAS', 'NBP Dias', 'NBP MEAN', 'NBP Mean', 'NBP SYS', 'NBP Sys', 'PlsNBP')

## Table of Contents

1. [Background](#background)
1. [Prerequisites](#prerequisites)
1. [File Structure](#file-structure)
2. [References](#references)

## Background

The [MIMIC-III Waveform Database Matched Subset v1.0](https://physionet.org/content/mimic3wdb-matched/1.0/) [3] contains a collection of medical waveform records and builds upon the foundational work of [2]. This project focuses on extracting specific physiological signals, including PPG (Photoplethysmogram), NBP (Non-invasive Blood Pressure), and ABP (Arterial Blood Pressure) records.

The project also acknowledges the contribution of [1], who established the foundation for complex physiologic signal research with the creation of PhysioBank, PhysioToolkit, and PhysioNet.

## Prerequisites

Before running the code, make sure you have the following dependencies installed:

* [wfdb-python](https://github.com/MIT-LCP/wfdb-python) - Python library for reading PhysioNet Waveform Database (WFDB) format files [4]

You can install wfdb-python using pip:

```bash
pip install wfdb
```

## File Structure

* **data/**: Contains the filtered PPG, NBP and ABP records
* **src/**: Contains the Python codes for filtering PPG, NBP, and ABP records

## References

> [1] Goldberger, A., Amaral, L., Glass, L., Hausdorff, J., Ivanov, P. C., Mark, R., ... & Stanley, H. E. (2000). PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research resource for complex physiologic signals. Circulation [Online]. 101 (23), pp. e215–e220.

> [2] [Johnson, A. E. W., Pollard, T. J., Shen, L., Lehman, L. H., Feng, M., Ghassemi, M., Moody, B., Szolovits, P., Celi, L. A., & Mark, R. G. (2016). MIMIC-III, a freely accessible critical care database. Scientific Data, 3, 160035](https://dx.doi.org/10.1038/sdata.2016.35).

> [3] Moody, B., Moody, G., Villarroel, M., Clifford, G. D., & Silva, I. (2020). MIMIC-III Waveform Database Matched Subset (version 1.0). PhysioNet. https://doi.org/10.13026/c2294b.

> [4] Xie, C., McCullum, L., Johnson, A., Pollard, T., Gow, B., & Moody, B. (2023). Waveform Database Software Package (WFDB) for Python (version 4.1.0). PhysioNet. https://doi.org/10.13026/9njx-6322.

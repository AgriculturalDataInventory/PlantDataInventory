# Plant data inventory
A collection of datasets related to plants.

<p align="center">
  <img src="https://github.com/AgriculturalDataInventory/PlantDataInventory/blob/main/DetectedStrawberries.png" width="300">
</p>

# Goal
Cooperationa and improving AI models for agricultural applications.

## Methods
- Development generic machine learning models based on different data sets.

- Concentration of efforts for solving of specific problems by collaboration.

# Strawberry
## Strawberry detection
| link | Size | Variables | Model | Paper |
|------|------|:---------:|-------|-------|
| https://strawdi.github.io/ | 4.1GB | images | Mask R-CNN | [Pérez-Borrero et al., 2020](https://www.sciencedirect.com/science/article/abs/pii/S0168169920300624) |
| https://zenodo.org/record/6126677 | 1.5 GB | images | CNN YOLOv5 | [Lemsalu et al., 2021]() |
| https://zenodo.org/record/5849025 | 41.7 MB | Ax, Ay, Az | CNN | [Li et al., 2021](https://ieeexplore.ieee.org/abstract/document/9566833) |
| https://zenodo.org/record/6784671 | 2.4 GB | Ax, Ay, Az | CNN | Bloch et al., 2022 |
## Cow indoor localization
| link | Size | Variables | Model | Paper |
|------|------|:---------:|-------|-------|
| https://zenodo.org/record/3981400 | 40 Gb | Frames | CNN | Pereira et al., in review |
| https://zenodo.org/record/3900340 | 50 Gb | RSS x 10 stations | Trilateration | [Bloch et al., 2020](https://www.mdpi.com/1424-8220/20/14/3841) |
## Cow outdoor localization

## Cow health and welfare
| link | Size | Variables | Model | Paper |
|------|------|:---------:|-------|-------|
| https://data.inrae.fr/dataset.xhtml?persistentId=doi:10.15454/52J8YS | 165 Mb |  |  | [Lardy et al. 2022](https://doi.org/10.1016/j.anopes.2022.100004) |

# Pigs
## Pigs behavior

# Suggestions for the data formats
## Tag acceleration
Files will be in .csv format with ';' as the delimiter. One file will contain data from one tag during one day from 00-00-00 till 23-59-59 or part of the day. The file name will have the format AccXYZ_YYYY-MM-DD_TagNNNN.csv, where NNNN is the number of the tag with the required number of digits and left 0 digits to keep all numbers in the same length. The file will include the time stamp in format HH-MM-SS.FFF, where HH is hours from 01 to 23 including the first 0 digit, MM are minutes including the first 0 digit, SS are seconds including the first 0 digit and FFF are milliseconds. The reference will be marked by a shortest distinguishable mark, for example, S is standing, L is lying, W is walking.

Example

| DateTime | Ax | Ay | Az | Reference behavior |
|----------|----|----|----|--------------------|
| 11-25-30.120 | 500 | 600 | -700 | S |

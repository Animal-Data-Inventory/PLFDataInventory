# PLF data inventory
A database collection of farm animal behaviour phenotypes for modelling exploration.

<p align="center">
  <img src="https://github.com/Animal-Data-Inventory/PLFDataInventory/blob/main/CowSensor.jpg" width="300">
</p>

# Goal
Complete solution of the animal monitoring behavior problem.

## Methods
- Development generic machine learning models based on different data sets.

- Concentration of efforts for solving of specific problems by collaboration.

# Cows
## Cow behavior
| link | Size | Variables | Model | Paper |
|------|------|:---------:|-------|-------|
| https://www.mdpi.com/1424-8220/20/17/4741 | 89Mb | X, Y, Z, Ax, Ay, Az | Linear mixed model | [Riaboff et al., 2020](https://www.mdpi.com/1424-8220/20/17/4741) |
| https://zenodo.org/record/4064802 | 8.2 GB | Ax, Ay, Az | CNN | [Pavlovic et al., 2021](https://www.mdpi.com/1424-8220/21/12/4050) |
## Cow indoor localization
| link | Size | Variables | Model | Paper |
|------|------|:---------:|-------|-------|
| https://zenodo.org/record/3981400 | 40Gb | Frames | CNN | [](https://www.frontiersin.org/articles/10.3389/frobt.2018.00107/full) |
| https://zenodo.org/deposit/3900340 | 50Gb | RSS x 10 stations | Trilateration | [Bloch et al., 2020](https://www.mdpi.com/1424-8220/20/14/3841) |
## Cow outdoor localization

# Pigs
## Pigs behavior

# Suggestions for the data formats
## Tag acceleration
Files will be in .csv format with ';' as the delimiter. One file will contain data from one tag during one day from 00-00-00 till 23-59-59 or part of the day. The file name will have the format AccXYZ_YYYY-MM-DD_TagNNNN.csv, where NNNN is the number of the tag with the required number of digits and left 0 digits to keep all numbers in the same length. The file will include the time stamp in format HH-MM-SS.FFF, where HH is hours from 01 to 23 including the first 0 digit, MM are minutes including the first 0 digit, SS are seconds including the first 0 digit and FFF are milliseconds. The reference will be marked by a shortest distinguishable mark, for example, S is standing, L is lying, W is walking.

Example

| DateTime | Ax | Ay | Az | Reference behavior |
|----------|----|----|----|--------------------|
| 11-25-30.120 | 500 | 600 | -700 | S |

# PLF data inventory
A database collection of farm animal behaviour phenotypes for modelling exploration.

<p align="center">
  <img src="https://github.com/oldtelescope/AnimalBehaviorDataBase/blob/main/CowSensor.jpg" width="300">
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
| https://zenodo.org/record/3981400 | 40Gb | Frames | Deep learning | in review |
| https://www.mdpi.com/1424-8220/20/17/4741/xml | 89Mb | X, Y, Z, Ax, Ay, Az | Linear mixed model | https://www.mdpi.com/1424-8220/20/17/4741/xml |
## Cow indoor localization
| link | Size | Variables | Model | Paper |
|------|------|:---------:|-------|-------|
| https://zenodo.org/deposit/3900340 | 50Gb | RSS x 10 stations | Trilateration | https://www.mdpi.com/1424-8220/20/14/3841 |
## Cow outdoor localization

# Pigs
## Pigs behavior

# Suggestions for the data formats
## Tag acceleration
Files in .csv format with ';' as the delimiter.

Example

| CowNo | DateTime | Ax | Ay | Az | Reference behavior |
|-------|----------|----|----|----|--------------------|
| 1234 | 2020-01-01 11-25-30 | 500 | 600 | -700 | Standing |

# Magnetic Field Strength vs Distance
## PHY 2049 Lab Report 2 
**Written in Python 3.8 by Alex C.** 

The best way to install the jupyter notebook dependencies is to install conda and activate the provided environment using `conda env create -f environment.yml`

To utilize the environment and ensure the code runs on your computer, download miniconda from [conda.io](https://docs.conda.io/en/latest/miniconda.html).

## Data
The data was taken through Google Science Journal on iOS 14.
Each test was run for 5 seconds 5 times, and then exported to a .csv file. The trials were conducted at lengths of 0-10 cm. 
The raw files are in the directory `./magnet-data/`.

The gathered data was analyzed using matplotlib.pyplot, numpy, and scipy.stats. 

## Expected vs Observed Outcome
For point electric charges like monopoles, the electric field strength decreases as the distance from the source increases, following Coulomb's law: ![equation](https://latex.codecogs.com/gif.latex?1/R^2)

## Outputs
Check `./figs/` for .png files of the data from each of the results. 
The subdirectory `./out/` contains csv files of each dataset where the first row is the mean, the second row is the standard deviation, and the third row is the chisquared values.

## Reproducing the Outputs
In a bash/zsh/sh shell with conda installed run:

```bash    
git clone https://github.com/doc-ock/magnets.git 
cd magnets
conda env create -f environment.yml
conda activate magnets
```

Once you are in an environment that has the required packages installed, open the jupyter notebook:

```bash
jupyter notebook
```
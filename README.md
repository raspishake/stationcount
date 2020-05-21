# stationcount
Time series graphs of currently active stations in the Raspberry Shake network. This graph was created with the help of Malcolm Maclean ([@d3noob](https://twitter.com/d3noob) on Twitter) who originally created it to track the growth of the network.

![Example plot](img/unique.png)

Required software:
- Python 3
- Jupyter
- Matplotlib
- Obspy
- Pandas
- tqdm

Installation via Anaconda:
```bash
# install the environment with the correct software:
conda create -n stationcount python=3 jupyter matplotlib obspy pandas tqdm
# activate the environment
conda activate stationcount
# start Jupyter Notebook
jupyter-notebook
```

Then, navigate to this repository and open one of the two `.ipynb` files. Each notebook plots the information in the same way but relies on different data.

- [stationcount-20191109.ipynb](stationcount-20191109.ipynb): Uses premade CSV file in this repository as data source
- [stationcount.ipynb](stationcount.ipynb): Uses the FDSN server as data source

## Note:
_As of 11 November 2019, the FDSN server contains a bug that causes incorrect connection time to appear in the station metadata. Until the FDSN data is corrected, it is currently best to use the [stationcount-20191109.ipynb](stationcount-20191109.ipynb) method above._ 

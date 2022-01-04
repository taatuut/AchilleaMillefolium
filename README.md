# AchilleaMillefolium
Playground for folium and movingpandas

# Setup

`python3 -m pip install --upgrade pip`

`python3 -m pip install folium`

Assumes

* pandas, if not installed `python3 -m pip install pandas`

# Data

https://github.com/trainline-eu/stations/blob/master/stations.csv

Created `stations_NL.csv` by selecting stations from NL with values for latitude and longitude fields. Notebook errors with `ValueError: Location values cannot contain NaNs.` when coordinates are missing.

# Run

Create Jupyter notebook `ezfolium.ipynb`

Add code, changing some of the original stuff like default start location and data for custom stuff, then play it.

Changed the coordinates to a different start location: OLV Kerk Amersfoort :-)

First run might show a popup stating "Running cells with 'Python 3.9.7 64-bit' requires ipykernel.", see Images/RunningCellsWithPPython3.9.7-64-bitRequires-ipykernel.jpg

Click `[ Install ]`

It will run `/usr/local/bin/python3 -m pip install -U ipykernel` in the VS Code context

`/usr/local/bin/python3 /Users/emil.zegers/.vscode/extensions/ms-python.python-2021.12.1559732655/pythonFiles/shell_exec.py /usr/local/bin/python3 -m pip install -U ipykernel /var/folders/4s/69z7hb_57zn27jq6pb0k8_780000gp/T/tmp-61747RA3u0OpndcOw.log`

Left out progress messages collecting the packages, in the end satisfied requirements and collected packages installed are reported:

```
Requirement already satisfied: six>=1.5 in /usr/local/lib/python3.9/site-packages (from python-dateutil>=2.1->jupyter-client<8.0->ipykernel) (1.15.0)
Installing collected packages: wcwidth, traitlets, ptyprocess, parso, tornado, pygments, prompt-toolkit, pickleshare, pexpect, nest-asyncio, matplotlib-inline, jupyter-core, jedi, entrypoints, decorator, backcall, appnope, jupyter-client, ipython, debugpy, ipykernel
```

NOTE: Initially tried to run teh code with a plain Python file called `folium.py`. Does not run anyway because it needs a notebook, but the point is you should not give it the same name as `folium` package or it will interfere with the import... I remmeber having seen this before, probably a generic non-feature.

# Inspiration

https://towardsdatascience.com/visualization-in-python-visualizing-geospatial-data-122bf85d128f

https://github.com/anitagraser/movingpandas

https://anitagraser.com/

https://en.wikipedia.org/wiki/Onze_Lieve_Vrouwetoren


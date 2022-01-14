# README

Open Jupyter notebook `ezfolium_mdb.ipynb` for up to date information. Creating a web gis app in just 10 lines of code (including the `import` statements). Ok, chained a few lines but there is still even some extra code in there e.g. for the (very nice!) multiple map base layers, check it out. And you do need to have a MongoDB instance with some geojson, that too.

(The Jupyter notebook `ezfolium_csv.ipynb` was a first try with `csv` as source data.)

# Inspiration

https://towardsdatascience.com/visualization-in-python-visualizing-geospatial-data-122bf85d128f

https://github.com/anitagraser/movingpandas

https://anitagraser.com/

https://en.wikipedia.org/wiki/Onze_Lieve_Vrouwetoren

https://thedatafrog.com/en/articles/mongodb-python-pandas/

## Notes

When using Microsfot VS Code, the first run might show a popup stating "Running cells with 'Python 3.9.7 64-bit' requires ipykernel.", see Images/RunningCellsWithPPython3.9.7-64-bitRequires-ipykernel.jpg

If so, click `[ Install ]`

It will run `/usr/local/bin/python3 -m pip install -U ipykernel` in the VS Code context, something like:

`/usr/local/bin/python3 /Users/emil.zegers/.vscode/extensions/ms-python.python-2021.12.1559732655/pythonFiles/shell_exec.py /usr/local/bin/python3 -m pip install -U ipykernel /var/folders/4s/69z7hb_57zn27jq6pb0k8_780000gp/T/tmp-61747RA3u0OpndcOw.log`

Left out the progress messages about collecting the packages, in the end requirements were satisfied and the collected packages installed are reported:

```
Requirement already satisfied: six>=1.5 in /usr/local/lib/python3.9/site-packages (from python-dateutil>=2.1->jupyter-client<8.0->ipykernel) (1.15.0)
Installing collected packages: wcwidth, traitlets, ptyprocess, parso, tornado, pygments, prompt-toolkit, pickleshare, pexpect, nest-asyncio, matplotlib-inline, jupyter-core, jedi, entrypoints, decorator, backcall, appnope, jupyter-client, ipython, debugpy, ipykernel
```

![image](https://user-images.githubusercontent.com/2260360/148051119-ac862c5c-21be-457c-b4c9-7d9f9f4f187c.png)

Initially tried to run the code with a plain Python file called `folium.py`. Does not run anyway because it needs a notebook, but the point is you should not give it the same name as `folium` package or it will interfere with the import... I remmeber having seen this before, probably a generic non-feature.

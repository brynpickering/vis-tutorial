# Openmod visualisation tutorial

Authors: Bryn Pickering, Stefan Pfenninger

License: MIT

## About

A tutorial on how to visualise data with Python, consisting of three Jupyter Notebooks:

* [01-matplotlib.ipynb](01-matplotlib.ipynb) shows how to use matplotlib, the workhorse of plotting in Python, together with pandas and seaborn.
* [02-web-based.ipynb](02-web-based.ipynb) introduces Plotly, a modern web-based library which makes it very easy to create interactive visualisations.
* [03-touching-up.ipynb](03-touching-up.ipynb) shows how to save vector graphics from matplotlib or plotly for final touching up in a separate tool, for example the free and open-source [Inkscape](http://inkscape.org/).

## Setup

### Environment

Create a new conda environment with the required packages:

```bash
$ conda env create -f requirements.yml
```

### Data

Download these three files and save them inside the `data` subdirectory:

* [time_series_60min_singleindex.csv](http://data.open-power-system-data.org/time_series/2017-03-06/time_series_60min_singleindex.csv)
* [conventional_power_plants_DE.csv](http://data.open-power-system-data.org/conventional_power_plants/2017-03-03/conventional_power_plants_DE.csv)
* [conventional_power_plants_EU.csv](http://data.open-power-system-data.org/conventional_power_plants/2017-03-03/conventional_power_plants_EU.csv)


The easiest way is to run these three commands in your terminal:

```bash

$ curl -o data/time_series_60min_singleindex.csv http://data.open-power-system-data.org/time_series/2017-03-06/time_series_60min_singleindex.csv

$ curl -o data/conventional_power_plants_DE.csv http://data.open-power-system-data.org/conventional_power_plants/2017-03-03/conventional_power_plants_DE.csv

$ curl -o data/conventional_power_plants_EU.csv http://data.open-power-system-data.org/conventional_power_plants/2017-03-03/conventional_power_plants_EU.csv

```

## Other libraries we don't cover here

* [bokeh](http://bokeh.pydata.org/en/latest/)
* d3 (e.g. [mpld3](https://mpld3.github.io/))
* [vega](https://vega.github.io/vega/) and [altair](https://altair-viz.github.io/)

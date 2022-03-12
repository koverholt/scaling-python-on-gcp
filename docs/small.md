# Small-scale Computations

## Overview

The
[notebook for this example](https://github.com/koverholt/scaling-python-on-gcp/blob/main/1-small-scale/satellite-imagery.ipynb)
runs small-scale computations on a laptop using XArray and Dask.

## Step 1: Clone the repository

Clone the repository with these examples by running the following command in
your terminal:

```shell
git clone https://github.com/koverholt/scaling-python-on-gcp
```

## Step 2: Install dependencies

Install the Python packages in this repository by running:

```shell
pip install -r requirements.txt
```

## Step 3: Run the small-scale notebook

The notebook for this small-scale computation contains all of the remaining code
that you need to run for this example. You can view and run the notebook by
using:

```shell
jupyter lab
```

Then, run through all of the notebook cells to download the satellite image
data, start a local Dask cluster on your machine, and compute and visualize the
NDVI.

## Success!

Congratulations! You've successfully run the small-scale computation example and
calculated the normalized difference vegetation index (NDVI) on a satellite
image from the comfort of your laptop.

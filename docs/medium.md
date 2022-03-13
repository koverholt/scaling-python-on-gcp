# Medium-scale Computations

## Overview

The
[notebook for this example](https://github.com/koverholt/scaling-python-on-gcp/blob/main/2-medium-scale/satellite-imagery.ipynb)
runs medium-scale computations on a notebook instance in GCP Vertex AI Workbench
using XArray and Dask.

## Step 1: Create a notebook environment in Vertex AI

Follow the steps in the GCP documentation to [create a user-managed notebook
instance within Vertex AI
Workbench](https://cloud.google.com/vertex-ai/docs/workbench/user-managed/create-user-managed-notebooks-instance).

From the Google Cloud Console, navigate to `Vertex AI` > `Workbench`, then click
on `New Notebook` in the `User-managed Notebooks` tab. For this example you can
select the `Python 3` environment, give your notebook a name, and select your
desired region.

<img src="/images/medium-scale-create-notebook.png" width="500px" style="display: block; margin-left: auto; margin-right: auto;" alt="Creating a notebook instance in GCP Vertex AI Workbench">

You can click on the `Create` button to create your notebook, or you can
customize your machine type and other settings by clicking on the
`Advanced Options` button.

For this example, we'll use a `n1-standard-64` notebook instance that has 16
vCPUs and 60 GB RAM by setting the following machine configuration in the
`Advanced Options` page:

<img src="/images/medium-scale-advanced-options.png" width="600px" style="display: block; margin-left: auto; margin-right: auto;" alt="Specifying a machine configuration in GCP Vertex AI Workbench">

Once the notebook instance is running, click on the `Open JupyterLab` button to
view the notebook environment in your browser.

## Step 2: Clone the repository

From within the notebook environment, open a new terminal window and clone the
repository with these examples by running the following command:

```shell
git clone https://github.com/koverholt/scaling-python-on-gcp
```

## Step 3: Install dependencies

Change to the `scaling-python-on-gcp` directory by running:

```shell
cd scaling-python-on-gcp
```

Install the Python packages in this repository by running:

```shell
pip install -r requirements.txt
```

## Step 4: Run the medium-scale notebook

Open the notebook located at
`scaling-python-on-gcp/2-medium-scale/satellite-imagery.ipynb` for this
medium-scale computation, which contains all of the remaining code that you need
to run for this example.

Run through all of the notebook cells to point to the satellite image data,
start a local Dask cluster on your machine, and compute and visualize the NDVI.

<img src="/images/medium-scale-notebook.png" width="1000px" style="display: block; margin-left: auto; margin-right: auto;" alt="Running the medium-scale satellite imagery notebook">

## Success!

Congratulations! 🎉 You've successfully run the medium-scale computation example
and calculated the normalized difference vegetation index (NDVI) on 10 satellite
images from a notebook instance within GCP Vertex AI Workbench.

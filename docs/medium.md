# Medium-scale Computations

## Prerequisites

- Clone this repository
- Install the Python packages in this repository by running `pip install -r requirements.txt`.
- Create a notebook in Vertex AI on GCP
- Create a Kubernetes cluster in GKE on GCP

## Use case

The notebooks in this repository are used to demonstrate how to scale Python on
GCP for image processing on satellite data. Specifically, these notebooks
compute the normalized difference vegetation index (NDVI) on Landsat 8 satellite
images using XArray and Dask.

Thanks to the open data policies of USGS and NASA,
the Landsat dataset is available for free as part of the Google Public Cloud
Data program. It can be used by anyone as part of Google Cloud.

## Multiple scales

The notebooks for this use case exercise Dask and XArray at three different
scales:

1. Small-scale computations on a laptop (10s of satellite images)
2. Medium-scale computations on a virtual machine (100s of satellite images)
3. Large-scale computations on a Kubernetes cluster (1,000s of satellite images)

## Additional resources

Refer to the respective projects and documentation for more information about
[Dask](https://dask.org/), [XArray](https://xarray.pydata.org/en/stable/),
[Dask Kubernetes](https://kubernetes.dask.org),
[GCP](https://cloud.google.com/), and the publicly available
[Landsat data on GCP](https://cloud.google.com/storage/docs/public-datasets/landsat).

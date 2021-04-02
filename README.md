# na-cordex-aws
Examples of analysis of NA-CORDEX data publicly available on Amazon S3 (us-west-2 region) using xarray and dask


### Installing and Running the Notebook(s)
For those interested in running the notebook(s) in this repo, the file `environment.yml` contains a conda environment description that
should work for running on the NCAR supercomputers.   If running outside of NCAR, you should be able to make minor modifications to this file to suit your needs.

If your machine does not have the conda package manager installed, see instructions at https://docs.conda.io/en/latest/miniconda.html for installing conda within your user environment.

To create the environment, assuming conda is available already, clone this repo to your preferred machine for running the notebook and create the conda environment:

```
# Create your own copy of the files in this repository
git clone https://github.com/NCAR/na-cordex-aws.git

# Change directory into the cloned repo
cd na-cordex-aws

# Create the conda environment.
conda env create -f environment.yml
```

NOTE: the conda environment install may require > 1GB of disk space;  add the option `-p <install_path>` to the `conda create` command
to change the installation folder.

# Writing an efficient code for GeoPandas and Shapely in 2023

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/martinfleis/efficient-geopandas-workshop/main?urlpath=lab/)

## Setting up to follow the workshop

### Step 1: Download the workshop material

If you are a git user, you can get the workshop materials by cloning this repo:

```sh
git clone https://github.com/martinfleis/efficient-geopandas-workshop.git
cd efficient-geopandas-workshop
```

Otherwise, to download the repository to your local machine as a zip-file,
click the `download ZIP` on the repository page
<https://github.com/martinfleis/efficient-geopandas-workshop>
(green button "Code"). After the download, unzip on the location you prefer
within your user account (e.g. `My Documents`, not `C:\`).

### Step 2: Install the required Python packages

To follow the workshop, we recommend creating a `conda` environment to
ensure you have all the required packages installed (the
[environment.yml](environment.yml) file list the required packages).

If you do not yet have `conda` installed, you can install miniconda
(<https://conda.io/miniconda.html>) or the (larger) Anaconda distribution
(<https://www.anaconda.com/download/>).

Using conda, we recommend to create a new environment with all packages using
the following commands (after cloning or downloading this GitHub repo and
navigating to the directory, see above):

```bash
# setting the configuation so all packages come from the conda-forge channel
conda config --add channels conda-forge
conda config --set channel_priority strict
# mamba provides a faster implementation of conda
conda install mamba
# creating the environment
mamba env create --file environment.yml
# activating the environment
conda activate geopandas-workshop
```

In case you do not want to install everything and just want to try out the course material, use the environment setup by Binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/martinfleis/efficient-geopandas-workshop/main?urlpath=lab/) and open the notebooks right away.

### Step 3: starting Jupyter Lab

The workshop itself is a [Jupyter notebook](http://jupyter.org/), an interactive environment to write and run code.

In the terminal, navigate to the `efficient-geopandas-workshop` directory (downloaded or cloned in the previous section)

Ensure that the correct environment is activated.

```sh
conda activate geopandas-workshop
```

Start a jupyter notebook server by typing

```sh
jupyter lab
```

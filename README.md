# cool-gliders
Python tools and scripts for searching and interacting the 
[Rutgers University Coastal Ocean Observing Lab's glider data API](https://marine.rutgers.edu/cool/data/gliders/api/).

# What Can You Do With This Package?

1. Search the [deployments API](https://marine.rutgers.edu/cool/data/gliders/api/) for deployments by:
   - Bounding Box
   - Time Range
   - Glider
   - Project
   - Active Deployments
2. Create a kml file displaying the tracks found for the search.
3. Create static global and zoomed in maps of tracks for the search.

Full documentation can be found on [the wiki](https://github.com/rucool/cool-gliders/wiki)

# Installation

1. Clone the repo
    > clone https://github.com/rucool/cool-gliders.git

2. Create the conda environment
    > conda env create -f environment.yml

3. Modify the path(s) in [env_vars.sh](https://github.com/rucool/cool-gliders/blob/main/env_vars.sh) and place it in:

    ${HOME}/miniconda3/envs/gliders/etc/conda/activate.d

This will store the current PYTHON_PATH paths in OLDPYTHON_PATH and add the paths in the file to PYTHON_PATH when the 
environment is activated. You can create another env_vars.sh and place it in:

    ${HOME}/miniconda3/envs/gliders/etc/deactivate.d

to set PYTHON_PATH to OLDPYTHON_PATH and unset OLDPYTHON_PATH. This will result in setting the PYTHON_PATH back to the 
paths prior to activating the environment.


# README for LADDMS data tutorial
Last updated: 18 August 2024
https://ndot-laddms.org

## Requirements

### Python environment
Use the `requirements.txt` file included in this repository to set up a Python environment with the necessary dependencies for the code. The recommended/verified Python version for this tutorial is 3.10. If you are using Anaconda, the environment setup can be performed with the following commands (executed from the working directory of the tutorial files): 
`conda create -n "laddms_tutorial" python=3.10`
`conda activate laddms_tutorial`
`pip install -r requirements.txt`

### Data files
The example trajectory data snippet should be downloaded from http://vu.edu/laddms-data-snippet. This data file should be placed in the same directory as the tutorial notebook and other files.

## Running the tutorial
Open the tutorial notebook `basic_data_tutorial.ipynb` by activating the Python environment (`conda activate laddms_tutorial`) and running Jupyter Lab notebook server with the terminal command `jupter lab`.

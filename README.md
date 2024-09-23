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
The example trajectory data snippet should be downloaded from [https://vu.edu/laddms-data-snippet](https://vu.edu/laddms-data-snippet). This data file should be placed in the same directory as the tutorial notebook and other files.

The data snippet is taken from an undisclosed day and time along the LADDMS corridor. Trajectory timestamps are internally consistent within the data. Data is provided in UTM coordinates to facilitate more straightforward local spatial analysis, using the Cartesian projection. The data may be converted back to WGS84 latitude/longitude when needed.

The following fields are included in each trajectory:
- object_id : Unique object ID number; only guaranteed unique within each location.
- location_id : Location ID number assigned within the database, corresponding to order of installations within the LADDMS corridor.
- classification : lidar-generated object classification (e.g., VEHICLE, LARGE_VEHICLE, PERSON, BICYCLE, UNKNOWN).
- sub_classification : lidar-generated object sub-classification.
- obj_length : Average length in meters across the trajectory.
- obj_width : Average width in meters across the trajectory.
- obj_height : Average height in meters across the trajectory.
- avg_filtered_confidence :  Classification confidence after filtering trajectory data points with < 0.5 confidence.
- ts :  Normalized within the dataset to 0-minimum to preserve data anonymity.
- vel_x : Velocity X component time series in m/s.
- vel_y : Velocity Y component time series in m/s.
- utm_x : Local UTM X coordinate time series (meters).
- utm_y : Local UTM X coordinate time series (meters).

## Running the tutorial
Open the tutorial notebook `basic_data_tutorial.ipynb` by activating the Python environment (`conda activate laddms_tutorial`) and running Jupyter Lab notebook server with the terminal command `jupyter lab`.

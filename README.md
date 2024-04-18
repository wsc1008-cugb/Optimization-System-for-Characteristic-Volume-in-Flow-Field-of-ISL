# Optimization-System-for-Characteristic-Volume-in-Flow-Field-of-ISL
This repository contains the code and data for the project. Below is an overview of the files and their purposes:

## Files
The flow field volume calculation method of ISL has been included in two source code files.
### C13-test_MODFLOW_text.zip

This compressed file contains the modflow basic file of the groundwater flow model created earlier. In order for subsequent programs to run normally, this set of files is necessary, and users can also create them themselves using flopy.

### time-C13.txt

The user enters the target time for subsequent ISL flow field simulation calculation and optimization in this text file, which can include several time nodes.

### inwell-C13.txt

"IJK" coordinates of injection well

### puwell-C13.txt

"IJK" coordinates of pumping well

### ore.txt

Ore body range. Can be calculated using geostatistical programs or manually delineated.

### SOO.ipynb

This notebook contains the calculation method for generating cell.txt and in.txt files according to MODPATH7 (that is, the original file for calculating the flow field volume), and also includes the set operation process of the flow field volume, and finally performs particle calculation within a given range. Single-target optimization of delivery methods. Determine the optimal number of particles to be placed in different directions when calculating the in.txt file

### SA.ipynb

Based on the single-objective optimization results, sensitivity analysis of the number of particles dropped in different directions is performed.

### MOO.ipynb

This notebook contains the calculation method for generating cell.txt and in.txt files according to MODPATH7 (that is, the original file for calculating the flow field volume). Based on the single-objective optimization results of the particle delivery plan, the multi-objective optimization model of the liquid pumping volume-flow field external influence range is solved.

## Usage

To run the above program correctly, you need to include the mf2005.exe and mp7.exe solvers for calling 

For any questions or inquiries, please contact [a19971008z@163.com].




## Content
# [<img alt="lifex" width="150" src="https://gitlab.com/lifex/lifex/-/raw/main/doc/logo/lifex.png" />](https://lifex.gitlab.io/lifex/)
This repository contains the example files needed to run some test cases for the
1D simulation of the hemodynamics in a vessels network.
Those files are supposed to be used within the **<kbd>life<sup>x</sup></kbd>**
(/,laɪfˈɛks/) library.

## Tests list
The available tests are:
1. Single vessel;
2. Single vessel with stent implanted;
3. Single vessel with stent implanted and adaptive mesh;
4. Bifurcation of a single vessel.

Each folder contains:
 - a subfolder **vessel_prm_files**, which has in it the 
 **<kbd>.prm</kbd>** input files for the vessel instances;
 - a **<kbd>.vtk</kbd>** file containing the topology of the network;
 - a **<kbd>.prm</kbd>** file named as the test folder;
 - a **<kbd>result.zip</kbd>** which stores the output of those very same simulations.

After installing and compiling **<kbd>life<sup>x</sup></kbd>**, you can copy and paste
the folder of a test case **in the same path** of the executable
**<kbd>lifex_example_vessels_network_1D</kbd>**. Then you can launch the simulation with
```
./lifex_example_vessels_network_1D -f 1-single_vessel/single_vessel.prm -o 1-single_vessel_output
```
This starts the first simulation and saves the output files within the folder
**<kbd>1-single_vessel_output</kbd>**. Then you can compare them with the results provided,
for example in ParaView.

## Get the software
To download, install or use **<kbd>life<sup>x</sup></kbd>**, please refer to
the [user guide and documentation](https://lifex.gitlab.io/lifex/).

## Referencing **<kbd>life<sup>x</sup></kbd>**
If you use the results obtained with the help of **<kbd>life<sup>x</sup></kbd>**,
please cite [this](https://doi.org/10.48550/arXiv.2207.14668) reference or one of the 
publications listed [here](https://lifex.gitlab.io/lifex/publications.html).

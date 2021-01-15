This readme.txt file helps the reader to understand the organization of the provided velocity and bed topography/water level data.

All data are stored as ".mat" (Matlab supported files). There are 2 types of data.

1. The mean velocity and mean turbulence kinetic energy data 

These data are organized by lateral cross-sections (as they were measured by ADV Vectrino probe).

The origin of the selected coordinate system in the horizontal plane (x−y) is the upstream junction corner of the confluence (X=0.00; Y=0.00), 
whereas the top of the bed sill was used as the origin of the vertical (z) axis, as described in the manuscript.

For instance, file name "section_uvw_x_0150.mat" indicates that this data was measured along the lateral cross-section X=-1.50, 
or 1.50 m upstream of the upstream juntion corner.

Each file contains the matrices of mean velocities ("U"-longitudinal,"V"-transversal, and "W"-vertical velocity components) and mean TKE data ("kinerg").
"X", "Y", "Z" are longitudinal, transversal and vertical coordinates (in meters), respectively.
The data is organized from top to bottom and from left to right. 
This means that the cell (1,1) corresponds to the point measured near the water surface and in the close vicinity of the right bank.

NaN values indicate either the proximity to the bed (they follow the irregularities of the bed topography), 
or the points that have been discarded from the analysis (poor signal, errors, etc.).

2. The bed topography and water surface maps

These data are stored in the file "topo_water_level_maps.mat". 

Since the bed topography and water surface level were acquired by different types of probes, 
the horizontal coordinates X and Y for these data are stored as different variables.

"Xtopo" - the matrix of longitudinal coordinates of the selected bed topography points;
"Ytopo" - the matrix of transversal coordinates of the selected bed topography points;
"Ztopo" - the matrix of bed topography elevations (vertical position with respect to the origin of the coordinate system);

"Xwl" - the matrix of longitudinal coordinates of the selected water surface points;
"Ywl" - the matrix of transversal coordinates of the selected water surface points;
"Zwl" - the matrix of water surface elevations (vertical position with respect to the origin of the coordinate system).

The velocity and bed topography/water level data share the same coordinate system.








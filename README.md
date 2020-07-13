# largescaleuavdataset
# A large-scale UAV dataset for image understanding, multi-view 3D reconstruction, and geo-localization
We present a large-scale UAV dataset with simulated UAV image sequences in urban areas and automatically generated pixel-level annotations for depth, surface normals, semantics, and edges of buildings in urban areas from an open CityGML model.

CityGML, as an open data model for the storage and exchange of virtual semantic 3D
city models, could serve as a useful source for deriving ground-truth semantic, geometric and topological information of geographical objects. It has 5 levels of details(LoDs), see https://de.wikipedia.org/wiki/Level_of_Detail.

We make use of the 3D city model of the Berlin city area published by the state of Berlin and its Senate Department for Economics, Technology and Research https://daten.berlin.de/tags/3d-stadtmodell.


We simulate UAV image sequences in Google Earth Studio, align parameters and derive annotations in Blender. For more details, please check our paper http://paperwillbepublishedinICPR.

![ ](simulateandrender.gif)

## Download
We share the simulated dataset with automatically generated annotations (depth, semantics, edges, surface normals) together with source codes as well as blender files. The dataset contains 144000 UAV images over 15 areas distributed in Berlin.
Three different scenarios are considered for simulation:
- the UAV flies at constant speed and with constant viewing
angle (dataset1)
- the UAV flies at constant speed with viewing angles
changing linearly (dataset2)
- the UAV flies at changing speeds with changing viewing
angles (dataset3)

For ground-truth annotations, numpy files are provided for each attribute of each frame: 
- depth (depth values of float type [270,480])
- surface normals (normal values of float type  [270,480,3])
- edges (binary files [270,480])
- semantics (semantic classes of integer type [270,480])
  1-wall, 2-flat roof, 3-tilted roof, 4-complicated roof, 5-ground, 0-unclassified



## Citation

please cite the following paper if you want to use either the dataset or the source codes/files.

## License

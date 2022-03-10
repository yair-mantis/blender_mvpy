# blender_mvpy
WIP of blender integration

how would mantis blnder integration look like?  
can we use renderer, caching, pointcloud, timeline  

how do we contribute, [addon](https://docs.blender.org/manual/en/latest/advanced/scripting/addon_tutorial.html), plugin, filter, node, 
### openVDB
[openVDB](https://github.com/AcademySoftwareFoundation/openvdb)
>It's a framework called OpenVDB [1], which we use to represent and manipulate volumetric data (level sets). It stores the data as a sparse hierarchical grid with (from a practical perspective) infinite dimensions, and allows very efficient iteration and local manipulations of the grid.
I'm not an expert on how it is implemted exactly, but I believe the way it uses Blosc is by saving leaves of the VDB grids in blosc-compressed chunks, which are loaded into memory directly and only decompressed on-demand when the data is accessed, then re-compressed when the leaves are processed.
[1] https://www.openvdb.org/

https://youtu.be/4QMuXQH_5ZA

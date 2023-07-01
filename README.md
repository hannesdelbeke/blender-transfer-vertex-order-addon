# Transfer vertex order  <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Blender-Dark.svg" width="32" style="max-width: 100%;">  Blender addon

 


 ! Prevent this | Vert transfer addon |
 | -- | -- |
 |  <img src="https://github.com/hannesdelbeke/blender-transfer-vertex-order-addon/assets/3758308/f497c5bd-f28b-4680-b971-cb35ab6ebd0b" height="200" style="max-width: 100%;">  | <img src="https://github.com/hannesdelbeke/blender-transfer-vertex-order-addon/assets/3758308/444103d3-64e2-4384-84bb-f048db2999d1" height="150" style="max-width: 100%;">    |

Transfer vert ID from one mesh to another in Blender 2.8+.<br>
This repo is a mirror of bartoszstyperek's script.<br>
Support the original author by buying his ⭐⭐⭐⭐⭐ 160+ reviews script on [GumRoad](https://bartoszstyperek.gumroad.com/l/copy_verts_ids)

## instructions
Addon will be located in right 3d View Sidebar(N) -> Tools panel

See video tutorial about addon made by Danny Mac 3D [here](https://www.youtube.com/watch?v=qTgSLYY9uew&t=1s).


This blender addon makes it possible to transfer the vertex order (face and edge too since 2.2 update), from mesh  A to mesh B, if both of them have the same topology (same vertex count, same polygon count).

With vert order copied you will be able to transfer mesh attributes like uv, weights, colors etc. by using Data Transfer modifier (and using'Topology' vertices matching).

For vert id transfer, if two meshes have same vertices position, you can use object mode 'ctrl+c' menu -> Transfer vert ID by vert proximity. Just select target object(s), then source mesh and use ctrl+c to transfer ids from source mesh to target mesh.

If two meshes have different vertices positions use editmode ctrl+c menu - Copy vert ID topological. First you need to select two, adjacent faces on source mesh - copy mesh id's with ctrl+c menu, and then, select two similar faces on target mesh and  paste IDs. Operation has to be repeated for each island (disconnected mesh parts)  separately.

Since version 2.3 now there is also option to Transfer vert IDs using matching UVs.


## Dependencies
This addon is using 'Copy Attributes Menu' addon, which is build-in into blender.

You can preview vert IDs by using MeasureIt addon (also build-in into blender).

This addon is base on Magic UV - UV Topological transfer script.


## Release notes

#### Update 2.1 and 1.1 for both  Blender 2.8 and 2.79 (13.06.2019):
- massive speed bump on high-poly meshes (thx. to zagzag)

#### Update 2.2 (blender 2.8 only)
- from now on all data is transfered (vertices ids, face ids, edge ids)

#### Update 2.3 ( 13.05.2022)
- New option to transfer Vert IDs using matching UVs


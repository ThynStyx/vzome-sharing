---
title: Plato's Solids
image: https://ThynStyx.github.io/vzome-sharing/2022/06/24/18-06-22-Platonics-hull/Platonics-hull.png
layout: vzome
description: 
 All Plato's solids exist within the same 3D convex hull and have their vertices on the same spherical surface.
---  

Selected Solid =
<select>
    <option value="https://ThynStyx.github.io/vzome-sharing/2022/04/30/22-59-09-Platonics-skeleton/Platonics-skeleton.vZome" >Skeleton</option>
    <option value="https://ThynStyx.github.io/vzome-sharing/2022/04/30/21-37-13-Platonics-hull/Platonics-hull.vZome" selected>Hull</option>  
    <option value="https://ThynStyx.github.io/vzome-sharing/2022/04/30/22-20-21-Platonics-Tetrahedron/Platonics-Tetrahedron.vZome" >Tetrahedron</option> 
    <option value="https://ThynStyx.github.io/vzome-sharing/2022/04/30/22-22-16-Platonics-Cube/Platonics-Cube.vZome" >Cube</option>
    <option value="https://ThynStyx.github.io/vzome-sharing/2022/04/30/22-16-13-Platonics-Octahedron/Platonics-Octahedron.vZome" >Octahedron</option>
    <option value="https://ThynStyx.github.io/vzome-sharing/2022/04/30/22-12-48-Platonics-Icosahedron/Platonics-Icosahedron.vZome" >Icosahedron</option>
    <option value="https://ThynStyx.github.io/vzome-sharing/2022/04/30/22-09-54-Platonics-Dodecahedron/Platonics-Dodecahedron.vZome" >Dodecahedron</option>
</select>

<figure style="margin:5%">
  <vzome-viewer id="viewer" style="width: 87%; height: 60vh;"
      src="https://ThynStyx.github.io/vzome-sharing/2022/04/30/21-37-13-Platonics-hull/Platonics-hull.vZome" >
    <img id="image" src="https://ThynStyx.github.io/vzome-sharing/2022/04/30/21-37-13-Platonics-hull/Platonics-hull.png" />
  </vzome-viewer>
  <figcaption style="text-align: center; font-style: italic;">Plato's 5 solids in their 3D hull (30-gon field).</figcaption>
</figure>

<script>
document.querySelector("select").addEventListener("input", (e) => {
  console.log( e.target.value );
  document.querySelector("vzome-viewer").src = e.target.value;
})	
</script>
Using the appropriate packing pieces, each of Plato's solid can be fitted into the same 3D hull.

The colouring of the 3D hull is the same for each model and on loading all the models are aligned in the same way and at the same scale.

There are actually multiple alignments available for positioning Cubes, Octahedra, Icosahedra and Tetrahedra within the hull.

The Tetrahedron model requires 4 "packing pieces" to permit the Tetrahedron to be fitted/extracted within the hull in a physical model.
(The other models can be built/disassembled using only two pieces.)

Only one example of each solid has been selected to keep these representations as simple as possible.  The alternatives could be found in the physical model by rotating the "packing pieces" within the trackball hull.

With thanks to Scott Vorthmann, John Kostick and David Hall.

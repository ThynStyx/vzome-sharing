---
title: The Platonic Solids
image: https://ThynStyx.github.io/vzome-sharing/2022/02/05/14-05-27-Platonic-Solids/Platonic-Solids.png
layout: vzome
---

{% comment %}
 - [***web page generated from this source***][post]
 - [data assets and more info][github]

[post]: <https://ThynStyx.github.io/vzome-sharing/2022/02/05/Platonic-Solids-14-05-27.html>
[github]: <https://github.com/ThynStyx/vzome-sharing/tree/main/2022/02/05/14-05-27-Platonic-Solids/>
{% endcomment %}

{{ page.description }}
There are actually multiple Cubes, Octahedra and Tetrahedra available within the hull. 
Only one example of each solid has been chosen to keep the skeleton as simple as possible.  However this does compromise the symmetry.

<html lang="en">
 <head>
  <meta charset="utf-8">
  <title>vZome Platonic Solids multi-viewer</title>
  <meta property="og:title" content="The Platonic Solids" />
  <meta property="og:locale" content="en_US" />
  <script>
  const sources = [
 "https://ThynStyx.github.io/vzome-sharing/2022/01/26/21-59-17-Keplers-Kosmos-Skeleton-only/Keplers-Kosmos-Skeleton-only.vZome",
 "https://ThynStyx.github.io/vzome-sharing/2022/01/26/21-30-34-Keplers-Kosmos-Tetrahedron-only/Keplers-Kosmos-Tetrahedron-only.vZome",
 "https://ThynStyx.github.io/vzome-sharing/2022/01/26/11-12-12-Keplers-Kosmos-Cube-only/Keplers-Kosmos-Cube-only.vZome",  
 "https://ThynStyx.github.io/vzome-sharing/2022/01/26/21-48-24-Keplers-Kosmos-Octahedron-only/Keplers-Kosmos-Octahedron-only.vZome",
 "https://ThynStyx.github.io/vzome-sharing/2022/01/26/21-25-59-Keplers-Kosmos-Icosahedron-only/Keplers-Kosmos-Icosahedron-only.vZome",
 "https://ThynStyx.github.io/vzome-sharing/2022/01/26/21-57-10-Keplers-Kosmos-Dodecahedron-only/Keplers-Kosmos-Dodecahedron-only.vZome"  
  ];
  function prevButton() {
	stepSource(-1);
  }

  function nextButton() {
	stepSource(1);

  }

  function stepSource(step) {
	  const src = document.getElementById("viewer").src;
	  for (let i = 0; i < sources.length; i++) {
		if(src == sources[i]) {
			setSource(i + step);
			break;
		}	  
	  }
  };

  function setSource(index) {
	const viewer = document.getElementById("viewer");
	viewer.src = sources[(index + sources.length) % sources.length];
  }
  </script>
  
 </head>
 <body>
	<button type="button" onclick='prevButton()'><< Previous solid </button>
	<button type="button" onclick='nextButton()'>Next solid >></button>
	<br /> 
	<button type="button" onclick='setSource(0)'>Hull Skeleton </button>
	<button type="button" onclick='setSource(1)'>Tetrahedron Solid</button>
	<button type="button" onclick='setSource(2)'>Cube Solid </button>
	<button type="button" onclick='setSource(3)'>Octahedron Solid </button>
	<button type="button" onclick='setSource(4)'>Icosahedron Solid </button>
	<button type="button" onclick='setSource(5)'>Dodecahedron Solid </button>
  
	<p> 
	Notice that the camera position and zoom level are retained when the model is changed!
	</p>
	
        <!-- Enable the vzome-viewer custom element -->	 
        <script type="module" src="https://www.vzome.com/modules/vzome-viewer.js"></script>
	<vzome-viewer id="viewer" style="width: 100%; height: 65vh;" src="https://ThynStyx.github.io/vzome-sharing/2022/01/26/21-59-17-Keplers-Kosmos-Skeleton-only/Keplers-Kosmos-Skeleton-only.vZome" >
	<img id="image" src="https://ThynStyx.github.io/vzome-sharing/2022/01/26/21-59-17-Keplers-Kosmos-Skeleton-only/Keplers-Kosmos-Skeleton-only.png" />
	</vzome-viewer>

</body>
</html>

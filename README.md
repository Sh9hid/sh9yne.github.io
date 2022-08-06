# sh9yne.github.io
_Learning to use github pages from the official docs_

# What I learned today: 
 *Creating 3D objects on 3JS and Normal Mapping**
>
Added our texture with the texture loader function in 3Js and we load a mesh after that. Then, we give that mesh some material and geometry. We create our object and map the texture with the map property and then for our moon we added a normal mapping texture on top that allows craters and dents to be reflected by the light.
<sub>
Here's the code I was working on:

 //Texture loader to load an image
  const PlanetText = new THREE.TextureLoader('SEA.jpg');
  //Then we load a mesh 
  const PlanetText = new.THREE.Mesh(
    //Then we give our sphere a basic sphere geometry and a material
    new THREE.SphereGeometry(3, 3, 3),
    new THREE.MeshStandardMaterial ({map:PlanetText})
    // map property on the material as the texture
    scene.add(Planet);
  
  // That's cool, but we need our closest satellite, the moon 
  //we'll add the texture as the moon jpg and add the map property
  
  const moonText = new THREE.TextureLoader().load('moonz.jpg')
  //we also add a normal mapping texture that allows light to bounce off to create an illusion of craters and mountains
  const normalText = new THREE.TextureLoader().load('normalmap.jpg')

  const MOON = new THREE.Mesh(
    new THREE.SphereGeometry(3 , 32, 32), // with a radius of three
    new THREE.MeshStandardMaterial ( {
      map : moonText,
      normalMap: normalText
      } )
  );
    scene.add(MOON);                                                                  
                                    
</sub>
>Trying ThreeJs and there is the scene, camera, renderer and a lot more learnt including this page formatting. Don't how well, it went or supposed to go 🧑‍🎓
![what I learned today at Aug, 6, 2022](https://upload.wikimedia.org/wikipedia/commons/9/9a/%E0%B9%80%E0%B8%9B%E0%B8%A3%E0%B8%B5%E0%B8%A2%E0%B8%9A%E0%B9%80%E0%B8%97%E0%B8%B5%E0%B8%A2%E0%B8%9A%E0%B9%82%E0%B8%A1%E0%B9%80%E0%B8%94%E0%B8%A5%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B9%83%E0%B8%8A%E0%B9%89_normal_map.png)



_is is my first commit on a personal project on Github pages. _

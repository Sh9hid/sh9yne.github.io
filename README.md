# ONE DAY, THREE JS
![what I learned today at Aug, 6, 2022](https://upload.wikimedia.org/wikipedia/commons/9/9a/%E0%B9%80%E0%B8%9B%E0%B8%A3%E0%B8%B5%E0%B8%A2%E0%B8%9A%E0%B9%80%E0%B8%97%E0%B8%B5%E0%B8%A2%E0%B8%9A%E0%B9%82%E0%B8%A1%E0%B9%80%E0%B8%94%E0%B8%A5%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B9%83%E0%B8%8A%E0%B9%89_normal_map.png)



## What I learned today: 

*Learning to use github pages from the official docs. Creating 3D objects using 3JS and concepts like Normal Mapping.*


> Added our texture with the texture loader function in 3Js and we load a mesh after that. Then, we give that mesh some material and geometry. We create our object and map the texture with the map property and then for our moon we added a normal mapping texture on top that allows craters and dents to be reflected by the light.
 
> Here's the code I was working on:

 > Texture loader to load an image.
 
  const PlanetText = new THREE.TextureLoader('SEA.jpg');
  
 > Then we load a mesh.
 
  const PlanetText = new.THREE.Mesh(
  
  > Then we give our sphere a basic sphere geometry and a material
   
   new THREE.SphereGeometry(3, 3, 3),
   new THREE.MeshStandardMaterial ({map:PlanetText})
  >  map property on the material as the texture
   scene.add(Planet);
    That's cool, but we need our closest satellite, the moon. We'll add the texture as the moonz jpg and add the map property to map 3d objects to our jpgs and later on add another texture to make it look more realistic.
  
  const moonText = new THREE.TextureLoader().load('moonz.jpg')
  
  
 > we also add a normal mapping texture that allows light to bounce off 
> to create an illusion of craters and mountains

  const normalText = new THREE.TextureLoader().load('normalmap.jpg')
  const MOON = new THREE.Mesh(
  
 > with a radius of three

new THREE.SphereGeometry(3 , 32, 32), 
new THREE.MeshStandardMaterial ( {
   map : moonText,
   normalMap: normalText
     } )
  );
  scene.add(MOON);                                                                
                                    
> Trying ThreeJs and there is the scene, camera, renderer and a lot more learnt including this page formatting. 
> Don't how well, it went or supposed to go 🧑‍🎓

## sh9yne.github.io

>Made with 💜 by sh9 😸

_This is a test! Don't believe everything you read on the internet_

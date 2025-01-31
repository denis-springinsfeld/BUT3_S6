# BUT3_S6

## Test

https://denis-springinsfeld.github.io/BUT3_S6/

## Google Sheet pour vos liens

https://docs.google.com/spreadsheets/d/1Ly7VBCWj0yJb8mM23XbKz0hqFLzxJTH5NuOIlaisgOc/edit?gid=1665760473#gid=1665760473


## Codes

### Mixin

```html
<a-assets>
  <a-mixin id="fire-truck-rig" gltf-model="url(https://assets.3dstreet.app/sets/vehicles-rig/gltf-exports/draco/fire-truck-pumper-rig.glb)"></a-mixin>
</a-assets>

<a-entity position="0 0 -9" mixin="fire-truck-rig"></a-entity>
```

```html
<a-scene>
  <a-assets>
    <a-asset-item id="ftruck-model" src="https://assets.3dstreet.app/sets/vehicles-rig/gltf-exports/draco/fire-truck-pumper-rig.glb"></a-asset-item>
    <a-mixin id="fire-truck-loaded" gltf-model="#ftruck-model"></a-mixin>
  </a-assets>

  <a-entity position="-2 0 -9" mixin="fire-truck-loaded"  scale="0.1 0.1 0.1">
</a-scene>
```


## Collisions

```html
<html>
  <head>
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta http-equiv="content-type" content="text/html; charset=utf-8" />
    <meta
      name="viewport"
      content="width=device-width,initial-scale=1,shrink-to-fit=no,user-scalable=no,maximum-scale=1"
    />
    <title>Examples • Castle</title>
    <script src="https://aframe.io/releases/1.6.0/aframe.min.js"></script>
    <script src="https://cdn.jsdelivr.net/gh/c-frame/aframe-extras@7.5.4/dist/aframe-extras.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/aframe-environment-component@1.3.7/dist/aframe-environment-component.min.js"></script>
  </head>
  <body>
    <a-scene environment="preset: forest; lighting: point; lightPosition: -5 10 0;"> 
      <a-assets>
       <!-- Zone de Collision. -->
        <a-asset-item
          id="navmesh"
          src="../assets/castle/Castle-navmesh5.glb"
        ></a-asset-item>
       <!-- Modèle 3D. -->
        <a-asset-item
          id="castle"
          src="../assets/castle/Castle.glb"
        ></a-asset-item>
      </a-assets>

      <!-- Player. -->
      <a-entity id="rig" movement-controls="constrainToNavMesh: true;">
        <a-entity
          camera
          position="0 1.6 0"
          look-controls="pointerLockEnabled: true"
        >
          <a-cursor></a-cursor>
        </a-entity>
      </a-entity>

      <!-- Nav mesh. -->
      <a-entity
        nav-mesh
        normal-material
        visible="false"
        position="0 0 20"
        gltf-model="#navmesh"
      ></a-entity>

      <!-- Scene. -->
      <a-entity
        position="0 0 20"
        scale="3 3 3"
        gltf-model="#castle"
        visible="true"
      >
      </a-entity>
    </a-scene>
  </body>


## Animation GLTF

https://github.com/rexraptor08/animation-controls?tab=readme-ov-file
</html>
```


https://github.com/MediaComem/VR-A-Frame/tree/master?tab=readme-ov-file

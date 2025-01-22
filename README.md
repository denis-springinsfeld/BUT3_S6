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

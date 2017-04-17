[查看演示](https://majieco.github.io/3d/example/demo/8.5.1.html)

```javascript
renderer = new THREE.WebGLRenderer();
renderer.shadowMapEnabled = true;
renderer.shadowMapSoft = true;

var plane = new THREE.Mesh(new THREE.PlaneGeometry(8, 8, 16, 16),
        new THREE.MeshLambertMaterial({color: 0xcccccc}));
plane.rotation.x = -Math.PI / 2;
plane.position.y = -1;
plane.receiveShadow = true;
scene.add(plane);

cube = new THREE.Mesh(new THREE.CubeGeometry(1, 1, 1),
        new THREE.MeshLambertMaterial({color: 0x00ff00}));
cube.position.x = 2;
cube.castShadow = true;
scene.add(cube);

var light = new THREE.SpotLight(0xffff00, 1, 100, Math.PI / 6, 25);
light.position.set(2, 5, 3);
light.target = cube;
light.castShadow = true;

light.shadowCameraNear = 2;
light.shadowCameraFar = 10;
light.shadowCameraFov = 30;
light.shadowCameraVisible = true;

light.shadowMapWidth = 1024;
light.shadowMapHeight = 1024;
light.shadowDarkness = 0.3;

scene.add(light);
```

* 设置透视投影照相机，这里Canvas长400px，宽300px，所以aspect设为400 / 300：

```javascript
var camera = new THREE.PerspectiveCamera(45, 400 / 300, 1, 10);
camera.position.set(0, 0, 5);
scene.add(camera);
```

* 设置一个在原点处的边长为1的正方体：

```javascript
var cube = new THREE.Mesh(new THREE.CubeGeometry(1, 1, 1),
        new THREE.MeshBasicMaterial({
            color: 0xff0000,
            wireframe: true
        })
);
scene.add(cube);
```

[查看演示](https://majieco.github.io/3d/example/demo/2.4.1.html)
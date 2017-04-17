* 例子：

```javascript
var camera = new THREE.OrthographicCamera(-2, 2, 1.5, -1.5, 1, 10);
camera.position.set(0, 0, 5);
scene.add(camera);
```

* 在原点处创建一个边长为1的正方体，为了和透视效果做对比，这里我们使用wireframe而不是实心的材质，以便看到正方体后方的边：

```javascript
var cube = new THREE.Mesh(new THREE.CubeGeometry(1, 1, 1),
        new THREE.MeshBasicMaterial({
            color: 0xff0000,
            wireframe: true
        })
);
scene.add(cube);
```

[查看演示](https://majieco.github.io/3d/example/demo/2.3.1.html)
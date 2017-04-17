* 聚光灯是一种特殊的点光源，它能够朝着一个方向投射光线。聚光灯投射出的是类似圆锥形的光线，这与我们现实中看到的聚光灯是一致的。

* THREE.SpotLight(hex, intensity, distance, angle, exponent)

```javascript
var cube = new THREE.Mesh(new THREE.CubeGeometry(1, 1, 1),
                    new THREE.MeshLambertMaterial({color: 0x00ff00}));

var light = new THREE.SpotLight(0xffff00, 1, 100, Math.PI / 6, 25);
light.target = cube;
```

[查看演示](https://majieco.github.io/3d/example/demo/8.4.1.html)


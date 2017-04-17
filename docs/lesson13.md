* 照相机（Camera）: 我们定义了一个透视投影的照相机，具体原理后面详细介绍

```javascript
var camera = new THREE.PerspectiveCamera(45, 4 / 3, 1, 1000);
camera.position.set(0, 0, 5);
scene.add(camera);
```

* 这里我们需要了解一下坐标系，WebGL和Three.js使用的坐标系是右手坐标系，看起来就是这样的：
![](http://www.hewebgl.com/attached/image/20130515/20130515134934_11.jpg?_=6007811)
* 添加物体: 我们要创建一个x、y、z方向长度分别为1、2、3的长方体，并将其设置为红色。

```javascript
var cube = new THREE.Mesh(new THREE.CubeGeometry(1, 2, 3),
        new THREE.MeshBasicMaterial({
            color: 0xff0000
        })
);
scene.add(cube);
```

* 上面涉及到geometry、material、Mesh obj等后面再详细说明
* 这里的长度是在物体坐标系中的，其单位与屏幕分辨率等无关，它就是一个虚拟空间的坐标系，1代表多少并没有实际的意义，而重要的是相对长度。
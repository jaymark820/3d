```javascript
new THREE.MeshBasicMaterial({
    color: 0xffff00,
    opacity: 0.75
});
```

将其应用于一个正方体（方法参见3.1节），效果为：[查看演示](https://majieco.github.io/3d/example/demo/4.1.1.html)

    - visible：是否可见，默认为true
    - side：渲染面片正面或是反面，默认为正面THREE.FrontSide，可设置为反面THREE.BackSide，或双面THREE.DoubleSide
    - wireframe：是否渲染线而非面，默认为false
    - color：十六进制RGB颜色，如红色表示为0xff0000
    - map：使用纹理贴图，详见4.5节

* Lambert材质（MeshLambertMaterial）:是符合Lambert光照模型的材质。Lambert光照模型的主要特点是只考虑漫反射而不考虑镜面反射的效果，因而对于金属、镜子等需要镜面反射效果的物体就不适应，对于其他大部分物体的漫反射效果都是适用的。

```javascript
new THREE.MeshLambertMaterial({
    color: 0xffff00
})
```

[查看演示](https://majieco.github.io/3d/example/demo/4.2.1.html)
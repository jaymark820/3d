* 阴影：在Three.js中，能形成阴影的光源只有THREE.DirectionalLight与THREE.SpotLight；而相对地，能表现阴影效果的材质只有THREE.LambertMaterial与THREE.PhongMaterial。因而在设置光源和材质的时候，一定要注意这一点。

```javascript
首先，我们需要在初始化时，告诉渲染器渲染阴影：
renderer.shadowMapEnabled = true;
然后，对于光源以及所有要产生阴影的物体调用：
xxx.castShadow = true;
对于接收阴影的物体调用：
xxx.receiveShadow = true;
```


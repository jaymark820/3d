* 同样地，可以指定emissive和ambient值，这里不再说明。下面就specular值指定镜面反射系数作说明。首先，我们只使用镜面反射，将高光设为红色，应用于一个球体：

```javascript
var material = new THREE.MeshPhongMaterial({
    specular: 0xff0000
});
var sphere = new THREE.Mesh(new THREE.SphereGeometry(3, 20, 8), material);
```



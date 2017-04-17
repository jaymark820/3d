* color是用来表现材质对散射光的反射能力，也是最常用来设置材质颜色的属性。除此之外，还可以用ambient和emissive控制材质的颜色。

* ambient表示对环境光的反射能力，只有当设置了AmbientLight后，该值才是有效的，材质对环境光的反射能力与环境光强相乘后得到材质实际表现的颜色。

* emissive是材质的自发光颜色，可以用来表现光源的颜色。单独使用红色的自发光：

```javascript
new THREE.MeshLambertMaterial({
    emissive: 0xff0000
})
```
效果如下：

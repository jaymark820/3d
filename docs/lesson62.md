* 平行光
* THREE.DirectionalLight(hex, intensity)
* 其中，hex是光源十六进制的颜色值；intensity是亮度，缺省值为1，表示100%亮度。此外，对于平行光而言，设置光源位置尤为重要。

```javascript
var light = new THREE.DirectionalLight();
light.position.set(2, 5, 3);
scene.add(light);
```


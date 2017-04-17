* 在JavaScript代码中定义一个init函数，在HTML加载完后执行：我们可以把绘制代码放在这里

* 一个典型的Three.js程序至少要包括渲染器（Renderer）、场景（Scene）、照相机（Camera），以及你在场景中创建的物体。这里只是简单示例，后面进一步详细讲解每一个部分。

* 渲染器（Renderer）：渲染器将和Canvas元素进行绑定

```javascript
var renderer = new THREE.WebGLRenderer({
    canvas: document.getElementById('mainCanvas')
});
```

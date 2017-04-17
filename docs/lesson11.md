* 如果想要Three.js生成Canvas元素，在HTML中就不需要定义Canvas元素

```javascript
var renderer = new THREE.WebGLRenderer();
renderer.setSize(400, 300);
document.getElementsByTagName('body')[0].appendChild(renderer.domElement);
```

* 我们可以使用下面的代码将背景色（用于清除画面的颜色）设置为黑色：

```javascript
renderer.setClearColor(0x000000);
```
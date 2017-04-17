### 三、第一个three.js程序

* 首先，在HTML的<head>部分，需要声明外部文件three.js。

```html
<head>
    <script type="text/javascript" src="js/three.js"></script>
</head>
```

* WebGL的渲染是需要HTML5 Canvas元素的，你可以手动在HTML的<body>部分中定义Canvas元素，或者让Three.js帮你生成。

```html
<body onload="init()">
    <canvas id="mainCanvas" width="400px" height="300px" ></canvas>
</body>
```

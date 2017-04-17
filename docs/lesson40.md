```javascript
THREE.TextGeometry(text, parameters)
```

其中，text是文字字符串，parameters是以下参数组成的对象：
    - size：字号大小，一般为大写字母的高度
    - height：文字的厚度
    - curveSegments：弧线分段数，使得文字的曲线更加光滑
    - font：字体，默认是'helvetiker'，需对应引用的字体文件
    - weight：值为'normal'或'bold'，表示是否加粗
    - style：值为'normal'或'italics'，表示是否斜体
    - bevelEnabled：布尔值，是否使用倒角，意为在边缘处斜切
    - bevelThickness：倒角厚度
    - bevelSize：倒角宽度

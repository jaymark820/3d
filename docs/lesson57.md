```javascript
var requestAnimationFrame = window.requestAnimationFrame 
        || window.mozRequestAnimationFrame
        || window.webkitRequestAnimationFrame
        || window.msRequestAnimationFrame;
window.requestAnimationFrame = requestAnimationFrame;

var scene = null;
var camera = null;
var renderer = null;

var id = null;

var stat = null;

function init() {
    stat = new Stats();
    stat.domElement.style.position = 'absolute';
    stat.domElement.style.right = '0px';
    stat.domElement.style.top = '0px';
    document.body.appendChild(stat.domElement);

    renderer = new THREE.WebGLRenderer({
        canvas: document.getElementById('mainCanvas')
    });
    scene = new THREE.Scene();

    id = requestAnimationFrame(draw);
}

function draw() {
    stat.begin();

    renderer.render(scene, camera);

    id = requestAnimationFrame(draw);

    stat.end();
}

function stop() {
    if (id !== null) {
        cancelAnimationFrame(id);
        id = null;
    }
}
```




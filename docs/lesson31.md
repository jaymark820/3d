* 球体（SphereGeometry）

```javascript
THREE.SphereGeometry(radius, segmentsWidth, segmentsHeight, phiStart, phiLength, thetaStart, thetaLength)
```

* 其中，radius是半径；segmentsWidth表示经度上的切片数；segmentsHeight表示纬度上的切片数；phiStart表示经度开始的弧度；phiLength表示经度跨过的弧度；thetaStart表示纬度开始的弧度；thetaLength表示纬度跨过的弧度。

* 首先，我们来理解下segmentsWidth和segmentsHeight。使用var sphere = new THREE.SphereGeometry(3, 8, 6)可以创建一个半径为3，经度划分成8份，纬度划分成6份的球体，如下图所示。

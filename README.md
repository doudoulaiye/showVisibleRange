# 展示可视域

为方便显示人或者设备的视野范围，改进了下代码

## 引入可视域
```javascript
import {ShowVisibleRange} from './ShowVisibleRange'
```
## 调用可视域
```javascript
// wr指视野宽度的角度
// hr指视野高度的角度
// 0.5 相机长度
let camrea = new THREE.PerspectiveCamera(wr,wr/hr,0.5,666)
//设置相机位置
camera.position.x = x
camera.position.y = y
camera.position.z = z
//设置相机的看的方向
camera.lookAt(new THREE.Vector3(x1,y1,z1))

let vr = new ShowVisibleRange(camera)

scene.add(vr)
```
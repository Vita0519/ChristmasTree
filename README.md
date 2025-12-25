# Magic Christmas Tree 🎄✨

一个基于 WebGL (Three.js) 和计算机视觉 (MediaPipe) 的交互式 3D 圣诞树体验。


## ✨ 特性 (Features)

* **沉浸式 3D 视觉**: 使用 Three.js 构建的粒子系统，包含金球、银块、红蓝宝石和辉光效果 (Bloom)。
* **AI 手势识别**: 集成 Google MediaPipe，无需任何穿戴设备，通过摄像头即可控制。
* **物理交互**:
    * ✊ **握拳 (Fist)**: 将星云粒子聚合成一棵旋转的圣诞树。
    * 🖐 **张手 (Open Palm)**: 粒子炸开成宇宙星云状态。
    * 👋 **挥动 (Wave)**: 在星云状态下，像拨动地球仪一样旋转视角（带有物理惯性）。
    * 👌 **捏合 (Pinch)**: 智能抓取并放大查看上传的照片。
* **回忆画廊**: 支持上传本地照片，照片会自动挂载在树上或漂浮在星云中。

## 🚀 快速开始 (How to Run)

### 方法 1: fork这个项目,顺手点颗✨增加开源动力（推荐）

开启 Pages: 进入仓库 Settings -> 左侧 Pages -> 在 Branch 处选择 main (或 master) -> 点击 Save。
访问: 等待几分钟，访问 https://你的用户名.github.io/仓库名/。

<img width="2402" height="1350" alt="image" src="https://github.com/user-attachments/assets/ccac4efd-803f-4c47-8e67-9b4e0ed3a2ed" />
<img width="2864" height="1536" alt="image" src="https://github.com/user-attachments/assets/ed5de940-02b5-45c7-99b7-5af57e63c617" />

方法 2: 直接本地双击html文件打开

## 🛠️ 技术栈 (Tech Stack)
- Three.js (r160): 核心 3D 渲染引擎。

- Three.js Post-processing: 用于实现辉光 (Bloom) 和色调映射 (Tone Mapping)。

- MediaPipe Hand Landmarker: 实时手部骨骼检测。

- HTML5/CSS3: 响应式布局与 UI 界面。

## ⚙️ 配置 (Configuration)
在代码顶部的 CONFIG 对象中可以调整视觉参数：
```bash
JavaScript

const CONFIG = {
    goldCount: 500,     // 金球数量
    bloomStrength: 0.7, // 辉光强度
    treeHeight: 75,     // 树的高度
    // ...
}; 
```
## 📝 注意事项
- 摄像头权限: 首次打开时浏览器会请求摄像头权限，请点击“允许”。

- 性能: 建议在带有独立显卡的 PC 或高性能手机上运行。代码已针对性能进行了优化（如手势检测节流），但在老旧设备上可能会有卡顿。
尝试解决办法：开启浏览器图形加速后重启浏览器，再打开
<img width="1583" height="741" alt="image" src="https://github.com/user-attachments/assets/e2baf57f-2cdd-428c-bb8c-9a62b84dee5b" />

- 环境光: 请确保您所处的环境光线充足，以便摄像头能准确识别手势。

<div align="center"><table><tbody><tr><td align="center"><b>个人QQ</b><br><img src="https://wmimg.com/i/1119/2025/02/67a96bb8d3ef6.jpg" width="250" alt="作者QQ"><br><b>QQ：154578485</b></td><td align="center"><b>QQ交流群</b><br><img src="https://github.com/user-attachments/assets/5f24482c-19fd-4aa5-8861-3a92a5fc5c79" width="250" alt="QQ群二维码"><br><small>群内会更新个人练手的python项目</small></td><td align="center"><b>微信赞赏</b><br><img src="https://wmimg.com/i/1119/2024/09/66dd37a5ab6e8.jpg" width="500" alt="微信赞赏码"><br><small>要到饭咧？啊咧？啊咧？不给也没事~ 请随意打赏</small></td><td align="center"><b>支付宝赞赏</b><br><img src="https://wmimg.com/i/1119/2024/09/66dd3d6febd05.jpg" width="300" alt="支付宝赞赏码"><br><small>如果觉得有帮助,来包辣条犒劳一下吧~</small></td></tr></tbody></table></div>

Merry Christmas! 🎁

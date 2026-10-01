# fluid-simulation

浏览器里的 **WebGL 流体模拟**：鼠标拖动即可扰动流体，右侧参数面板可实时调耗散、压力、涡度等系数。

## 运行

纯静态页面，**无需构建**：直接用浏览器打开 `index.html`（需要 WebGL，建议 Chrome / Firefox）。

## 文件

| 文件 | 作用 |
| --- | --- |
| `index.html` | 页面入口（画布 + `dat.gui` 参数面板） |
| `script.js` | 流体求解与渲染：WebGL 着色器、半拉格朗日平流、压力迭代、涡度约束 |
| `dat.gui.js` | 参数调节面板 |
| `logo.png` | favicon |
| `LDR_LLL1_0.png` | 环境贴图（LDR） |
| `iconfont.ttf` | 图标字体 |

## 操作

- **鼠标拖动**：注入速度与密度（“搅动”流体）
- **右上角面板**：实时调整密度/速度耗散、压力、涡度（`CURL`）、扩散半径等参数

## 说明

实现与经典的 **WebGL Fluid Simulation**（Pavel Dobryakov 一脉）同源，此处整理为可直接打开的单页工程；如用于二次分发，请注意保留上游的版权声明。

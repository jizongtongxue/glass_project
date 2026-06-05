# glass_project

一个基于 WebGL 的玻璃质感演示项目，包含主展示页和一个用于调整背景着色器参数的可视化编辑器。

## 项目内容

- `index.html`：全屏玻璃质感 Demo，使用双层 canvas 渲染动态背景与半透明玻璃层。
- `editor.html`：背景颜色编辑器，可实时调节渐变、光晕位置和扩散强度，并复制对应的着色器代码。
- `displacement.png`：高度图素材。
- `normal.png`：法线贴图素材。
- `roughness.png`：粗糙度贴图素材。

## 功能特性

- 纯前端实现，无需构建工具或依赖安装
- 基于 WebGL 的动态背景与玻璃层渲染
- 支持窗口自适应和高分屏渲染
- 提供多个背景预设，便于快速试色
- 可在编辑器中直接复制背景片元着色器代码

## 使用方式

### 直接打开

直接用浏览器打开以下文件即可：

- `index.html`
- `editor.html`

### 本地服务器方式

如果你希望用本地服务器访问，可在项目目录执行：

```bash
python3 -m http.server 8000
```

然后在浏览器访问：

- `http://localhost:8000/index.html`
- `http://localhost:8000/editor.html`

## 适用场景

- 玻璃拟态视觉实验
- 着色器背景效果调试
- 落地页或品牌展示页视觉原型
- WebGL 入门练习与材质表现参考

## 技术说明

- 使用原生 HTML、CSS、JavaScript
- 使用 WebGL Shader 实现背景光晕和玻璃层效果
- 主页面通过纹理数据生成法线、粗糙度与位移结果
- 编辑器使用参数化方式实时预览背景片元着色器效果

## 文件结构

```text
glass_project/
├── index.html
├── editor.html
├── displacement.png
├── normal.png
├── roughness.png
└── README.md
```

## 后续可扩展

- 增加鼠标交互或视差效果
- 将编辑器参数保存为 JSON 配置
- 拆分 shader 代码为独立文件
- 部署到 GitHub Pages 作为在线演示

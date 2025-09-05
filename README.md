# 正十二面体 3D 交互应用

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Glossary/HTML5)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)

> 🎲 一个基于原生 JavaScript 的 3D 正十二面体交互应用，支持完整的 3D 渲染、动画控制和骰子投掷功能。

## ✨ 功能特性

### 🎯 核心功能
- **3D 正十二面体渲染** - 完整的几何体生成和 3D 投影
- **实时交互控制** - 支持鼠标拖拽、触摸手势操作
- **骰子模式** - 完整的 12 面骰子投掷体验
- **动画系统** - 流畅的旋转动画和物理模拟

### 🎮 交互方式
- **鼠标控制**：拖拽旋转模型，双击重置位置
- **触摸手势**：
  - 单指拖拽：调整模型角度
  - 双指捏合：调整模型大小
  - 三指点击：重置模型位置
- **键盘快捷键**：
  - 空格键：暂停/播放旋转
  - R 键：重置模型位置

### ⚙️ 可调节参数
- 旋转速度控制
- 模型大小缩放
- 面颜色明艳度
- 面透明度调节
- 面数字大小
- 面板透明度和毛玻璃效果

## 🚀 快速开始

### 在线体验
直接打开 `index.html` 文件即可在浏览器中体验完整功能。

### 本地运行
```bash
# 克隆项目
git clone <repository-url>

# 进入项目目录
cd dodecahedron-3d

# 使用本地服务器启动（推荐）
# Python 3
python -m http.server 8000

# 或使用 Node.js
npx http-server

# 打开浏览器访问 http://localhost:8000
```

### 系统要求
- 现代浏览器（支持 HTML5 Canvas 和 ES6+）
- 无需额外依赖或构建工具

## 🛠️ 技术栈

### 核心技术
- **HTML5 Canvas** - 2D 图形渲染
- **原生 JavaScript** - 完整的 3D 数学计算和动画系统
- **CSS3** - 响应式布局和视觉效果

### 架构设计
```
├── 渲染系统 (RenderSystem)
│   ├── 3D 到 2D 投影
│   ├── 面排序和遮挡处理
│   └── 光照效果计算
├── 动画系统 (AnimationController)
│   ├── 普通旋转模式
│   └── 骰子物理模拟
├── 数学工具库 (Utils)
│   ├── 向量运算
│   ├── 矩阵变换
│   └── 几何计算
└── 事件管理系统 (EventManager)
    ├── 统一事件处理
    └── 移动端优化
```

## 📖 项目说明

### 🤖 AI 辅助开发
本项目是在 AI 助手的协助下完成的，体现了人机协作在软件开发中的创新应用。AI 在以下方面提供了重要支持：

- **架构设计**：模块化的代码组织结构
- **数学算法**：3D 几何计算和投影算法
- **性能优化**：事件管理和渲染优化
- **代码质量**：最佳实践和设计模式

### 🔧 技术亮点

#### 1. **纯 JavaScript 3D 引擎**
- 完整的 3D 数学库实现
- 高效的渲染管线
- 无需外部 3D 库依赖

#### 2. **移动端优化**
- 专门的触摸事件处理
- 防误操作设计
- 响应式布局适配

#### 3. **物理模拟**
- 真实的骰子投掷物理效果
- 球面均匀分布速度生成
- 平滑的减速动画

#### 4. **事件管理系统**
- 统一的事件处理模式
- 高效的事件监听器管理
- 内存泄漏防护

## 📁 项目结构
```
├── index.html              # 主应用文件
├── README.md              # 项目说明文档
└── LICENSE               # 开源许可证
```

## 🎨 使用指南

### 基本操作
1. **旋转模型**：鼠标拖拽或单指滑动
2. **缩放模型**：双指捏合手势
3. **重置位置**：双击或三指点击
4. **暂停动画**：空格键或单击画布

### 骰子模式
1. 点击「骰子模式」按钮进入骰子模式
2. 点击「掷骰子」开始投掷
3. 观察物理动画并查看结果
4. 点击「停止」可提前停止投掷

### 控制面板
1. 点击「显示控制面板」打开设置
2. 调节各项参数实时预览效果
3. 支持毛玻璃效果和透明度调节

## 🧪 浏览器兼容性

| 浏览器       | 最低版本 | 支持程度 |
|-------------|---------|---------|
| Chrome      | 60+     | ✅ 完全支持 |
| Firefox     | 55+     | ✅ 完全支持 |
| Safari      | 12+     | ✅ 完全支持 |
| Edge        | 79+     | ✅ 完全支持 |
| Mobile Safari | 12+  | ✅ 完全支持 |
| Chrome Mobile | 60+  | ✅ 完全支持 |

## 🤝 贡献指南

我们欢迎所有形式的贡献！

### 开发流程
1. Fork 本项目
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

### 代码规范
- 使用现代 JavaScript 语法 (ES6+)
- 遵循现有代码风格
- 添加必要的注释
- 确保移动端兼容性

## 📄 开源许可证

本项目采用 [MIT 许可证](LICENSE) - 查看文件了解更多信息。

## 🙏 致谢

- 感谢 AI 助手在项目开发过程中的技术支持和代码优化建议
- 感谢开源社区提供的灵感和技术参考
- 感谢所有为 Web 3D 图形学发展做出贡献的开发者

## 📞 联系方式

如有问题或建议，欢迎：
- 开启 Issue
- 发送 Pull Request
- 通过邮件联系

---

<div align="center">
  <p>用 ❤️ 制作，基于 AI 辅助开发</p>
  <p>探索 3D 图形学的无限可能</p>
</div>

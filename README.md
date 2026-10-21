# 拾沙物语 Sand Story 🏖️✨

> 一款治愈系马卡龙配色的沙画收集解谜游戏。让玩家在层层剥离的沙粒流动中，感受策略规划的乐趣与画面重现的满足感。

![Sand Story Banner](https://img.shields.io/badge/Style-Macaron_Healing-ffb3ba?style=for-the-badge)
![Vue 3](https://img.shields.io/badge/Vue.js-3.x-4fc08d?style=for-the-badge&logo=vuedotjs&logoColor=white)
![HTML5 Canvas](https://img.shields.io/badge/Canvas-HTML5-e34f26?style=for-the-badge&logo=html5&logoColor=white)
![Web Audio API](https://img.shields.io/badge/Audio-Web_Audio_API-005580?style=for-the-badge)

🎮 **[👉 立即在线体验 (Live Demo)](https://yyyxinhu-ctrl.github.io/sand-story/)**  
*(点击上方链接，无需下载，打开浏览器即可游玩)*

---

## 💡 项目立意 (Project Concept)

《拾沙物语》旨在打造一款**低压力、高正向反馈的轻度益智小游戏**。

与传统的消消乐或无脑点击游戏不同，本项目结合了**分区沙层遮挡**与**同色收集机制**：
* 🌸 **治愈系体验**：采用奶油白、薄荷绿、蜜桃粉、薰衣草紫等柔和马卡龙色彩，搭配轻柔舒缓的音效。
* 🧩 **策略性解谜**：玩家需要仔细观察各区域的沙层堆叠关系，合理安排收集顺序与桶子容量。
* ✨ **成就感揭晓**：随着沙粒被逐层收走，被遮挡的沙画图案逐渐显现，带来视觉与心灵的双重满足。

---

## 🎯 核心机制 (Core Game Rules)

| 规则模块 | 机制设计说明 |
| :--- | :--- |
| **分区遮挡** | 画布由多个沙区组成，每个区域堆叠了不同颜色的沙层，**只能收集当前暴露在最表层的沙粒**。 |
| **同色收集** | 点击底部颜色桶，系统自动扫描并收集所有符合条件的表层沙粒。 |
| **容量限制** | 每个颜色桶有固定的储存上限（如 12 粒），满了需先完成收集目标，考验空间规划能力。 |
| **友好的容错** | 提供 **撤销 (Undo)**、**提示 (Hint)** 与 **重置** 功能，避免玩家因误操作直接卡死。 |
| **必定可解** | 所有关卡的沙层分布与配色均经过路径校验，保证至少存在一条通解逻辑。 |

---

## 🎨 视觉与交互亮点 (Key Features)

* **流沙粒子特效**：基于 HTML5 Canvas 绘制，沙粒在被收集时会产生流向对应颜色桶的抛物线粒子轨迹。
* **程序化程序音效**：使用原生 Web Audio API 合成，无需加载外部大音频文件，实现轻盈自然的流沙与清脆清桶音效。
* **响应式 UI 布局**：适配桌面端与移动端浏览器，带来顺畅的触摸/点击体验。
* **本地进度保存**：基于 LocalStorage 实现星级评价与关卡解锁状态的无缝保存。

---

## 🛠️ 技术栈与实现 (Tech Stack)

* **前端框架**：Vue 3 (SFC / Composition API)
* **渲染引擎**：HTML5 Canvas (粒子物理与动态流沙效果)
* **样式处理**：CSS3 (Flexbox/Grid 布局、CSS 变量、过渡动画)
* **音频合成**：Web Audio API (定制振荡器与频率渐变)
* **部署托管**：GitHub Pages / Vercel

---

## 📂 关卡设计规划 (Level Design)

* **关卡 1（初入沙洲）**：3 种基础配色，简单遮挡，帮助玩家快速建立“表层先收”的心理模型。
* **关卡 2（薄荷清晨）**：引入容量限制，引导玩家关注颜色桶的空间管理。
* **关卡 3（蜜桃晚霞）**：多区域交错遮挡，要求规划 2-3 步以后的显色顺序。
* **关卡 4（薰衣草夜）**：复合层级结构，提升深度策略解谜体验。
* **关卡 5（日光花园）**：多色彩与多通道组合，考验全局统筹能力。

---

## 🚀 本地运行 (Getting Started)

因为本项目采用了轻量化设计，无需复杂的编译环境：

1. 克隆本仓库到本地：
   ```bash
   git clone [https://github.com/yyyxinhu-ctrl/sand-story.git](https://github.com/yyyxinhu-ctrl/sand-story.git)

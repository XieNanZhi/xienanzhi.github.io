# xienanzhi.github.io

**谢永胜的个人作品集** —— 前端开发 / 软件测试方向求职作品展示。

在线访问：https://xienanzhi.github.io

## 站点结构

| 文件 | 说明 |
| --- | --- |
| `index.html` | 作品集主页：自我介绍、技能栈、项目亮点、质量实践、联系方式 |
| `game.html` | 代表作品：Flappy Bird 网页游戏，可在线试玩 |

## 代表作品：Flappy Bird 网页游戏

- 点击画面 / 空格 / 向上键：小鸟向上飞；松手自然下落
- 穿过上下管道的空隙得 1 分，撞到管道或落地即结束，按 R 重开
- 内置难度递增、5 套场景主题、间距/空隙可调、本地最高分记录

## 技术实现

原生 HTML / CSS / JavaScript，无框架、无依赖、无构建步骤：

- `requestAnimationFrame` + delta time 游戏循环
- 重力 / 冲量 / 角度插值的简化物理系统
- AABB 碰撞检测（含容差收缩）
- Canvas 2D 分层渲染 + `devicePixelRatio` 高清适配
- WebAudio API 合成音效（零音频文件）
- ready / play / over 状态机，`visibilitychange` 后台暂停
- `localStorage` 持久化（读取带 try/catch 容错）
- 主页滚动动效：`IntersectionObserver` + 被动事件监听

## 更新方式

修改代码后提交推送，等 1~5 分钟 GitHub Pages 自动更新。

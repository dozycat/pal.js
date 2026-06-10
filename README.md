# 仙剑奇侠传 JS 专案

像素风同人重制，致敬经典。在线游玩：

**[http://dozycat.github.io/pal.js/](http://dozycat.github.io/pal.js/)**

![](https://img.shields.io/badge/%E5%89%A7%E6%83%85-%E7%AC%AC%E4%B8%80%E7%AB%A0%E5%AE%8C%E6%95%B4%E5%8F%AF%E7%8E%A9-success)

## 像素版 · 第一章

`pixel/` 目录是一个独立的像素风实现，**零依赖原版资源文件**：

- 所有像素美术由代码绘制（9 个人物精灵 + 约 20 种地形图块）
- 剧情对白为原创撰写，完整覆盖第一章主线：
  客栈帮工 → 酒剑仙传剑 → 婶婶病倒 → 湖畔行舟 → 仙灵岛斗蛇妖 →
  初遇灵儿 → 姥姥逼婚 → 拜堂得药 → 离岛忘情 → 返乡救人 → 第一章 完
- 回合制战斗（攻击 / 仙风剑诀 / 金创药），战败不设死局
- WebAudio 芯片音源：六首原创五声音阶循环曲 + 全套音效，随场景自动切换
- 像素化启动加载动画（原 `loadingScreen.js` 圆环进度的重制）
- 引擎为 320×240 低分辨率缓冲放大渲染，无任何第三方依赖

### 操作

| 按键 | 功能 |
| --- | --- |
| 方向键 / WASD | 移动 |
| 回车 / Z / 空格 | 确认、对话、互动 |
| X / Esc | 取消 |
| M | 静音 / 恢复 |

左下角的绿色提示会引导剧情流程。

### 本地运行

无需构建，直接用浏览器打开 `pixel/index.html` 即可。

## 目录结构

```
pixel/            像素版（第一章）
  js/engine.js    渲染缓冲与键盘输入
  js/assets.js    代码绘制的全部像素美术
  js/maps.js      四张单屏地图数据
  js/dialog.js    对话框（打字机、分页、选项）
  js/battle.js    回合制战斗
  js/music.js     芯片音乐引擎与原创曲目
  js/story.js     第一章剧情脚本
  js/main.js      主循环与场景状态机
classic.html      早期的原版引擎实验入口（读取 resources/ 数据）
javascripts/      早期实验的引擎代码
resources/        原版游戏数据（版权归大宇/软星，像素版不使用）
```

## 致谢

- 引擎实验阶段参考了 [sivory/pal.js](http://sivory.github.io/pal.js/)
- 《仙剑奇侠传》为大宇资讯/软星科技作品，本仓库为粉丝同人习作，不作商业用途

# 李伟翔的游戏策划作品集

我做游戏玩法与系统设计，用 Godot 和 Unity 把规则做成可玩的原型。独立项目中，我用 AI 辅助实现和排查问题，自己负责玩法取舍、试玩和验收。

[在线作品集](https://lovevx.github.io/my-work/) · [中文文件导航](文件导航.md)

## 代表作品

| 项目 | 我负责的内容 | 作品入口 |
| --- | --- | --- |
| **Boomame · 放置破坏游戏** | 独立设计与开发。用砸楼、赚金币和解锁炮台串起从手动破坏到自动化的成长过程。 | [Windows 试玩](https://github.com/lovevx/boom/releases/tag/snapshot-2026-10-09) · [实机演示](https://lovevx.github.io/my-work/works/boomame.html) · [源码](https://github.com/lovevx/boom) · [AI 协作复盘](https://github.com/lovevx/boom/blob/main/docs/AI_Workflow.md) |
| **HD-2D · 动作 RPG 原型** | 个人全程负责，AI 辅助。设计序章引导、森林探索与成长循环，记录技能提示、通路和装备反馈的迭代。 | [项目展示](https://lovevx.github.io/my-work/works/hd2d.html) · [源码与运行说明](https://github.com/lovevx/HD2Dgame) · [展示与验证材料](files/hd2d/README.md) |
| **Pool · 追逐解谜原型** | 团队项目，副策划兼副程序。参与背包规则、手电视野和街道追逐谜题的设计及验证。 | [项目展示](https://lovevx.github.io/my-work/works/pool.html) · [Windows 街道白盒试玩](https://github.com/lovevx/my-work/releases/tag/pool-street-v3-2026-10-09) |
| **《杖剑传说》体验分析** | 从轻付费玩家视角持续体验 36 天，结合玩家反馈，提出副本保底和低战力资源获取建议。 | [体验分析报告](https://lovevx.github.io/my-work/works/zhangjian-chuanshuo.html) |

## AI 协作案例

Boomame 进场时一次创建大量建筑方块，导致切场卡顿。AI 给出分帧方案和代码骨架，我调整为从底层向上生成，让建筑支撑尽早建立，再进游戏检查加载和破坏逻辑。[查看完整复盘](https://github.com/lovevx/boom/blob/main/docs/AI_Workflow.md)

## 补充项目

**潮汐声律终端 · Windows 音乐播放器**。我负责需求和交互取舍，用 AI 辅助实现与测试。歌单支持先浏览、选曲后再切换队列，找歌时可以继续播放当前曲目。公开版附有合成音乐和时间轴歌词，可免登录体验。[源码与项目说明](https://github.com/lovevx/resonance-terminal)

## 更多设计与分析

| 作品 | 简介 | 在线阅读 |
| --- | --- | --- |
| 探洞先锋 · GDD | 从 0 到 1 从核心循环到结算全链路的主策划设计文档 | [在线阅读](https://lovevx.github.io/my-work/works/tan-dong-xian-feng.html) |
| 空之轨迹1st · 战斗与养成拆解 | 经典 JRPG 系统拆解 + 面向移动端可迁移思路 | [在线阅读](https://lovevx.github.io/my-work/works/kongzhigui-1st.html) |
| 鸣潮商城系统 | 商业化系统 + 可读配表（xlsx 落地成品） | [在线阅读](https://lovevx.github.io/my-work/works/mingchao-mall.html) |
| 王者数值建模 · 作品摘要 | MOBA 装备铭文伤害仿真，方法论 + 量化结论 | [在线阅读](https://lovevx.github.io/my-work/works/wangzhe-numerics.html) |
| 超自然行动组 · 新手引导改造 | 体验→问题定位→三阶段递进改造的引导设计 | [在线阅读](https://lovevx.github.io/my-work/works/chaoziran-tutorial.html) |

## 原始文档下载

Boomame 当前源码与参数见 [游戏仓库](https://github.com/lovevx/boom)、[数值平衡](https://github.com/lovevx/boom/blob/main/docs/Numeric_Balance.md)和[本次更新记录](https://github.com/lovevx/boom/blob/main/docs/Release_2026-10-09.md)。以下 Word 文件保留早期设计材料。

| 作品 | 文件 |
| --- | --- |
| HD-2D · 执行与系统策划 | [六页展示 PDF](files/hd2d/01_项目展示稿.pdf) · [Word](files/hd2d/01_项目展示稿.docx) · [完整展示包](files/hd2d/HD2D_策划展示包_20261013.zip) |
| Pool · 系统与关卡 | [背包功能说明](https://github.com/lovevx/my-work/blob/main/files/pool/inventory-rules.md) · [街道谜题卡](https://github.com/lovevx/my-work/blob/main/files/pool/street-design.md) · [验证记录](https://github.com/lovevx/my-work/blob/main/files/pool/street-verification.md) |
| 探洞先锋 · GDD | [探洞先锋游戏设计文档.docx](files/探洞先锋游戏设计文档.docx) |
| Boomame · 设计文档 | [Boomame_游戏设计文档_GDD.docx](files/Boomame_游戏设计文档_GDD.docx) |
| Boomame · AI 协作文档 | [Boomame_AI协作文档.docx](files/Boomame_AI协作文档.docx) |
| 空之轨迹1st · 拆解 | [《空之轨迹1st》战斗与养成系统拆解.docx](files/《空之轨迹1st》战斗与养成系统拆解.docx) |
| 鸣潮商城系统 | [鸣潮商城系统.xlsx](files/鸣潮商城系统.xlsx) |
| 王者数值建模 · 摘要 | [王者数值建模_作品摘要.docx](files/王者数值建模_作品摘要.docx) |
| 杖剑传说 · 报告 | [手游杖剑传说体验分析报告.docx](files/手游杖剑传说体验分析报告.docx) |
| 超自然行动组 · 引导 | [超自然行动组新手引导流程.docx](files/超自然行动组新手引导流程.docx) |

## 游戏试玩包（Windows）

| 游戏 | 下载 | 大小 |
| --- | --- | --- |
| Boomame · 2026-10-09 | [Boomame_Windows.zip（解压后运行，无需 Godot）](https://github.com/lovevx/boom/releases/download/snapshot-2026-10-09/Boomame_Windows.zip) | 以 Release 标注为准 |
| Pool · 街道v3白盒 | [Pool_AngerStreetV3_Windows.zip（解压后运行）](https://github.com/lovevx/my-work/releases/download/pool-street-v3-2026-10-09/Pool_AngerStreetV3_Windows.zip) | 以 Release 标注为准 |
| 勇者传说 Windows 版 | [YongZhe_Windows.zip（解压即玩）](https://github.com/lovevx/my-work/releases/download/demo-builds/YongZhe_Windows.zip) | 约 42MB |

## 演示视频

| 项目 | 视频 |
| --- | --- |
| Boomame 当前美术与自动轰炸演示 | [点击观看 / 下载](videos/boomame.mp4) |
| 勇者传说（勇者之路） | [点击观看 / 下载](videos/勇者之路.mp4) |

## 通用简历

[李伟翔_游戏策划简历.docx](files/李伟翔_游戏策划简历.docx)

## HD-2D 展示材料说明

包含项目介绍、系统规则、三个设计迭代案例、八张实机截图与六页作品展示稿。实机视频尚未录制，未将旧验证包作为当前试玩包上架。当前工程证据与本轮复核见[成果证据](files/hd2d/04_成果证据.md)。

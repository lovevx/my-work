# 李伟翔的游戏策划作品集

我做玩法与系统设计，用 Godot 和 Unity 制作可玩的原型。独立项目中，我用 AI 辅助实现和排查问题，自己负责玩法取舍、试玩和验收。

[在线作品集](https://lovevx.github.io/my-work/) · [游戏策划简历 Word](files/李伟翔_游戏策划简历.docx) · [完整文件索引](文件导航.md)

## 游戏原型

### Boomame 放置破坏游戏

**个人设计与开发 · Godot**。玩家从手动砸楼赚金币开始，升级后解锁自动炮台，再用跨局转生延续成长。

进场一次生成大量建筑方块会造成卡顿。我用 AI 起草分帧加载方案，并调整为从底层向上生成，让支撑先建立，再在游戏里检查加载和破坏逻辑。

[Windows 试玩](https://github.com/lovevx/boom/releases/download/snapshot-2026-10-09/Boomame_Windows.zip) · [项目页与实机演示](https://lovevx.github.io/my-work/works/boomame.html) · [源码](https://github.com/lovevx/boom) · [AI 协作复盘](https://github.com/lovevx/boom/blob/main/docs/AI_Workflow.md)

<details>
<summary>设计与迭代资料</summary>

[数值平衡](https://github.com/lovevx/boom/blob/main/docs/Numeric_Balance.md) · [版本记录](https://github.com/lovevx/boom/blob/main/docs/Release_2026-10-09.md) · [早期设计文档](files/Boomame_游戏设计文档_GDD.docx) · [AI 协作 Word 版](files/Boomame_AI协作文档.docx)

</details>

### HD-2D 动作 RPG 原型

**个人项目 · Godot · AI 辅助**。设计序章引导、森林探索与成长循环，迭代技能提示、场景通路和装备对比。可用 Godot 从源码运行。

[项目展示](https://lovevx.github.io/my-work/works/hd2d.html) · [源码与运行说明](https://github.com/lovevx/HD2Dgame) · [展示稿 PDF](files/hd2d/01_项目展示稿.pdf)

<details>
<summary>展示与验证材料</summary>

[展示稿 Word](files/hd2d/01_项目展示稿.docx) · [完整展示包](files/hd2d/HD2D_策划展示包_20261013.zip) · [验证记录](files/hd2d/04_成果证据.md)

</details>

### Pool 追逐解谜原型

**团队项目 · 副策划兼副程序 · Unity**。参与背包规则、手电视野和遮挡验证，围绕怪物追击设计街道谜题、操作窗口与返程路线。

[项目展示](https://lovevx.github.io/my-work/works/pool.html) · [Windows 街道白盒试玩](https://github.com/lovevx/my-work/releases/download/pool-street-v3-2026-10-09/Pool_AngerStreetV3_Windows.zip)

<details>
<summary>系统与关卡资料</summary>

[背包功能说明](files/pool/inventory-rules.md) · [街道谜题卡](files/pool/street-design.md) · [验证记录](files/pool/street-verification.md)

</details>

## 游戏设计与体验分析

| 作品 | 内容 | 材料 |
| --- | --- | --- |
| 《杖剑传说》体验分析 | 以轻付费视角体验 36 天，结合玩家反馈提出副本保底与低战力资源获取建议 | [在线报告](https://lovevx.github.io/my-work/works/zhangjian-chuanshuo.html) · [Word](files/手游杖剑传说体验分析报告.docx) |
| 《探洞先锋》设计文档 | 担任主策划，设计核心循环、资源规则与结算流程 | [在线文档](https://lovevx.github.io/my-work/works/tan-dong-xian-feng.html) · [Word](files/探洞先锋游戏设计文档.docx) |
| 《超自然行动组》新手引导 | 梳理教学断点，设计三阶段引导流程 | [在线方案](https://lovevx.github.io/my-work/works/chaoziran-tutorial.html) · [Word](files/超自然行动组新手引导流程.docx) |
| 《空之轨迹 1st》系统拆解 | 分析战斗与养成系统，整理可迁移到移动端的设计思路 | [在线拆解](https://lovevx.github.io/my-work/works/kongzhigui-1st.html) · [Word](files/《空之轨迹1st》战斗与养成系统拆解.docx) |
| 《鸣潮》商城系统 | 拆解商品分类、货币结算、购买限制和折扣规则 | [在线方案](https://lovevx.github.io/my-work/works/mingchao-mall.html) · [Excel 配表](files/鸣潮商城系统.xlsx) |
| 《王者荣耀》数值建模 | 用 MATLAB 模拟装备与铭文收益，对比不同出装和目标防御条件 | [在线摘要](https://lovevx.github.io/my-work/works/wangzhe-numerics.html) · [Word](files/王者数值建模_作品摘要.docx) |

## 其他可体验作品

- **勇者传说**。Godot 横版动作冒险，包含连击、滑铲、场景探索与首领战。[Windows 试玩](https://github.com/lovevx/my-work/releases/download/demo-builds/YongZhe_Windows.zip) · [实机视频](videos/勇者之路.mp4) · [源码](https://github.com/lovevx/Brave-person)
- **潮汐声律终端**。Windows 音乐播放器。我负责需求和交互取舍，用 AI 辅助实现和测试。先浏览歌单、选曲后再切换队列，找歌时可以继续播放当前曲目。[Windows 鸣潮主题版下载](https://github.com/lovevx/resonance-terminal/releases/tag/v1.11.0-original) · [源码与实机截图](https://github.com/lovevx/resonance-terminal)

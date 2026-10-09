# 街道 v3 验证记录

日期：2026-10-09。Unity 6000.3.24f1，Windows x64，Direct3D 11。

| 检查 | 结果 | 证据 |
|---|---|---|
| 场景生成 | `STREET_V3_SCENE_PASS` | `Pool/Captures/AngerStreetV3/scene-build.txt` |
| Windows 构建 | `STREET_V3_BUILD_PASS` | `Pool/Captures/AngerStreetV3/player-build.txt` |
| 功能、实际输入、物理与重开 | **72 项通过**，`STREET_V3_PLAY_PASS` | `Pool/Captures/AngerStreetV3/checks.txt` |
| 怪物全程启用的完整路线 | **55 项通过**，`STREET_V3_PLAY_PASS`；零被捕 | `Pool/Captures/AngerStreetV3/live-checks.txt` |
| 摄像机画面 | 已逐张检查线路板、冲锋准备视角、远端保持柄、配电、交付与全图 | 同目录 `.png` |
| 三名未读文档玩家 | **待验证** | `playtest-sheet.md` |

## 功能与物理证据

- 两只 L 接头按实际输入旋转；错误方向停止传电，只接好上游时不打开维修铺；完整接通后全部维修铺入口打开。可重复机关不加入一次性背包收集。
- 窄口内按 E 不能操作街道检修柄；离开窄口实际接近才完成检修供电。
- 踩压板真实开门。满体力怒区奔跑无法在 0.9 秒延时内通过；失败后能回压板重试。错误支路冲锋在真实墙体处撞停眩晕，能步行返回。
- 压板附近的观察镜头同时容纳错误转角、远端保持柄和停点墙；正确怒冲锋通过卷帘、抵达终端墙并眩晕，恢复后 E 拉保持柄，永久开门。
- 后屋／归途切换改变两道实体门，前厅能反复切换。取物后重新供电归途，并走完整条通道回中心 E 放置；拾取不是交付，最终为 1/5，完整大门不打开。
- 怪物根据玩家位置起冲、途中不受新位置转向影响；实际撞墙后重新瞄准，不采用固定轴折返。开放后的归途能被怪物使用，实体窄口不能被其身体穿过。
- 中心真实接触会捕获。临时压板计时在被捕后复位；已完成线路、检修、永久开门、供电档位、钥匙和交付保留。按真实 R 输入重新加载场景后全部清空并恢复初始门状态。

功能检查在机关通行部分暂时停用怪物以隔离碰撞与规则；怪物行为、窄口、归途通行及捕获部分另行启用。不可把功能路线当作持续追击证据。

## 持续追击证据

从场景原生出生点开始，使用输入系统事件移动、拾怒球、转接头、等待怪物实际冲离、拉检修柄、冲过卷帘、保持开门、切换供电、取钥匙、走归途、中心交付。全程一个怪物启用；没有瞬移、停用怪物、修改追击、延长保护或利用捕获搬回。

事件记录包含：检修柄拉开时怪物在 `(19.56, 24.84)`，冲刺方向约 `(0.00, -1.00)`；卷帘保持柄手动拉开；先切归途再切回后屋；取钥匙后切归途；最终中心交付。最终版本的准确时间与坐标见 `live-events.txt`。

这是已知解法的可完成性检查，不能说明首次玩家需要 10–15 分钟，也不能替代线索理解、恐怖氛围和操作容错的玩家验收。

## 复现

```powershell
& 'D:\聚光灯gj\deliverables\AngerStreetV3\AngerStreet.exe' -street-v3-check -street-output C:/Temp/PoolStreetV3QA -screen-width 1280 -screen-height 960 -screen-fullscreen 0 -force-d3d11
& 'D:\聚光灯gj\deliverables\AngerStreetV3\AngerStreet.exe' -street-v3-live-check -street-output C:/Temp/PoolStreetV3LiveQA -screen-width 1280 -screen-height 960 -screen-fullscreen 0 -force-d3d11
```

源码入口为 `StreetV3Checks`，启动参数只用于独立验证。正常试玩不自动求解，也不加载检查组件。

试玩包的 `设计与验证` 目录同时保存同名报告、事件记录和画面副本，队友不必打开 Unity 工程即可查看。

## 改动边界

新增 v3 场景、生成器、机关与检查组件；既有 v2、五区框架、背包、怒融合和共享追击实现均保留。Unity 构建生成的渲染管线与项目设置变更已经审计并恢复到本次工作开始前状态。已有工作区改动没有回滚。

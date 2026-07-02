# 轻度 Roguelike v1.0 - 第 1 周开发计划

## Day1
任务：
- 创建 Unity 项目目录结构
- 创建 Boot 与 Game 场景
- 创建核心脚本文件

验收标准：
- 所有目录存在
- 所有脚本文件存在
- Boot.unity 与 Game.unity 存在

## Day2
任务：
- 搭建 DiceSystem 与 MapSystem 骨架
- 明确掷骰子与线性移动流程

验收标准：
- 可以描述掷骰子到移动的流程
- 地图规则限定为线性节点

## Day3
任务：
- 搭建 CombatSystem 骨架
- 明确自动回合制战斗结束条件

验收标准：
- 战斗开始、进行、结束流程明确
- 死亡判定存在

## Day4
任务：
- 搭建 RewardSystem 与 ProgressionSystem 骨架
- 明确三选一 buff 奖励流程

验收标准：
- 奖励为三选一 buff
- 成长流程可以衔接下一轮推进

## Day5
任务：
- 搭建 UIManager、HUDController、RewardPanel 骨架
- 明确掷骰子、战斗、奖励 UI 流程

验收标准：
- 三类 UI 流程已定义
- UI 文件已存在

## Day6
任务：
- 搭建 AdsManager、IAPManager、SaveSystem 骨架
- 保留商业系统 mock 接口

验收标准：
- ShowRewardAd() 存在
- ShowInterstitialAd() 存在
- RemoveAds、StarterPack、BoostPack 已预留

## Day7
任务：
- 检查所有目录、文档、脚本与场景是否齐全
- 对照 MVP 标准进行核对

验收标准：
- 文件无遗漏
- 文档无遗漏
- 结构路径符合要求

## MVP 完成标准
- 可以掷骰子
- 可以移动
- 可以触发战斗
- 战斗可结束
- 可以死亡重开
- 可连续运行 10 轮不崩溃

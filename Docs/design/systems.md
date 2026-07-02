# 系统设计说明

系统列表：
- DiceSystem
- MapSystem
- CombatSystem
- RewardSystem
- ProgressionSystem
- AdsManager（mock）
- IAPManager（mock）

职责划分：
- DiceSystem：负责 1~6 随机掷骰结果。
- MapSystem：负责线性节点地图与角色移动。
- CombatSystem：负责自动回合制战斗流程与战斗结束判定。
- RewardSystem：负责战斗后或事件后的三选一 buff 奖励。
- ProgressionSystem：负责本局成长结果的应用与重开循环衔接。
- AdsManager（mock）：预留激励广告与插屏广告接口。
- IAPManager（mock）：预留 RemoveAds、StarterPack、BoostPack 商品接口。

系统关系：
1. DiceSystem 产出点数。
2. MapSystem 根据点数推进角色位置并触发节点事件。
3. CombatSystem 处理战斗节点内容。
4. RewardSystem 在战斗胜利或奖励节点后提供三选一 buff。
5. ProgressionSystem 记录成长结果，并在死亡后进入重开循环。
6. AdsManager 在死亡复活、奖励翻倍、宝箱节点时提供 mock 接口。
7. IAPManager 仅保留商品定义，不接入 SDK。

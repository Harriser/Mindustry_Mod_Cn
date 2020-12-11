# 通用字段
- 删减部分6.0不适用，或作用不大的条目（声音、效果等）
- 来源页已不可访问

## Block（固体）
- 建筑
| 字段                | 字段类型    | 描述         |
| ------------------- | ----------- | ------------ |
| update              | boolean     | 更新         |
| destructible        | boolean     | 易损坏的     |
| unloadable          | boolean     | 卸载能力     |
| solid               | boolean     | 固体         |
| rotate              | boolean     | 旋转         |
| breakable           | boolean     | 易碎的       |
| rebuildable         | boolean     | 可重建的     |
| insulated           | boolean     | 绝缘         |
| health              | int         | 健康         |
| baseExplosiveness   | float       | 基础爆炸性   |
| floating            | boolean     | 漂浮的       |
| size                | int         | 尺寸         |
| expanded            | boolean     | 扩展的       |
| timers              | int         | 计时器       |
| configurable        | boolean     | 可配置的     |
| canOverdrive        | boolean     | 可以超速     |
| requirements        | [ItemStack] | 需求         |
| category            | Category    | 类别         |
| buildCost           | float       | 建造成本     |
| buildVisibility     |             | 建筑可见性   |
| buildCostMultiplier | float       | 建造成本乘数 |

## BlockStorag（扩展内容）
- 可存储物品或液体缓冲液的块的类型。

| 字段           | 字段类型  | 描述       |
| -------------- | --------- | ---------- |
| hasItems       | boolean   | 项目需求   |
| hasLiquids     | boolean   | 液体需求   |
| hasPower       | boolean   | 电力需求   |
| outputsLiquid  | boolean   | 输出液体   |
| consumesPower  | boolean   | 消耗电力   |
| outputsPower   | boolean   | 输出电力   |
| itemCapacity   | int       | 物品容量   |
| liquidCapacity | float     | 液体容量   |
| item           | float     | 项目       |
| liquidPressure | float     | 液体的压力 |
| consumes       | Consumers | 消耗       |

### Block部分字段说明

- unloadable
	- 卸载器或工厂
- rotate
	- 钻机或武器
- breakable
	- 是否可以通过右键删除
- health
	- 建筑血槽
- floating
	- 空中构建或漂浮
- size
	- 建筑大小
- priority
	- 被敌人看到时，此方块的目标优先级。
- timers
	- 部分建筑的可选项，例如修复器，力墙
- configurable
	- 是否可以点击并选择该块进行配置。（例如：节点连接）
- consumesTap
	- 点击此块时是否消耗点击事件。（大门，开启/关闭）
- configurable
	- 是否可以点击并选择该块进行配置。（例如：节点连接）
- canOverdrive
	- 是否受超速器影响
- requirements
	- 建设需求/材料
- buildCost
	- 建造该区块的成本；不要直接修改！
- buildCostMultiplier
	- 建造成本翻倍乘数
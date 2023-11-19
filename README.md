# Origins Themed Pack

---

在开始之前，您可能需要了解以下内容。

1. Origins Mod
   
    以数据驱动格式为Minecraft添加种族的模组，本数据包依赖于此。
    https://github.com/apace100/origins-fabric

2. Open Loader
   
   最快更新，应用最广泛的开放式数据包/材质加载器。
   本项目需以数据包形式进行加载，使用类似功能的模组以获得更佳体验。
   https://beta.curseforge.com/minecraft/mc-mods/open-loader


**这个数据包使用了 Origins 1.9.0 及以上的语法。** _请使用 1.19.4 以上的版本进行游玩。_

---

## 设计思路

> 本数据包是 _Salty Origins_ ~~在某种程度上的~~ 续作，你可以在我的 Git 仓库页面找到它（和它的美术资源）。  

大体量的数据包无论是跟进更新，Bugfix，还是维护优化... 都非常痛苦折磨，而且缓慢。因此，这个数据包做了极大幅度的精简，以确保可维护性。

> _和 Salty Origins 相同，这个数据包主要面向 **多人游戏** 。_ 但同时，我会在 _最大限度上_ 保证单人游戏时的游玩体验。

_为了适配多人对抗的游戏风格的同时保留鼓励各种族协作的玩法，尽最大可能贴合每个玩家的游玩风格_，我将 Origins Mod 添加的 _种族_ 从 **9** 个缩减至 **4** 个，分别对应四种游玩风格的大体方向，即：

_建造，战斗，探索，生存_。

那么，在对种族进行介绍之前，请允许我再次介绍以下 Emoji 符号代表的含义：

* 🔺代表这个能力将给玩家带来正面增益。符号的数量越多，这个能力为玩家带来的增幅就越强。

* 🔻代表这个能力将为玩家带来负面效果。符号的数量越多，这个能力为玩家带来的负面效果就越强。_这些负面效果可能只会在特定情况下触发，作为玩家游玩过程中行为的软限制存在。_

* 🔶 代表这个能力将同时带来正面效果与负面效果。_力量代价。_
  
* 💦 代表这个能力是纯装饰性的。

---

### 🌊 Merling - 海洋族裔

> _Origins Mod 其原版模组内容中种族设计的巅峰。_
>
> 与原版模组内容相差较小，其改动集中在优化单人游玩体验上。

#### Gills - 水生

🔶🔻🔻

> _与原版 Origins 保持一致。_

赋予玩家在水中呼吸的能力，以取代玩家在陆地上呼吸的能力。潮湿度将取代氧气条展示玩家剩余的可呼吸时间。

暴露在雨水中会阻止潮湿度的流失。

#### Ocean Spawn - 来自海洋

🔺

~~玩家将在距离初始重生点最近的 _沙滩_ 出生。~~

因为部分版本依然存在的巨大性能消耗（很可能因为 `locate` 指令的同步执行），暂时不对出生点进行修改。

这个问题在 _1.20.2_ 版本得到改善。

玩家出生时将获得 **180s** 的 _水下呼吸_ 效果。在复活时，获得 **45s**。

#### Wet Eyes - 海洋之眼

🔺🔺

> _与原版 Origins 保持一致。_

当玩家浸没在水体中时，将获得 _夜视_ 效果。

_*这个能力通过首要能力按键_ （默认为 `G`） _切换开关。_

#### Like Water - 洋流适应

🔺

> *与原版 Origins 保持一致。*

赋予玩家在水体中漂浮的能力。阻止玩家在水中自然下沉，除非玩家潜行。

#### Aqua Affinity - 水下速掘

🔺🔺

> *与原版 Origins 保持一致。*

浸没在水中将不会减缓玩家的挖掘速度。

#### Fins - 鳍

🔺🔺

> *与原版 Origins 保持一致。*

大幅提高玩家游泳时的速度，_提升至原游泳速度的 **1.5** 倍_。

#### Conduit Power on Land - 潮涌力量

🔺

> *与原版 Origins 保持一致。*
> 
> *这个能力是隐藏的，不会在界面中显示。*

#### Air From Potions - 补水

🔺

> *这个能力是隐藏的，不会在界面中显示。*

使用任意类型的药水将补充 **4s** 的呼吸时间。

> *原版Origins的行为将补充 3s 的呼吸时间，相较原版延长了 1s。🐸*

#### Aquatic - 海洋生物

🔻

> *与原版 Origins 保持一致。*
> 
> *这个能力是隐藏的，不会在界面中显示。*

被视为 _水生生物_ ，将从穿刺等附魔中受到更多伤害。

#### Catch The Rainbow - 彩虹捕手

🔺🔺

*当玩家脱离水体时，如果当前世界天气为 _晴朗_，则可以通过在 **主手** 持有 **海洋之心** 并按下 _首要能力按键_ （默认为 `G`）将世界天气更改为 _雷暴_。

_这个操作将会消耗掉 **1** 个海洋之心。_

#### Glow in Water - 熠熠生辉

💦

> *这个能力是隐藏的，不会在界面中显示。*

当玩家完全浸没在水中时，将会在周身环绕发光鱿鱼的粒子效果。

---

### 🔥 Blazeborn - 烈焰族裔

> Origins Mod 其原版模组内容中 ~~开局游玩体验最差的种族没有之一~~
>
> 其改动以“地狱生存”为主要方向进行调整，鼓励玩家在地狱长期居住，发展，同时优化玩家全时期在地狱的生存体验。

#### Nether Spawn - 地狱呼唤

🔶🔻

玩家的初始重生点将位于 _与主世界对应最接近初始重生点位置_ 的 _诡异森林_。


#### Water Vulnerability - 恐水症

🔻🔻🔻

> *与原版 Origins 保持一致。*

接触水体或暴露在雨中会使玩家以每秒 **2** 点（♥）的速度失去生命值。

饮用药水也将导致玩家失去 **2** 点（♥）生命值。

_防水_ 附魔将延后因接触水体及淋雨而受到伤害的时间，允许玩家短暂接触水体而不受到伤害。

_防水_ 附魔与其他 _保护_ 附魔冲突。

#### Nether Immunity - 地狱造物

🔺🔺

赋予玩家免疫 _火焰伤害_ 与 _凋零效果_ 的能力。

#### Inferno - 炽热

🔺🔺

当玩家处于 _着火_ 状态时，按下 _首要能力按键_ （默认为 `G`）发射三个 _小火球_ 。

这个能力有 **5** 秒 的冷却时间。

玩家发射出的箭矢（除药箭）将始终赋予 _着火_ 效果，其效果等同于 _火矢_ 附魔。

#### Anchor Charger - 萤石力量

🔺🔺

使用 _空手_ 右击未处于最大充能状态的 _重生锚_ 将为其补充 **1** 次充能。这将消耗掉玩家 **2** 点（♥）生命值。

这个能力有 **2** 秒 的冷却时间。

#### Lava Wander - 熔岩漫步

🔺🔺

使玩家能够骑乘未安装鞍的炽足兽。

#### Fear Cold - 畏惧寒冷

🔻🔻

被 _雪球_ 攻击将使玩家受到 **3** 点（1.5 ♥）。

从 _细雪_ 带来的 _寒冷_ 效果中受到 **5** 倍伤害（2.5♥ / 2s）。

> _与原版烈焰人行为逻辑一致。_

#### Ash Particles - 灰烬

💦

> *这个能力是隐藏的，不会在界面中显示。*

当玩家位于地狱时，将会在周身环绕火焰粒子的效果。

当玩家位于其他维度时，将会在周身环绕灰烬粒子的效果。

---

### 👁 Enderian - 末影族裔

> 原版 Origins Mod 里最强大的种族。设计上不好评价，但玩起来非常开心。
>
> 极大削弱了战斗能力和投掷珍珠传送的频率，但补足了 _一些_ 能力，以鼓励玩家探索。

#### Ender Pearl - 传送

🔺🔺🔺

每隔 **6** 秒，通过按下 _首要能力按键_ （默认为 `G`），玩家将投掷出一颗不造成伤害的末影珍珠。

#### Space Traveler - 空间旅行者

🔺🔺🔺

当玩家的生命值高于 **4** 点（♥♥），饱食度高于 **8** 点（🍗🍗🍗🍗）且处于 _空手_ 状态时，_潜行时打开背包_ （默认为 `Shift + E`） 将以 **4** 点 _饱食度_（🍗🍗）及饱和度为代价，为玩家打开末影箱存储界面。

使用这个能力将为玩家带来 **2** 秒的失明状态。_这个效果从设计上几乎是装饰性的。_

这个能力有 **4** 秒的冷却时间。

#### Water Vulnerability - 恐水症

🔻🔻🔻

> *与原版 Origins 保持一致。*

接触水体或暴露在雨中会使玩家以每秒 **2** 点（♥）的速度失去生命值。

饮用药水也将导致玩家失去 **2** 点（♥）生命值。

_防水_ 附魔将延后因接触水体及淋雨而受到伤害的时间，允许玩家短暂接触水体而不受到伤害。

_防水_ 附魔与其他 _保护_ 附魔冲突。

#### Extra Reach - 瘦长鬼影

🔺🔺

> *这个能力是隐藏的，不会在界面中显示。*

玩家将拥有额外 **1.25** 格的触及距离（不包含攻击距离）。

#### ??? ???

🔻

_使玩家无法理解任何形式的 ???。_

使玩家无法看到在头部位置穿戴 ??? 的任何实体。

玩家无法食用任何 ??? （被标记为 `origins:pumpkin_related`）制作成的食物。

玩家无法种植 ??? 。

玩家无法穿戴 ??? 。 _原版 Origins 没有阻止这个行为，~~这太缺德了~~_。

???（被标记为 `origins:pumpkin_related`）的物品 将会 ???。

玩家现在甚至连雪傀儡头上的 ??? 都看不到了。

> ~~其实我有想过阻止玩家破坏被这个Tag标记的方块。~~
>
> _我为什么没做？因为这真的太缺德了。_

#### Ender Particles - 神秘

💦

将会在玩家周身环绕地狱传送门的粒子效果。

---
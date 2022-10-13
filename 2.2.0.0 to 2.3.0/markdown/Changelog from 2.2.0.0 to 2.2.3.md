# 2.2.0.0 到 2.2.3 更新内容

## Mods文件变动
* 版本格式变动的Mod
  * OpenPrinter：改为-GTNH版本。
* 移除的Mod
  * Command Blocks for Better Questing
  * QuestBook
  * StandardQuestingPack

（注：移除的原因，见下面BetterQuesting的更新内容。）

## Mods更新

### AE2FluidCraft-Rework（AE2FC）
* 版本号：1.0.18-GTNH → 1.0.22-GTNH
* 合成计划预览界面的物品现在支持添加/删除NEI书签。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/20)）
* 精简了asm。（by GlodBlock [相关commit](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/commit/989cd173fbe4ef978862a1c10ff772cf43c33e50)）
* 原材料缓存仓现在有了实时显示流体储量的tooltip，鼠标移动到相应流体上可查看。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/20)）
* AE2FC的相关方块现在支持EIO流体导管。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/21)）
* AE2FC的ME流体输出总线现在支持合成卡。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/22)）
* 修复了当原材料不足时，合成计划显示的字节占用不正确的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/23)）
* 修复了ME流体解包器复制流体的bug（当ME流体存储总线所接仓室容量小于解包器内流体片的流体量时，不会消耗流体。）（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/23)）

### Applied-Energistics-2-Unofficial（AE2）
* 版本号：rv3-beta-107-GTNH → rv3-beta-111-GTNH
* 加入了P2P通道-ME接口，又称为“镜像接口”，可以将ME接口的内容“复制”到多个P2P输出端口。[^1]（by Kuba6000 [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/183) [discord前瞻视频](https://discord.com/channels/181078474394566657/295669878222880769/1026078863794634782)）
* 修复了流体处理样板终端设置的单格物品数量超过127时会变为负数的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/188)）
* ME存储总线设置界面的虚拟物品槽位中放置的物品，其格子右下角不再显示数量"1"。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/188)）
* "toggle focus"（切换焦点）的默认键位改为未绑定。（by miozune [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/189)）

[^1]: 目前只有物品版本的P2P通道-ME接口，流体版本会在以后更新中加入。

### Bartworks
* 版本号：0.5.86 → 0.5.90
* 修正了重复的本地化key。（by iouter [相关pr](https://github.com/GTNewHorizons/bartworks/pull/207)）
* 加入了两种新等级的强化硼玻璃方块。（by BlueWeabo [相关pr](https://github.com/GTNewHorizons/bartworks/pull/208)）
  * 无尽强化硼玻璃方块：UIV等级玻璃；
  * 超时空金属强化硼玻璃方块：UMV等级玻璃。

### BetterQuesting（更好的任务）
* 版本号：3.0.367-GTNH → 3.1.0-GTNH
* StandardExpansion, QuestBook, CB4BQ三个BetterQuesting附属Mod整合到了BetterQuesting中。（by eigenraven [相关pr-1](https://github.com/GTNewHorizons/BetterQuesting/pull/78) [相关pr-2](https://github.com/GTNewHorizons/BetterQuesting/pull/79)）
* Mod config增加了浏览模式中属性为UNLOCKED的未解锁任务线可见性切换的选项，默认开启。（也就是修复了2.2.0.0任务书浏览模式后续任务栏不可见的问题）（by Glease [相关pr](https://github.com/GTNewHorizons/BetterQuesting/pull/76)）
* 移植了部分1.12.2版本BetterQuesting的特性。（by Glease [相关pr](https://github.com/GTNewHorizons/BetterQuesting/pull/76)）具体为：
  * 可以通过聊天栏分享任务。
  * 玩家在使用了编辑模式-任务编辑界面中的“重置任务”按钮后，会被标记为"dirty"。
  * 任务书章节界面上方的“完成进度”现在会自适应调整字号。

### BloodMagic（血魔法）
* 版本号：1.3.14 → 1.3.16
* 修复了matchitem导致的NPE（空指针）错误。（by miozune [相关pr](https://github.com/GTNewHorizons/BloodMagic/pull/33)）
* 删除了语言文件中的重复key。（by ChromicRedBrick [相关pr](https://github.com/GTNewHorizons/BloodMagic/pull/34)）

### Botanic-horizons
* 版本号：1.0.11-GTNH → 1.0.12-GTNH
* 修复了花药台配方不支持藤蔓的bug。（by combusterf [相关pr](https://github.com/GTNewHorizons/Botanic-horizons/pull/17)）

### CookingForBlockheads（懒人厨房）
* 版本号：1.2.12-GTNH → 1.2.13-GTNH
* 添加了俄语语言文件。（by ldrinn-Elantey [相关pr](https://github.com/GTNewHorizons/CookingForBlockheads/pull/35)）

### Crops-plus-plus
* 版本号：1.3.6.3 → 1.3.6.4
* 删除了语言文件中的重复key。（by ChromicRedBrick [相关pr](https://github.com/GTNewHorizons/Crops-plus-plus/pull/43)）

### EnderCore
* 版本号：0.2.10 → 0.2.11
* 加入了getFluidFromItem的NEI支持，也就是说，EIO流体导管设置界面可以拖动NEI中的GT“流体片”配置。（by miozune [相关pr](https://github.com/GTNewHorizons/EnderCore/pull/10)）

### EnderIO（末影接口）
* 版本号：2.3.1.46 → 2.3.1.47
* 修复了使用龙研的权杖破坏EIO导管会导致游戏崩溃的bug。（by eigenraven [相关pr](https://github.com/GTNewHorizons/EnderIO/pull/86)）

### ForestryMC（林业）
* 版本号：4.4.15 → 4.4.16
* 修复了林业工作台中保存有无效配方时会导致进入存档崩溃的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/ForestryMC/pull/30)）

### GT5-Unofficial（格雷科技）
* 版本号：5.09.41.61 → 5.09.41.74
* 修复了黑青铜搅拌-电解配方未配平的问题。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1422)）
* 使用三录仪扫描集成矿石处理厂时会显示当前并行数。（by boubou19 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1426)）
* 修复了部分mod魔改配方失效的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1423)）
* 修复了使用三录仪扫描超净间开机时功率显示错误的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1425)）
* 处理阵列可以处理两种以上流体输入/输出的配方，所有含单元的配方都可以映射为对应的流体。（by BlueWeabo [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1346)）
* 重构fluid_api，使得GT_Fluid相关接口更流畅。（by leagris [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1407)）
* 修正了重复的本地化key。（by iouter [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1424)）
* 新增高级/无线红石覆盖板。（by dipo33 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1401)）
  * 新增2种高级红石覆盖板。
    * 高级红石信号发射器支持反相输出；
    * 高级红石信号接收器支持5种模式：与门、与非门、或门、或非门、模拟信号，前四种模式可以接受同一频道下多个覆盖板发出的红石信号；
  * 新增3种无线覆盖板：无线维护提示覆盖板、无线流体探测覆盖板、无线物品探测覆盖板。
* 地下流体生成计算公式修正：修复了设定的最小储量>0时流体实际生成量可能远超设定的最大储量的bug。（by chochem [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1418)）
* NEI页面拼写错误修复：1 ticks → 1 tick。（by Connor-Colenso [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1430)）
* GT的GUI/tooltip支持数字格式化，例如1000000会格式化为1,000,000。（by Connor-Colenso [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1431)）
* 将处理蜂窝配方中需求的邻苯二甲酸与氢氟酸对调，即以前要求氢氟酸处理的现在要求邻苯二甲酸，反之亦然。（by Runakai1 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1433)）
* 修复了红石信号、能量、物品不能越过流体过滤器覆盖板传输的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1437)）
* 修复了Botania梦之木和活木的板材切割机配方缺少电路板导致配方冲突的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1436)）
* 移植了GT6的万能工具。可以Shift+右键切换小刀、锯、锉、螺丝刀、剪线钳、剪枝器六种模式。（by iouter [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1435)）
* 加入了茶蜂，生产潘马斯茶叶。（by Runakai1 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1439)）
* 限制了处理阵列的最大并行，现在放入UEV+机器，最多只能降低1级电压处理配方，也就是最大并行=256。（by BlueWeabo [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1438)）
* 现在大型热交换机可以处理太阳能盐，1L热太阳能盐=1000L过热蒸汽，而最大过热蒸汽产量等同于热冷却液。（by Steelux8 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1444)）
* 处理阵列新增批处理模式，剪线钳Shift+右键切换。批处理模式可以为配方加上一个由输入原料量决定的并行系数，这个系数最大为128。最终的输入、输出为最大并行\*并行系数，同时配方处理时间也为原时间\*并行系数。批处理模式可以极大降低处理阵列造成的延迟，但不会增加其生产效率。（by S4mpsa [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1446)）
* nerf铟蜂：禁止通过诱变培育，杂交概率降至1%，初始速度改为“最慢”。（by Runakai1 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1442)）

### GTNHLib
* 版本号：0.0.5 → 0.0.6
* 使用事件提供的文字渲染分辨率。（by Alexdoru [相关pr](https://github.com/GTNewHorizons/GTNHLib/pull/10)）

### GTplusplus（GT++）
* 版本号：1.7.110 → 1.7.118-pre
* 修复了工业搅拌机使用存储输入总线（ME）导致的物品复制bug。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/380)）
* 修复了工业搅拌机输入总线独立失效的bug。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/379)）
* 合金冶炼炉部分配方更改。（by boubou19 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/382)）
  * 制作熔融铊的配方输出从3/4锭（108mB）改为2锭（288mB）。
  * 将熔融铊配方原料中洗净的铁矿石改为洗净的锌矿石。
  * 将熔融博特姆合金配方的处理时间从480s改为120s。
* 修正了重复的本地化key。（by iouter [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/381)）
* 更新了texture_api。（by leagris [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/386)）
* 删除了语言文件中的重复key。（by ChromicRedBrick [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/387)）
* 修复了最大堆叠小于64的物品在作物管理器中可以超限堆叠的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/391)）
* 修复了硫化铜\(II\)和氰化钠没有大化反合成配方的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/392)）
* 更新俄语语言文件。（by Eldrinn-Elantey [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/390)）
* 新加入巨型合金冶炼炉，是合金冶炼炉的升级版。（by MadMan310 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/394)）
  * UV阶段可以制造。
  * 最大256并行。
  * 有基于线圈等级的速度加成，为线圈等级/130，计算结果按千分位四舍五入，使用时永恒线圈达到10%的最大加成。结构中也可以使用冶炼炉线圈方块，此时没有速度加成。
  * UV+玻璃解锁激光仓，UEV+玻璃解锁所有等级能源仓。
  * 支持超过MAX电压的超频。
  * Shift+右键切换输入总线独立。
* 修复了脱水机配方没有编程电路，导致配方冲突的问题。（by Steelux8 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/393)）

### Galacticraft（星系）
* 版本号：3.0.44-GTNH → 3.0.45-GTNH
* yeet RuntimeException（by mitchej123 [相关pr](https://github.com/GTNewHorizons/Galacticraft/pull/54)）

### GoodGenerator
* 版本号：0.4.31 → 0.4.33
* 修复了大力合金有两个不同电压的高炉配方的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/88)）
* 修复了无法扫描YOT流体单元方块T9和T10配方的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/89)）

### Hodgepodge
* 版本号：1.7.35 → 1.7.37
* 修复了`speedupBOPFogHandling`不兼容的bug。（by makamys [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/129)）
* 修复了使用分割徽章去除附魔会导致复制物品的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/131)）
* 加入了有关dimension provider导致的游戏崩溃的debug log。（by miozune [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/132)）

### HydroEnergy
* 版本号：1.0.12 → 1.0.13
* 修复了mixin本地变量的注入。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/HydroEnergy/pull/17)）

### Infernal-Mobs
* 版本号：1.7.5-GTNH → 1.7.6-GTNH
* 限制了可以将玩家拉向自己的精英怪的最大作用距离。（by Glease [相关pr](https://github.com/GTNewHorizons/Infernal-Mobs/pull/11)）

### KekzTech
* 版本号：0.6.15 → 0.6.16
* 修改了兰波顿超级电容库计算平均输入输出的方式。（by TrainerSnow [相关pr](https://github.com/GTNewHorizons/KekzTech/pull/43)）

### KubaTech
* 版本号：0.5.10 → 0.5.11
* 工业屠宰场在超频到1t之后会按4/4的模式继续增加并行。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/KubaTech/pull/25)）

### LogisticsPipes（逻辑管道）
* 版本号：0.9.4.5.7-GTNH → 0.9.4.5.8-GTNH
* 修复了NEI幽灵物品拖放功能在逻辑管道中失效的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/LogisticsPipes/pull/12)）

### MX-Random
* 版本号：0.1.4 → 0.1.5
* 修复了从大型分子装配室中取走数据球导致的游戏崩溃问题。（by eigenraven [相关pr](https://github.com/GTNewHorizons/MX-Random/pull/5)）

### MagicBees（魔法蜜蜂）
* 版本号：2.5.12-GTNH → 2.5.13-GTNH
* 修复了语言文件中错误的本地化key。（by ChromicRedBrick [相关pr](https://github.com/GTNewHorizons/MagicBees/pull/13)）

### NewHorizonsCoreMod
* 版本号：1.9.80 → 1.9.83
* 删除了语言文件中的重复key。（by ChromicRedBrick [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/421)）
* 统一了组装机制作Ztones方块配方使用编程电路的格式，即对应序号的方块使用对应编程电路。（by miozune [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/423)）
* Buff了蒸汽时代的一些配方。（by Connor-Colenso [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/422)）
  * 研磨燧石：80s → 40s；
  * 将部分合金炉配方蒸汽需求量减为原来的一半；
  * 合金炉制作玻璃管：12s → 6s。

### OpenComputers（开放式电脑）
* 版本号：1.7.7.2-GTNH → 1.8.0.0-GTNH-pre
* 同步更新了源mod仓库的最新代码。（by asiekierka [相关pr](https://github.com/GTNewHorizons/OpenComputers/pull/81)）

### OpenPrinter
* 版本号：0.1.0.132 → 0.1.2-GTNH
* 更新了构筑。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/OpenPrinter/pull/3)）

### Realistic-World-Gen（真实世界生成）
* 版本号：alpha-1.3.2.1 → alpha-1.3.3.0
* 撤销了上版本中噪声生成器的变动，修复了世界生成高山过多、群系混乱的问题。（by eigenraven [相关pr](https://github.com/GTNewHorizons/Realistic-World-Gen/pull/3)）

### SleepingBags
* 版本号：0.1.3 → 0.1.4
* 添加了俄语语言文件。（by Eldrinn-Elantey [相关pr](https://github.com/GTNewHorizons/SleepingBags/pull/3)）

### StorageDrawers（储物抽屉）
* 版本号：1.11.17-GTNH → 1.11.18-GTNH
* 现在破坏抽屉时会掉落更少堆叠的物品，减少可能发生的卡死或崩溃。（掉落物品总量不变）（by wohaopa [相关pr](https://github.com/GTNewHorizons/StorageDrawers/pull/17)）

### TC4Tweaks
* 版本号：1.4.16 → 1.4.18
* 修复了神秘时代注魔配方不稳定度过高会导致游戏崩溃的bug。（by Alexdoru [相关pr](https://github.com/GTNewHorizons/TC4Tweaks/pull/11)）

### TecTech
* 版本号：5.0.39 → 5.0.42
* 修复了文本显示可能超出屏幕范围的问题。（by Connor-Colenso [相关pr](https://github.com/GTNewHorizons/TecTech/pull/102)）
* 修复了结构搭建中特斯拉电塔无法识别LuV线圈的bug。（by albus12138 [相关pr](https://github.com/GTNewHorizons/TecTech/pull/104)）
* 修正了重复的本地化key。（by iouter [相关pr](https://github.com/GTNewHorizons/TecTech/pull/103)）

### ThaumicHorizons（神秘视界）
* 版本号：1.2.1.6 → 1.2.1.7
* 删除了语言文件中的重复key。（by ChromicRedBrick [相关pr](https://github.com/GTNewHorizons/ThaumicHorizons/pull/36)）

### TinkersConstruct（匠魂）
* 版本号：1.9.4-GTNH → 1.9.6-GTNH
* 匠魂冶炼炉GUI中按Shift现在会精确显示流体的量(mB)。（by Glease [相关pr](https://github.com/GTNewHorizons/TinkersConstruct/pull/56)）
* 主动更新排液口比较器的输出。（by Glease [相关pr](https://github.com/GTNewHorizons/TinkersConstruct/pull/57)）

### TwilightForest（暮色森林）
* 版本号：2.3.8.16 → 2.3.8.17
* 删除了语言文件中的重复key。（by ChromicRedBrick [相关pr](https://github.com/GTNewHorizons/twilightforest/pull/17)）

### VisualProspecting
* 版本号：1.0.33 → 1.0.34
* 使用流体名而非ID保存扫描到的流体，修复了更新游戏后可能造成小地图流体显示错乱的bug。（by eigenraven [相关pr](https://github.com/GTNewHorizons/VisualProspecting/pull/21)）

### WarpTheory
* 版本号：1.2.6-GTNH → 1.2.7-GTNH
* 修复了config选项中allowWarpEffects处理不正确的问题。（by skizzerz [相关pr](https://github.com/GTNewHorizons/WarpTheory/pull/24)）
* 修复了游戏中扭曲守护效果可能永久激活的bug。（by skizzerz [相关pr](https://github.com/GTNewHorizons/WarpTheory/pull/24)）

## 任务书及配置文件更新
* 修复了数十条任务书文本的问题。（by chochem & Steelux8 [相关pr1](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11485) [相关pr2](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11522) [相关pr3](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11552) [相关pr4](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11576)）
* 植物魔法任务线扩充。（by hallucinogender [相关pr1](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11534) [相关pr2](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11550) [相关pr3](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11554)）
* 无尽、海珀珍、永恒三种线圈的任务增加了大量传说风格的叙述文本。（by Steelux8 [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11576)）
* 更新了默认服务器列表，加入了Zvezdolet GTNH 2.0和Zvezdolet GTNH Hardcore两个服务器。（by Ethryan [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11513)）
* 修复了水晶缠绕宇宙中子法杖无法合成的bug。（by wohaopa [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11515)）




参考文本：
> * [Changelog from DreamAssemblerXXL](https://github.com/GTNewHorizons/DreamAssemblerXXL/blob/master/releases/changelogs/changelog%20from%202.2.0.0%20to%202.2.3.md)
> * All pull requests and commits from [GTNewHorizons repositories](https://github.com/GTNewHorizons)
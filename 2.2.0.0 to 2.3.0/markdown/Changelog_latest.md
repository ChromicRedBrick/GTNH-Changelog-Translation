# 2.2.3至今更新内容



## Mod文件变动

## Mod更新

### AE2FluidCraft-Rework（AE2FC）
* 版本号：1.0.22-GTNH → 1.0.32-GTNH
* 修复了ME增广流体样板终端保存8种物品输出的配方会出现错误的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/25)）
* 修复了极端情况下流体样板编码可能会导致ArrayIndexOutOfBoundsException的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/26)）
* 为流体存储元件加入了显示过滤流体种类的tooltip。（by dipo33 [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/27)）
* 新增（AE2FC版）ME流体终端。支持显示每种最高long max量的流体。（by asdflj [相关pr1](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/28) [相关pr2](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/29) [相关pr3](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/30)）
* 阻挡模式支持流体p2p。（by guineawheek [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/31)）
* 修复了一个导致二合一接口无限输出流体的bug。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/32)）
* 在流体样板终端界面Shift+左键物品栏中的样板，现在会自动将其放到样板输出格，而不是放入ME网络库存内。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/33)）
* 加入了ME缓存指令器（ME Level Maintainer），用于让ME网络中某个物品保持在一定数量之内。支持开放式电脑（OC）相关控制。[^1]（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/36)）
* 大大提高了ME-IO端口输入/输出ME流体元件中流体的速度。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/36)）
* 可以将物品拖到AE2FC终端顶部搜索栏上，自动用物品名填充搜索栏（与原版AE2相同）。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/36)）
* AE2FC终端顶部搜索栏现在支持NEI搜索历史（需要将搜索模式调为NEI同步，使用Ctrl+鼠标滚轮调整历史条目）。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/36)）
* 修复了ME流体样板终端中Shift+鼠标左键双倍样板输入/输出对流体包不生效的bug。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/36)）
* 修复了格雷化（魔改）的AE2FC流体元件合成配方失效的bug。（by OneEyeMaker [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/37)）

[^1]: 源自懒人AE2（Lazy AE2）。

### Applied-Energistics-2-Unofficial（AE2）
* 版本号：rv3-beta-111-GTNH → rv3-beta-118-GTNH
* 改善了禁用频道时ME网络的性能表现。（by xyqyear [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/190)）
* 如果config禁用了充能赛特斯石英矿石的生成，那么NEI不会再显示"可以在世界中找到充能赛特斯石英"相关的信息。（即：GTNH中，NEI不会再显示"可以在世界中找到充能赛特斯石英"）（by miozune [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/191)）
* 撤回了之前对于压印器配方的更改（将其移动到整合包设置文件中），修复了在GTNH之外压印器配方丢失的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/192)）
* P2P通道-ME接口现在支持使用ME接口终端放置样板。（by greesyB [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/193)）
* 修复了在合成模拟界面取消涉及到奥术合成终端的合成会导致游戏崩溃的bug。（by greesyB [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/194)）
* 开启“启用替换”选项时，可以请求合成配方所需物品的同矿辞物品。[^2]（by eigenraven [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/195)）
* 进一步完善格式化数字文本。（by Connor-Colenso [相关pr](https://github.com/GTNewHorizons/Applied-Energistics-2-Unofficial/pull/197)）

[^2]: 例如编写样板：4橡木木板+4燧石→1工作台，开启“启用替换”功能，此时ME网络内没有任何种类的木板，但是有白桦木原木，同时也有1白桦木原木→4白桦木木板的合成样板。此时进行合成时，终端便会使用白桦木原木合成白桦木木板，再合成工作台。此前终端只会调取网络内已有的同矿辞物品，不够时不会请求合成。

### Bartworks
* 版本号：0.5.90 → 0.5.111
* 修复了细菌培养缸内部显示的流体方块没有lang key的问题。（by Quarri6343 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/209)）
* 修复了极限工业温室不支持多输入仓供水的bug。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/210)）
* 提高了极限工业温室设置模式的输入速度。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/210)）
* 加入了封装贴片电感的合成配方。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/bartworks/pull/212)）
* 加入了Bartworks材料的箔形式。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/bartworks/pull/213)）
* 修复了风车并行数计算错误导致的物品复制bug。（by iouter [相关pr](https://github.com/GTNewHorizons/bartworks/pull/214)）
* 将合成配方中使用的0号电路板改为1号。（by miozune [相关pr](https://github.com/GTNewHorizons/bartworks/pull/215)）
* 修复了[pr#210](https://github.com/GTNewHorizons/bartworks/pull/210)意外导致的物品复制bug。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/216)）
* 修复了风车输出物品没有正确分割的bug。（by iouter [相关pr](https://github.com/GTNewHorizons/bartworks/pull/217)）
* 加入了使用电动聚爆压缩机制造浓缩铀、钍、钚的新配方。（by GDCloudstrike [相关pr](https://github.com/GTNewHorizons/bartworks/pull/218)）
* 修复了电路元件矿辞化导致部分电路装配线配方（主要是集成逻辑电路）无法生成的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/bartworks/pull/219)）
* 修正了极限工业温室的结构tooltip文本。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/221)）
* 为巨型工业高炉、巨型真空冷冻机、巨型化学反应釜、巨型蒸馏塔加入了批处理模式，剪线钳Shift+右键切换。该模式旨在降低延迟。[^3]（by S4mpsa [相关pr](https://github.com/GTNewHorizons/bartworks/pull/225)）
* 修复了铱锇合金涡轮配方被钌铱合金错误替代的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/bartworks/pull/226)）
* 修复了硫酸钠粉电解配方会生成液态钠而不是钠粉的问题。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/bartworks/pull/227)）
* 修改了Bartworks材料的流体固化配方机制，现在默认情况下不会生成齿轮、螺栓、转子的流体固化配方，并且将配方生成分成了两个独立的选项，"addMetalCraftingSolidifierRecipes"会生成杆、板的流体固化配方，"addMetaSolidifierRecipes"会生成齿轮、螺丝、螺栓、环等的流体固化配方。（by Elisis [相关pr](https://github.com/GTNewHorizons/bartworks/pull/228)）
* 修复了存储输入总线（ME）会在机器内部的一格内输入超过一组种子的bug。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/230)）
* 将Bartworks生成线缆二极管及其配方的最高等级限制为UV。[^4]（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/231)）
* 修复了极限工业温室不支持云母草（Micadia）的问题。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/232)）
* 修复了IC2模式下作物产出计算错误的bug（略微nerf了IC2模式）。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/232)）
* 取消了盐根种子在极限工业温室中的湿度判定。盐根产量现在会正确地随种子G值增加而增加。[^5]（by xSkewer [相关pr](https://github.com/GTNewHorizons/bartworks/pull/233)）
* 修复了LuV部分使用到铂线材料的配方生成错误的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/bartworks/pull/234)）
* 修复了氯化钙流体产出钙过多的问题，将1000mB氯化钙→3氯化钙粉改为1000mB氯化钙→1氯化钙粉。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/bartworks/pull/236)）
* 修复了电路装配线和风车结构判定相关的bug。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/237)）

[^3]: 批处理模式可以为配方加上一个由输入原料量决定的并行系数，这个系数最大为128。最终的输入、输出为原最大并行量\*并行系数，同时配方处理时间也为原时间\*并行系数。批处理模式可以极大降低处理阵列造成的延迟，但不会增加其生产效率。
[^4]: 因为UHV+的线缆和线缆二极管配方在GTNewHorizonsCoreMod中定义，在Bartworks中不限制可能会导致配方问题。
[^5]: 湿度判定会导致盐根产量与种子G值的关系并不是单调递增的，而是在G=11或12时产量取得最大值。

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
* 新加入巨型合金冶炼炉，是合金冶炼炉的升级版。（by MadMan310 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/394) [discord特性前瞻](https://discord.com/channels/181078474394566657/295669878222880769/1028718667275440249)）
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
* 修改了兰波顿超级电容库计算平均输入输出的方式。[^3]（by TrainerSnow [相关pr](https://github.com/GTNewHorizons/KekzTech/pull/43)）

[^3]: 会导致进入存档崩溃，解决方法为手动更新TecTech。

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




> 参考文本：
> * [Changelog from DreamAssemblerXXL](https://github.com/GTNewHorizons/DreamAssemblerXXL/blob/master/releases/changelogs/changelog%20from%202.2.0.0%20to%202.2.3.md)
> * All pull requests and commits from [GTNewHorizons repositories](https://github.com/GTNewHorizons)
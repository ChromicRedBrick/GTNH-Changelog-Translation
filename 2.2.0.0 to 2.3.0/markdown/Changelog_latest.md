# 2.2.3至今更新内容



## Mod文件变动

## Mod更新

### AE2FluidCraft Rework（AE2FC）
* 版本号：1.0.22-GTNH → 1.0.32-GTNH
* 修复了ME增广流体样板终端保存8种物品输出的配方会出现错误的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/25)）
* 修复了极端情况下流体样板编码可能会导致ArrayIndexOutOfBoundsException的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/26)）
* 为流体存储元件加入了显示过滤流体种类的tooltip。（by dipo33 [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/27)）
* 新增（AE2FC版）ME流体终端。支持显示每种最高long max量的流体。（by asdflj & GlodBlock [相关pr1](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/28) [相关pr2](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/29) [相关pr3](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/30)）
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

### Applied Energistics 2 Unofficial（AE2）
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

### BetterCrashes
* 版本号：1.1.6-GTNH → 1.1.7-GTNH
* 精简了ModIdentifier相关后台日志。（by miozune [相关pr](https://github.com/GTNewHorizons/BetterCrashes/pull/7)）

### BetterQuesting（更好的任务）
* 版本号：3.1.0-GTNH → 3.1.4-GTNH
* 修复了在NEI任务界面中，无法获取任务本地化名称的bug。（by iouter [相关pr](https://github.com/GTNewHorizons/BetterQuesting/pull/80)）
* 修复了打开空任务线时游戏偶尔会未响应的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/BetterQuesting/pull/81)）
* 修复了任务书设置中主题重复的bug。（by eigenraven [相关pr](https://github.com/GTNewHorizons/BetterQuesting/pull/82)）
* 修复了在服务器中可重复任务进度不会重置的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/BetterQuesting/pull/83)）

### BloodMagic（血魔法）
* 版本号：1.3.16 → 1.3.18
* 修复了当服务器请求仪式推测杖的本地化文本时会导致崩溃的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/BloodMagic/pull/35)）
* 修正了NEI坠星仪式矿石数量估计的算式错误。（by ChromicRedBrick [相关pr](https://github.com/GTNewHorizons/BloodMagic/pull/36)）

### Botania
* 版本号：1.9.10-GTNH → 1.9.11-GTNH
* 修复了ManaNetworkHandler的一个内存泄漏问题。（by Glease [相关pr](https://github.com/GTNewHorizons/Botania/pull/18)）

### Crops plus plus
* 版本号：1.3.6.4 → 1.3.6.8
* 移除了夜光珊瑚高压釜配方生产阳光化合物中的随机概率，将50%出4个阳光化合物粉改为100%出2个。（by dipo33 [相关pr](https://github.com/GTNewHorizons/Crops-plus-plus/pull/44)）
* 修复了作物矿辞相关的问题。（by Glease [相关pr](https://github.com/GTNewHorizons/Crops-plus-plus/pull/45)）
* 加入了魔豆作物。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/Crops-plus-plus/pull/46)）

### DefaultServerList
* 版本号：1.1.1 → 1.4.0
* 同步原mod的更新。（by glowredman [相关pr](https://github.com/GTNewHorizons/DefaultServerList/pull/1)）
* 允许拖拽改变默认服务器列表排序。（by Quarri6343 [相关pr](https://github.com/GTNewHorizons/DefaultServerList/pull/2)）
* 修复了默认服务器列表不会随配置文件更新的bug。（by wohaopa [相关pr](https://github.com/GTNewHorizons/DefaultServerList/pull/3)）
* 加入了curseforge和modrinth上本mod项目的相关信息。（因为mod现在发布到了这两个网站上）（by glowredman [相关pr](https://github.com/GTNewHorizons/DefaultServerList/pull/4)）
* 以临时文件的形式获取Changelog。（by glowredman [相关pr](https://github.com/GTNewHorizons/DefaultServerList/pull/5)）

### Electro Magic Tools（电动魔法工具）
* 版本号：1.2.8.21 → 1.2.8.23
* 修复了大型源质发电机和奥法研究阐释者控制器方块ID对调的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/Electro-Magic-Tools/pull/49)）
* 将所有数字格式化。（by Connor-Colenso [相关pr](https://github.com/GTNewHorizons/Electro-Magic-Tools/pull/50)）

### EnderIO（末影接口）
* 版本号：2.3.1.47 → 2.3.1.48
* 将RandomThings的沃土加入种植站识别的耕地列表中。（by miozune [相关pr](https://github.com/GTNewHorizons/EnderIO/pull/87)）

### Eternal Singularity（永恒奇点）
* 版本号：1.0.4 → 1.0.5
* 回退着色器版本，修复了MacOS的兼容性问题。（by LionZXY [相关pr](https://github.com/GTNewHorizons/Eternal-Singularity/pull/2)）

### ExtraCells2
* 版本号：2.5.24 → 2.5.25
* 使EC2的网络部件和AE2部件采取一致的渲染方式。（by dipo33 [相关pr](https://github.com/GTNewHorizons/ExtraCells2/pull/71)）

### ForestryMC（林业）
* 版本号：4.4.16 → 4.5.6
* 更改了蜜蜂产出计算公式。现在产出公式为：$$P=\left(1+\frac{t}{6}\right)\cdot\left(\left(x\right)^{\frac{1}{2}}\right)\cdot2\left(1+s\right)+p^{\left(x^{\frac{1}{3}}\right)}-3$$[^6]（by kuba6000 [相关pr](https://github.com/GTNewHorizons/ForestryMC/pull/31)）
* 巨型红杉树的突变不再需要夜晚和特定生物群系。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/ForestryMC/pull/32)）
* 将GT中蜜蜂加速效果相关代码移到林业Mod中。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/ForestryMC/pull/34)）
* 加入了对蜜蜂愉快属性的描述。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/ForestryMC/pull/35)）
* 修复了潜在的内存泄漏问题。（by Glease [相关pr](https://github.com/GTNewHorizons/ForestryMC/pull/36)）
* 修复一处拼写错误。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/ForestryMC/pull/38)）
* 修复了Biomes O'Plenty（超多生物群系）中芜青种子提取出种子油的量为0的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/ForestryMC/pull/39)）

[^6]: $x$为基础产出概率，$s$为蜜蜂速度，$p$为生产加速，$t$为不同蜂箱的修正系数，$P$为最终产出概率。

### Galacticraft（星系）
* 版本号：3.0.45-GTNH → 3.0.47-GTNH
* 在配置文件中添加"Enable Oxygen Tank Hand fill"（启用手动填装氧气罐）条目，启用后可以直接用GC的罐装液态氧和氧气罐合成得到满的氧气罐。（by Glease [相关pr](https://github.com/GTNewHorizons/Galacticraft/pull/55)）
* 修复了玩家提前跳下登陆舱会导致无法打开着陆气球的bug。（by glowredman [相关pr](https://github.com/GTNewHorizons/Galacticraft/pull/57)）

### GalaxySpace
* 版本号：1.1.16p-GTNH → 1.1.19-GTNH
* **不要问我更新了什么，我不知道**

### GoodGenerator
* 版本号：0.4.33 → 0.4.48
* 多方块自动放置功能完善。[^7]（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/83)）
* 修复了热大力合金锭没有真空冷冻机处理配方的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/90)）
* 修复了之前更新导致的中子活化器结构检测失败的问题。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/92)）
* 修复了几个YOT储罐的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/94)）包括：
  * 修复了YOT储罐不识别UEV+玻璃的问题。修复之后，YOT储罐存储单元的等级和需求的玻璃等级正确地一一对应。
  * 修复了YOT储罐的延迟问题。
  * YOT仓现在最大可以访问max long mB的流体。[^8]
  * YOT仓现在最大可以每t输入/输出max long mB的流体。
* 加入了硅岩基流体燃料MkIV和MkV的新配方，是原配方的高阶替代，使用更后期的材料为原料，旨在为游戏后期提供更高效率的硅岩燃料生产手段。（by GDCloudstrike [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/91)）
* 将精密自动组装机tooltip中的"0.03mm"改为"7nm"。（by MadMan310 [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/95)）
* 修复了GoodGenerator的IC2核反应堆燃料棒正常枯竭后会生成堆叠数为0的枯竭燃料棒的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/98)）
* 硅岩燃料相关配方调整。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/96)）
  * 调整了原子分离催化剂的合成配方：9个火石粉改为4个火石粉，暗影金属粉改为龙尘，基岩锭粉改为量子锭粉，移除了阳光化合物粉、铕粉、灵宝锭粉合成的配方，统一产出为63个原子分离催化剂粉。
  * 调整了合成玉板的合成配方：4个泰伯利亚板改为1个泰伯利亚板。
  * 调整了硅岩燃料精炼厂相关方块的配方：统一为UHV+等级。
* 硅岩基流体燃料MkI、MkII和MkIII重做，旨在让这三种燃料成为ZPM~UHV阶段等离子发电的相近水平替代品。（by xSkewer [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/99)）
  * 硅岩乳液相关配方buff。
  * 重做后的硅岩基流体燃料-MkI定位为ZPM末期。
  * 重做后的硅岩基流体燃料-MkII定位为UV中期。
  * 重做后的硅岩基流体燃料-MkIII定位为UHV中期。
  * 具体内容请看相关pr。
* 钍相关配方平衡调整。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/76)）
  * 枯竭的钍基流体燃料不再产出镥，改为钍-232。
  * 大型化学反应釜制造钍-232的产线消耗氟量增多。
  * 钍基流体燃料降价。
  * 枯竭的浓缩钚燃料棒离心产出由氪改为氩。
* YOT储罐现在支持流体探测覆盖板。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/101)）
* YOT储罐加入开关溢出销毁选项。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/100)）
* YOT储罐不再需要维护仓。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/104)）
* 配平了氢氧化镓粉与钠粉反应的配方消耗和产出的钠数量。

[^7]: 包括：压缩核聚变反应堆、精密自动组装机、冷却塔、大型源质发电机、大型源质冶炼厂、大型硅岩反应堆、中子活化器、硅岩燃料精炼厂、通用化学能引擎、YOT储罐、极限热交换机。
[^8]: 例如：ME流体存储总线接YOT仓时，以前最多只能读取int long (2^31) mB的流体，现在可以读到最多max long (2^62) mB。

### GT5 Unofficial（格雷科技）
* 版本号：5.09.41.74 → 5.09.41.132
* 凛冰蜂主产出改为暴雪蜂窝，概率15%，离心产出暴雪棒，特殊产物凛冰蜂窝概率从15%改为20%。（by Runakai1 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1443)）
* 破坏超级缸时，只保留流体种类和存量这两个必要信息，不保留超级缸的设置模式。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1448)）
* 允许使用胶带直接右键维护仓维护机器，不需要打开GUI。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1451)）
* 泵[^9]现在不会自动收回采矿管道，只有用软锤右键的时候才会收回。电烙铁右键泵可以切换回触底自动收回模式。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1449)）
* 超级箱/量子箱优化。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1450)）
  * 支持输入过滤。
  * WAILA支持显示储存物品相关信息。
  * 在代码中统一了超级箱和量子箱。
* 将新的蜜蜂产出公式[^10]应用于工业蜂箱。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1447)）
* 将工业蜂箱的升级从Gendustry（基因工业）移动到GT中。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1447)）
* 将UIV~MAX的机器部件加入到机器配方生成列表中。（by S4mpsa [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1452)）
* 添加了将Gendustry（基因工业）的升级框架转换为GT版本的配方。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1453)）
* 撤回对白千层树的更改[^11]，并且在Mod依赖中移除了Harvestcraft（潘马斯）。（by Alastors [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1459)）
* 修复了`CoverDataSetter`相关的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1458)）
* 大型热交换机加入热量计数器，当蒸馏水不足时，需要过100秒才会达到最大热量而爆炸。此计数器只与爆炸有关。（by Steelux8 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1455)）
* 加入了配置蜜蜂效果能否加速的接口。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1460)）
* 修正了重复的本地化key。（by iouter [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1457)）
* 修复了GT蜂窝无法本地化的问题。（by iouter [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1454)）
* 将配置蜜蜂效果能否加速的接口移动至Forestry。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1462)）
* 修复了超级缸开启溢出销毁模式时，WAILA显示储量错误的bug。（by Matriac [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1463)）
* 修复了超级缸开启溢出销毁模式时，流体探测覆盖板红石行为错误的bug。（by Matriac [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1464)）
* 处理阵列现在支持处理最高long max的功率。（by BlueWeabo [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1465)）
* 修复了GT工具对其他模组支持使用了错误的Mod ID的问题，也即修复了GT工具无法正确代替其他Mod对应工具使用的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1466)）
* 将蜂窝矿辞从整合包设置文件移动到GT代码中。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1468)）
* 修复了NEI中蒸汽机器配方总蒸汽使用量计算错误的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1467)）
* 修正了工业高炉结构的tooltip。现在的表述为：液体形式的流体输出仓位于底层机械方块，气体形式的流体输出仓位于顶层机械方块。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1469)）
* 限定无尽、宇宙中子素、无尽催化剂、镅、氪蜂窝只能在巨型蜂箱（Mega Apiary）中产出。（by Runakai1 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1470)）
* 修复了之前更新导致意外的蜜蜂产出提升的问题。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1472)）
* 修复了之前更新未考虑蜂箱升级数量效果叠加的问题。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1474)）
* 为GT扳手加入了对ProjectRed（红石计划）扳手的支持。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1475)）
* 加入了ME输出仓，可以直接将流体输出到ME网络中。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1473)）
* 修复了重载材质会导致GT流体材质丢失的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1477)）
* 取代了代码中一处`gridproxy`，修复了一项空指针异常。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1478)）
* 修复了客户端没有正确读取机器流体槽位，使得填充流体槽时会先消耗错误数量的流体再与服务端同步修正的问题。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1480)）
* 移除了将Gendustry（基因工业）的蜜蜂转换为GT蜜蜂的代码。（by DianeXD [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1187)）
* 将方块被破坏时是否应该掉落其内容物的检测加入到API中。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1479)）
* 加入了铝土、钛铁、蓝宝石、石榴石等一系列用途较少矿石的新处理线，可以从中获取一些有用的产物。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1210)）
* 将多重锭/板、齿轮、转子等一系列部件的最大堆叠数改为64。（by Phineasor [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1484)）
* 用钛-铂-钒（TPV）线圈代替了钨钢线圈。TPV的成分为3:3:1的钛、铂、钒。意在减少EV阶段对钨钢的需求，以及鼓励在EV制作自动化的铂产线。（by Steelux8 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1211)）
* 修复了一系列的配方bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1489)）
  * 修复了Botania（植物魔法）中玄武岩台阶和玄武岩板的配方冲突。
  * 修复了部分配方中单元数量不守恒的问题。
  * 修复了板材切割机存在空输出配方的问题。
  * 修复了GT玄武岩切割配方重复的问题。
  * 修复了GT玄武岩相关配方不平衡的问题。
* 修复了四重输入仓在特殊情况下会吞流体的bug。（by guineawheak [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1487)）
* 加入了含内部存储的能源仓的构造器，意在修复GT++的相关bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1488)）
* 强制工业蜂箱最多请求4A电流，修复了工业蜂箱无法获取足够功率的bug。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1492)）
* 修复了某些情况下机器控制覆盖板会在聊天栏中刷屏的bug。（by johnch18 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1490)）
* 允许超净间结构中放置最多2个门，意在使Alastors能够心满意足，安心睡觉。（by POPlol333 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1493)）
* 加入了从Forge流体中创建GT材料的方法。（by Elisis & Glease [相关pr1](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1497) [相关pr2](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1502)）
* 加入了集成矿石处理厂相关成就的本地化key。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1499)）
* 加入了新回旋加速器多方块结构所需的线圈方块。[^12]（by Conner-Colenso [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1494)）
* 更改了引擎进气机械方块的材质。（by leagris [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1500)）
* 修复了物品tooltip中的原始类型（raw type）警告。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1501)）
* 修正了集成矿石处理厂的消声仓和输入仓使用的索引。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1503)）
* 覆写了存储输入总线（ME）代码中的`setStackToZeroInsteadOfNull`，修复了相关bug。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1504)）
* 修复了拆解机无法正确处理含有容器的配方的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1505)）
* 移除了对IC2燃油罐的兼容。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1506)）
* 基于新的蜜蜂产出公式[^10]，调整了部分蜂窝的产出概率。（by Runakai1 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1508)）
* 修复了蕴魔蜂突变需求，与对应的要素匹配。（by Runakai1 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1508)）
* 修复了`depleteInput`只读取多重输入仓第一格内容的bug，从而可以在例如大型内燃引擎上使用1个四重输入仓处理所有需要的流体。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1509)）
* 加入了EV和IV单方块燃气涡轮，燃料效率分别为60%和50%。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1511)）
* 修正了木炭气蒸馏配方的一氧化碳输出量，由2340mB改为240mB。（by OneEyeMaker [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1512)）
* 修复了在加入EV和IV燃气涡轮后，继续使用旧的配置文件，会导致游戏崩溃的bug。（by Quarri6343 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1516)）
* 修复了在[上一项更新](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1516)后，大型燃气涡轮不消耗燃料的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1517)）
* 加入了量子力转换机（Quantum Force Transformer）多方块结构[^13]相关的机械方块。（by Steelux8 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1514)）
* 加入了由[Jimbno](https://github.com/Jimbno)设计的几种新披风。（by boubou19 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1519)）
* 修复了当包含空堆叠的物品组由`getNonUnidiedStack`处理时，游戏崩溃的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1520)）

[^9]: 指GT单方块机器“泵”，不是电动泵覆盖板。
[^10]: 见ForestryMC（林业）更新部分。
[^11]: 对白千层树的更改见[这条pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/917) 。
[^12]: 见GoodGenerator更新部分。
[^13]: 见GTplusplus（GT++）更新部分。

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
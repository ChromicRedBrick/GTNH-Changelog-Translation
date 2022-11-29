# 2.2.3至今更新内容

## Mod文件变动

## Mod更新

### AE2FluidCraft Rework（AE2FC）
* 版本号：1.0.22-GTNH → 1.0.36-GTNH
* 修复了ME增广流体样板终端保存8种物品输出的配方会出现错误的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/25)）
* 修复了极端情况下流体样板编码可能会导致ArrayIndexOutOfBoundsException的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/26)）
* 为流体存储元件加入了显示过滤流体种类的tooltip。（by dipo33 [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/27)）
* 新增（AE2FC版）ME流体终端。支持显示每种最高long max量的流体。（by asdflj & GlodBlock [相关pr1](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/28) [相关pr2](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/29) [相关pr3](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/30)）
* 阻挡模式支持流体p2p。（by guineawheek [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/31)）
* 修复了一个导致二合一接口无限输出流体的bug。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/32)）
* 在流体样板终端界面Shift+左键物品栏中的样板，现在会自动将其放到样板输出格，而不是放入ME网络库存内。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/33)）
* 加入了ME缓存指令器（ME Level Maintainer），用于让ME网络中某个物品保持在一定数量之内。支持开放式电脑（OC）相关控制。[^1]（by asdflj [相关pr1](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/36) [相关pr2](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/41)）
* 大大提高了ME-IO端口输入/输出ME流体元件中流体的速度。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/36)）
* 可以将物品拖到AE2FC终端顶部搜索栏上，自动用物品名填充搜索栏（与原版AE2相同）。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/36)）
* AE2FC终端顶部搜索栏现在支持NEI搜索历史（需要将搜索模式调为NEI同步，使用Ctrl+鼠标滚轮调整历史条目）。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/36)）
* 修复了ME流体样板终端中Shift+鼠标左键双倍样板输入/输出对流体包不生效的bug。（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/36)）
* 修复了格雷化（魔改）的AE2FC流体元件合成配方失效的bug。（by OneEyeMaker [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/37)）
* 在ME流体封包解码器中加入了限制输入流体的槽位（by asdflj [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/39)）
* 为ME二合一接口加入了OC（开放式电脑）相关的API。（by GlodBlock [相关pr1](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/40) [相关pr2](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/42)）
* 修复了当样板只含有流体时，二合一接口阻挡模式不生效的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/38)）
* 禁止流体样板终端在合成模式下更改样板中物品数量。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/AE2FluidCraft-Rework/pull/38)）

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
* 版本号：0.5.90 → 0.5.116-pre
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
* 修复了极限工业温室可能导致玩家物品栏崩坏的bug。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/235)）
* 修复了巨型石油裂化机的自动放置问题。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/bartworks/pull/238)）

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

### BloodArsenal（血液兵工厂）
* 版本号：1.2.6 → 1.2.7
* 修复了可携式祭坛的tooltip会导致游戏崩溃的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/BloodArsenal/pull/15)）

### BloodMagic（血魔法）
* 版本号：1.3.16 → 1.3.18
* 修复了当服务器请求仪式推测杖的本地化文本时会导致崩溃的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/BloodMagic/pull/35)）
* 修正了NEI坠星仪式矿石数量估计的算式错误。（by ChromicRedBrick [相关pr](https://github.com/GTNewHorizons/BloodMagic/pull/36)）

### Botania（植物魔法）
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
* 版本号：2.5.24 → 2.5.27
* 使EC2的网络部件和AE2部件采取一致的渲染方式。（by dipo33 [相关pr](https://github.com/GTNewHorizons/ExtraCells2/pull/71)）
* 使EC2流体发信器、流体输入/输出总线支持NEI幽灵物品拖放标记。（by asdflj [相关pr](https://github.com/GTNewHorizons/ExtraCells2/pull/73)）

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
* 版本号：3.0.45-GTNH → 3.0.52-GTNH-pre
* 在配置文件中添加"Enable Oxygen Tank Hand fill"（启用手动填装氧气罐）条目，启用后可以直接用GC的罐装液态氧和氧气罐合成得到满的氧气罐。（by Glease [相关pr](https://github.com/GTNewHorizons/Galacticraft/pull/55)）
* 修复了玩家提前跳下登陆舱会导致无法打开着陆气球的bug。（by glowredman [相关pr](https://github.com/GTNewHorizons/Galacticraft/pull/57)）
* 修复了星系服装会跨存档渲染的bug。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/Galacticraft/pull/59)）
* 更新build script，使用GTNHMixins，并且精简了代码。（by glowredman [相关pr](https://github.com/GTNewHorizons/Galacticraft/pull/58)）

### GalaxySpace
* 版本号：1.1.16p-GTNH → 1.1.19-GTNH
* **不要问我更新了什么，我不知道**

### GoodGenerator
* 版本号：0.4.33 → 0.4.56
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
* 配平了氢氧化镓粉与钠粉反应的配方消耗和产出的钠数量。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/105)）
* 允许精密自动组装机超过MAX功率超频。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/106)）
* 枯竭钍基流体燃料离心配方产出32个镨粉的概率从10%改为100%。（by querns [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/107)）
* 加入了部件装配线（Component Assembly Line）多方块结构。（by MadMan310 [相关pr](https://github.com/GTNewHorizons/GoodGenerator/pull/102)）详细内容如下：
  * 定位为UV+机器。
  * 该多方块结构可以大批量高效制造LV~UMV的基础部件（例如电动马达、电动泵、电动活塞等等），旨在提高后期基础部件产能，腾出装配线空间。
  * 所有配方都是自动生成的，输入48倍原料，输出64倍产物。部分原料会转换成流体、多倍线缆、致密板形式。
  * 机器能制造的部件等级受结构顶部的部件装配线机械方块限制，机械方块有LV~MAX等级，需要用对应等级的部件、电路板、材料合成。
  * 支持超过MAX的超频。
  * 支持TecTech激光仓和多安能源仓。

[^7]: 包括：压缩核聚变反应堆、精密自动组装机、冷却塔、大型源质发电机、大型源质冶炼厂、大型硅岩反应堆、中子活化器、硅岩燃料精炼厂、通用化学能引擎、YOT储罐、极限热交换机。
[^8]: 例如：ME流体存储总线接YOT仓时，以前最多只能读取int long (2^31) mB的流体，现在可以读到最多max long (2^62) mB。

### GT5 Unofficial（格雷科技）
* 版本号：5.09.41.74 → 5.09.41.151-pre
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
* 限定无尽、宇宙中子态素、无尽催化剂、镅、氪蜂窝只能在巨型蜂箱（Mega Apiary）中产出。（by Runakai1 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1470)）
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
* 加入了含内部存储的能源仓的构造器，意在修复GT++ RTG动力单元相关的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1488)）
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
* 修复了`depleteInput`只读取多重输入仓第一格内容的bug，从而可以在例如大型内燃引擎上使用一个四重输入仓处理所有需要的流体。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1509)）
* 加入了EV和IV单方块燃气涡轮，燃料效率分别为60%和50%。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1511)）
* 修正了木炭气蒸馏配方的一氧化碳输出量，由2340mB改为240mB。（by OneEyeMaker [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1512)）
* 修复了在加入EV和IV燃气涡轮后，继续使用旧的配置文件，会导致游戏崩溃的bug。（by Quarri6343 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1516)）
* 修复了在[上一项更新](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1516)后，大型燃气涡轮不消耗燃料的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1517)）
* 加入了量子力转换机（Quantum Force Transformer）多方块结构[^13]相关的机械方块。（by Steelux8 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1514)）
* 加入了由[@Jimbno](https://github.com/Jimbno)设计的几种新披风。（by boubou19 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1519)）
* 修复了当包含空堆叠的物品组由`getNonUnidiedStack`处理时，游戏崩溃的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1520)）
* 增加了支持机器功率以long值处理的`MultiBlockBase`文件，并且同时支持普通和TecTech能源仓。（by GlodBlock & BlueWeabo [相关pr1](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1521) [相关pr2](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1523)）
* 计算超频时，机器的功率现在以long值处理。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1522)）
* 使用ModularUI重写了GUI。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1381)）比较重要的更改内容如下：
  * 所有虚拟库存栏位现在都会自动支持NEI幽灵物品拖放。例如存储输入总线（ME）。
  * NEI配方界面会忽略物品/流体槽位之外的UI部分，由ModularUI提供的“进度条”动画替代。
  * NEI配方界面中，GT机器配方本身的区域会突出显示。
  * NEI多方块机器和单方块机器配方显示中输入输出槽位的风格统一。
  * 部分“进度条”动画是回环式的，例如洗矿厂、搅拌机。
  * 机器的名称标题会绘制于GUI主窗口上方，并且选项卡的样式是可配置的。不会再出现标题重叠。
  * 支持虚拟电路板的机器GUI右下角的GregTech图标替换成了更加有辨识度的“电路槽位”样式。
  * 解决了例如碎石机一类的配方需要编程电路，但是机器没有可用实体槽位的情况下的NEI配方显示问题。
  * 覆盖板窗口与服务端同步。服务器中其他玩家配置覆盖板的时候，客户端也会同步更改。并且如果在GUI打开的情况下有玩家移除了覆盖板，GUI窗口会立刻关闭。
  * 点击覆盖板标签栏会打开浮于机器主GUI上方的可拖动配置窗口。可以同时打开多个覆盖板配置窗口。
  * 数字文本`field`支持使用数学表达式。
  * 修复了工业蜂箱中“插入已分析蜜蜂以查看详细信息”无法正常工作的bug。
  * 原有资源包对GUI的更改会失效，需要重做。
* 加入了聚苯并咪唑管道方块、高级过滤机械方块、核能之星（Nuclear Star），用于部件装配线（Component Assembly Line）的结构方块和处理配方。[^12]（by MadMan310 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1524)）
* 修复了使用存储输入总线（ME）的机器开启配方锁定会导致原料不消耗的bug。（by repo-alt [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1526)）
* 允许自定义NEI和基础机器界面中的GregTech图标。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1525)）
* 将ModularUI的功能移动至底层代码。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1510)）
* Nerf了甲烷加水在化学反应釜中生成氢的配方，现在原料需要使用蒸馏水，并且基础配方时间从8.75秒增加到10秒。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1525)）
* WAILA支持显示方块上的所有覆盖板信息。（by miozune [相关pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/1527)）

[^9]: 指GT单方块机器“泵”，不是电动泵覆盖板。
[^10]: 见ForestryMC（林业）更新部分。
[^11]: 对白千层树的更改见[这条pr](https://github.com/GTNewHorizons/GT5-Unofficial/pull/917) 。
[^12]: 见GoodGenerator更新部分。
[^13]: 见GTplusplus（GT++）更新部分。

### GTNEIOrePlugin
* 版本号：1.0.17 → 1.0.18
* 更新了由@Jimbno提供的新材质。（by miozune [相关pr](https://github.com/GTNewHorizons/GTNEIOrePlugin/pull/23)）

### GTNH Lanthanides
* 版本号：0.9.18 → 0.9.20
* 加入了一系列流体的本地化key。（by ArtherCasan [相关pr](https://github.com/GTNewHorizons/GTNH-Lanthanides/pull/39)）
* 修正了配方中的单元数量平衡。（by miozune [相关pr](https://github.com/GTNewHorizons/GTNH-Lanthanides/pull/40)）

### GTNHLib
* 版本号：0.0.6 → 0.0.7
* 添加了服务端请求客户端在快捷栏上显示信息的API。（by miozune [相关pr](https://github.com/GTNewHorizons/GTNHLib/pull/11)）

### GTNHMixins
* 版本号：2.0.2（新Mod）

### GTplusplus（GT++）
* 版本号：1.7.118-pre → 1.7.149-pre
* 将化工厂定位为MV可制作，并且统一制作材料为MV级别。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/396)）
* 回退了对无菌农场机械方块造价的nerf，并且调整藻类农场控制器方块的造价为MV级别。（by Steelux8 [相关pr1](https://github.com/GTNewHorizons/GTplusplus/pull/397) [相关pr2](https://github.com/GTNewHorizons/GTplusplus/pull/402)）
* 将无尽突变催化剂配方的输出从1调整为5，以匹配输入消耗的5个催化剂外壳。（by Steelux8 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/398)）
* 修复了GT++材料不显示本地化的bug。（by iouter [相关pr1](https://github.com/GTNewHorizons/GTplusplus/pull/395) [相关pr2](https://github.com/GTNewHorizons/GTplusplus/pull/404) [相关pr3](https://github.com/GTNewHorizons/GTplusplus/pull/405)）
* 由于TPV线圈的加入[^14]，修改了化工厂手册的描述。（by miozune [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/409)）
* 修复了作物管理器在log中`NoSuchElementException`刷屏的bug。（by guineawheek [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/408)）
* 修复了硫镉矿石电解配方产出过多的问题。（by miozune [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/410)）
* 修复了氯乙酸混合物制作配方不返还空单元的问题。（by miozune [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/410)）
* 移除了RTG动力单元的反射。（by miozune [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/411)）
* 修改了一些GT++材料的等级顺序。（by Steelux8 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/403)）
* 略微降低了半流质的造价，并且使LV半流质发电机在LV阶段即可制作。（by Steelux8 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/403)）
* 加入了XL超临界蒸汽涡轮。与其他XL涡轮基本属性一致。（by GlodBlock [相关pr1](https://github.com/GTNewHorizons/GTplusplus/pull/413) [相关pr2](https://github.com/GTNewHorizons/GTplusplus/pull/414)）
* 修复了因代码问题导致能源站实际损耗为10%的bug，修正到5%。（by chochem [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/417)）
* 更改了量子反常的材质，新材质由@Jimbno制作。（by Connor-Colenso [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/415)）
* 允许原木拟生场种植腐化树苗。（by guineawheek [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/418)）
* GT++多方块机器控制器和结构方块配方使用材料等级统一，并且加入组装机配方便于自动化。（all by Dream-Master）
  * EV：工业焦炉（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/433)）
  * IV：工业线缆机（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/434)）、工业搅拌机（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/430)）、炽焱高炉（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/435)）、工业电解机（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/429)）、工业热力精炼厂（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/426)）、工业筛选机（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/428)）、工业洗矿厂（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/421)）、工业粉碎机（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/427)）、珠海渔场（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/421)）、工业压模机（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/424)）、合金冶炼炉（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/419)）、工业离心机（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/437)）、工业辊压机（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/437)）、工业切割机（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/437)）
  * LuV：亚马逊仓库（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/436)）
  * UV：质量发生器（[相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/437)）
* 修复了部分有序合成配方失效的问题。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/438)）
* 修复了部分GT++材料在锻造锤配方中不是3锭→2板的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/438)）
* 移除了涡轮材质的反射。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/439)）
* 用`static`修饰所有结构定义field。（by Glease [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/443)）
* 使用ModularUI重写了GUI。（by miozune [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/440)）
* 修复了反应堆燃料精炼厂GUI材质缺失的问题。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/447)）
* 在XL涡轮的tooltip中加入了需求30个涡轮轴方块的描述。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GTplusplus/pull/448)）

[^14]: 见GT5 Unofficial（格雷科技）更新部分。

### HarvestCraft（潘马斯）
* **未知更新**

### Hodgepodge
* 版本号：1.7.37 → 2.0.8
* 将ModMixins重新并入Hodgepodge。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/134)）
* 加快了`World.updateEntites`移除方块实体的速度，修复了某些情况下区块重载会导致方块实体停止工作的bug。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/133)）
* 修复了未启用fastcraft时，Opis在服务器中默认启用，产生延迟的问题。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/133)）
* 更新到Hodgepodge 2.0。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/116)）
  * 使用GTNHMixins 2.0。
  * 使用`IEarlyMixin`和`ILateMixin`，将mixins重新分为`early/`和`late/`。
  * 不再以JAR文件名称匹配Mod，而是使用已加载核心Mod类的列表，以及Mod id。
  * 重新组织Mod项目的结构，使之更直观，并且极大减少了意外的早期类加载。
  * 移除了多余的`getBlock()`修复内容。
  * 移除了GT5u锯子采集冰块相关的修复，该修复已移动到GT5u的代码中。
  * 应用Hodgepodge 2.0更新，需要移除SpongeMixins、ModMixins，并添加GTNHMixins 2.0.0以上版本。
* 修复了`Tunnel Bore mixin`。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/135)）
* 修复了一处拼写错误。（by Alexdoru [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/137)）
* 加入了在CurseForge上使用的相关Mod依赖列表。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/138)）
* 修复了食用堆叠的蘑菇煲会全部消耗，只返还1个碗的bug。（by wlhlm [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/141)）
* 加入了在CurseForge上使用的可选Mod依赖列表。（by glowredman [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/139)）
* 修复了未安装NEI时，`fixPotionEffectRender`会导致游戏崩溃的bug。并且正确地将该修复应用于原版NEI和GTNH版NEI。（by makamys [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/142)）
* 修复了兼容类会导致服务端崩溃的bug。（by makamys [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/144)）
* 修复了原版中玩家的某些声音被注册为友好生物的bug。（by Cleptomania [相关pr](https://github.com/GTNewHorizons/Hodgepodge/pull/143)）

### HoloInventory
* 版本号：2.1.17-GTNH → 2.1.18-GTNH
* 修复了安装了OptiFine时，全息眼镜在特定角度下不会显示抽屉内容物的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/HoloInventory/pull/29)）

### HydroEnergy
* 版本号：1.0.13 → 1.0.14
* 修复了在Apple Silicon处理器（如M1系列/M2）上启动会直接崩溃的bug。（by LionZXY [相关pr](https://github.com/GTNewHorizons/HydroEnergy/pull/18)）

### IFU (I will find you!)（寻矿魔杖）
* 版本号：1.9.4 → 1.9.5
* 使用Mod本地而非基于Mixin的Visual Prospecting集成。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/IFU/pull/12)）

### Infernal-Mobs
* 版本号：1.7.6-GTNH → 1.7.7-GTNH
* 防止`onAttack`在反射伤害中触发，以避免攻击怪物会导致玩家被反射造成凋零和反胃状态。（by Glease [相关pr](https://github.com/GTNewHorizons/Infernal-Mobs/pull/12)）

### KekzTech
* 版本号：0.6.15 → 0.6.16
* 修复了[最近的更改](https://github.com/GTNewHorizons/KekzTech/pull/43)导致进入存档崩溃的bug。（by miozune [相关pr](https://github.com/GTNewHorizons/KekzTech/pull/44)）
* 完全重做TFFT。（by DianeXD [相关pr1](https://github.com/GTNewHorizons/KekzTech/pull/45) [相关pr2](https://github.com/GTNewHorizons/KekzTech/pull/47)）详细内容如下：
  * 完善了多方块结构全息投影仪以及自动放置支持。
  * 修复了偶然出现的吞流体bug。
  * 修复了锁定输出仓流体不起作用的bug。
  * 修复了TFFT输入/输出仓不支持末影流体导管的bug。
  * 为TFFT加入了全种类玻璃支持。
  * 修改了相关主方块、TFFT机械方块、TFFT存储库方块的材质。
  * 加入了T6-T10的TFFT存储库方块。T1-T10 TFFT存储库方块的数据如下：
    * T1单方块储量1,000,000L，耗电1 EU/t，LV等级。
    * T2单方块储量4,000,000L，耗电2 EU/t，MV等级。
    * T3单方块储量16,000,000L，耗电5 EU/t，HV等级。
    * T4单方块储量64,000,000L，耗电14 EU/t，EV等级。
    * T5单方块储量256,000,000L，耗电42 EU/t，IV等级。
    * T6单方块储量2,048,000,000L，耗电132 EU/t，LuV等级。
    * T7单方块储量131,072,000,000L，耗电429 EU/t，UV等级。
    * T8单方块储量8,388,608,000,000L，耗电1430 EU/t，UEV等级。
    * T9单方块储量536,870,912,000,000L，耗电4862 EU/t，UMV等级。
    * T10单方块储量1,099,511,627,776,000,000L，耗电为0，UXV等级。
    * TFFT单种流体的储量仍然为存储库方块总储量的1/25。
  * TFFT总耗电为0的时候，可以不安装能源仓。
  * 用一种TFFT仓取代了此前的三种TFFT输入/输出仓。TFFT仓可使用末影流体导管直接输入/输出特定流体，也可以连上AE的ME流体存储总线，直接与ME网络交互。ME网络可以经由此读取每种最大long max量的流体，交互速率无限制。
  * 加入了TFFT相关新方块的配方，并且修改了全部原有的配方，价格总体上降低。该多方块结构仍然定位为EV+可以制造。
* 修复了兰波顿超级电容库相关的一个`NullPointerException`错误。（by spacebuilder2020 [相关pr](https://github.com/GTNewHorizons/KekzTech/pull/46)）
* 在检测结构前重置结构相关变量，修复了需要重新放置主方块才能更改结构的bug。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/KekzTech/pull/48)）

### KubaTech
* 版本号：0.5.11 → 0.6.5-pre
* 禁止工业屠宰场主方块任意旋转（by kuba6000 [相关pr](https://github.com/GTNewHorizons/KubaTech/pull/27)）
* 加入了巨型工业蜂箱/繁殖站（Industrial Apicultural Acclimatiser and Drone Domestication Station，简称Mega Apiary）多方块结构[^15]。（by kuba6000 [相关pr1](https://github.com/GTNewHorizons/KubaTech/pull/26) [相关pr2](https://github.com/GTNewHorizons/KubaTech/pull/28) [相关pr3](https://github.com/GTNewHorizons/KubaTech/pull/29) [相关pr4](https://github.com/GTNewHorizons/KubaTech/pull/31)）详细内容如下：
  * 定位为UV+机器。
  * 旨在为后期提供更高效率的蜜蜂生产方案。
  * 该机器有三种运行模式：输入模式、输出模式、工作模式。这三种模式的切换和用途与极限工业温室类似。
  * 工作模式分为两种子模式：普通(Normal)模式和蜂群(Swarmer)模式。
    * 普通模式下：是工业蜂箱的多方块升级版。每只蜂后消耗1A LuV。单次运行时间5秒。自带64倍加速、8倍产出升级、基因稳定升级，并且会模拟蜜蜂生长的最佳环境。可以提供蜂王浆提高产出，每个蜂王浆增加每次运行每只蜜蜂5%产出，最大加成200%。
    * 蜂群模式下：只能放入1只蜂后。会缓慢产出卑劣公主蜂。每次运行消耗100个蜂王浆。基础运行时间为1分钟，基础功率为1A IV，可以超频。
    * 部分蜜蜂只能使用巨型工业蜂箱产出蜂窝。详见GT5u更新部分。
* 将工业屠宰场对武器损耗的判定改为`hitEntity`，从而修复了部分实际使用时不会消耗耐久的武器在工业屠宰场中会消耗耐久的bug。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/KubaTech/pull/32)）
* 将Mod中mixin的部分改为调用GTNH Mixins。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/KubaTech/pull/33)）

[^15]: 这是一台机器的名字。

### LogisticsPipes（物流管道）
* 版本号：0.9.4.5.8-GTNH → 0.9.4.5.9-GTNH
* 修复了发送无效容器中的物品时，会导致`NullPointerException`崩溃的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/LogisticsPipes/pull/13)）

### MagicBees（魔法蜜蜂）
* 版本号：2.5.13-GTNH → 2.5.15-GTNH
* 加入蜜蜂效果能否加速的接口，但在之后的pr中又将其移至Forestry（林业）。相当于未更新实际功能。（by kuba6000 [相关pr1](https://github.com/GTNewHorizons/MagicBees/pull/14) [相关pr2](https://github.com/GTNewHorizons/MagicBees/pull/15)）

### MalisisDoors（更多门）
* 版本号：1.13.5-GTNH → 1.13.6-GTNH
* 加快了力场控制器的冷却速度。（by MadMan310 [相关pr1](https://github.com/GTNewHorizons/MalisisDoors/pull/4)）

### ModularUI
* 版本号：1.0.22（新Mod）
* 是1.12.2 ModularUI的向下移植版。ModularUI是一个GUI库，源于GTCE，可以简化创建GUI的过程。需要GTNHMixins做前置。更多详见GT5u等Mod的更新内容。

### MouseTweaks（鼠标手势）
* 版本号：2.4.5-GTNH → 2.4.6-GTNH
* 取消了开发环境以外的debug log。（by miozune [相关pr](https://github.com/GTNewHorizons/MouseTweaks/pull/2)）

### NEI Addons
* 版本号：1.12.19 → 1.12.22
* 加入了对蜜蜂愉快属性的描述。（by kuba6000 [相关pr1](https://github.com/GTNewHorizons/neiaddons/pull/4) [相关pr2](https://github.com/GTNewHorizons/neiaddons/pull/4)）
* 使NEIAddons不会为每个`AEBaseGui`的子类添加默认的handler。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/neiaddons/pull/6)）

### NewHorizonsCoreMod
* 版本号：1.9.83 → 1.9.109
* 在高阶电路配方中使用贴片电感替代小型线圈。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/424)）
* 加入了贴片电感、进阶贴片电感、光学贴片电感的合成配方。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/425)）
* 将蜂箱升级的合成配方移动至CoreMod中。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/429)）
* 加入了UIV和UMV单方块机器的合成配方。UIV的主要合成材料为下界之星线缆和黑钚；UMV的主要合成材料为量子锭线缆和时空。（by S4mpsa [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/430)）
* 使活化工具台无法获得玩家限定的特殊怪物掉落物。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/432)）
* 移除了配方中的所有0号电路板。（by miozune [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/431)）
* 移除了氧化锌的高炉配方，用焙烧锌取代。（by miozune [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/433)）
* 将蜂箱升级配方中的毒藤换成仙人掌。（by Runakai1 [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/434)）
* 加入了输入仓（ME）[^14]的配方。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/435)）
* 加入了使用UEV+超导制作超导线圈方块的配方。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/435)）
* 加入了使用电路组装机制造TPS卡的配方。（by POPlol333 [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/436)）
* 粗制超立方体的较低级DTPF配方需求线圈从海珀珍降为无尽。（by POPlol333 [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/438)）
* 将原钨钢线圈相关配方的材料都换为新的钛-铂-钒（TPV），以适配TPV线圈实装。[^13]（by Steelux [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/363)）
* 将AFB的三个配方合并，任意IV电路板都可以作为原料。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/441)）
* 缩短了热钽锭的烧制时间。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/440)）
* 将EIO双层电容配方改为使用钽螺栓，并且将银制电容配方需求的银螺栓减半。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/440)）
* 加入了UHV以上等级线缆二极管的配方。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/442)）
* 小幅更改了铝酸钠相关的配方。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/443)）
* 将ME流体存储组件合成ME流体存储元件的配方格雷化。（by OneEyeMaker [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/445)）
* 加入UMV变压器的合成配方。（by BlueWeabo [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/446)）
* 使用ModularUI重写了GUI。（by miozune [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/447)）
* 有full-hazmat-protection（危害防护）效果的装备现在可以保护玩家不受自定义效果（如手持污染物桶）的影响。（by miozune [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/448)）
* 修复了酿造室中用蜂蜜制造生物质配方需求无法合成的蜂蜜的问题。（by chochem [相关pr](https://github.com/GTNewHorizons/NewHorizonsCoreMod/pull/449)）

### NotEnoughEnergistics
* 版本号：1.3.21 → 1.3.23
* 使流体样板终端支持优先级调整模式。（即可以切换同矿辞物品）（by asdflj [相关pr](https://github.com/GTNewHorizons/NotEnoughEnergistics/pull/23)）

### NotEnoughItems
* 版本号：2.3.7-GTNH → 2.3.16-GTNH
* 在AE2压印器配方可用机器中加入了AE2 Stuff的高级压印器。（by miozune [相关pr](https://github.com/GTNewHorizons/NotEnoughItems/pull/306)）
* 删除了书签物品重排动画，禁用了相关功能，修复了从NEI书签将物品拖入样板终端时崩溃的bug。（by slprime [相关pr](https://github.com/GTNewHorizons/NotEnoughItems/pull/307)）
* 修复了用Ctrl+Shift+A收藏输出单种物品大于64个的配方时，无法正确收藏输出物品数量的bug。（by slprime [相关pr](https://github.com/GTNewHorizons/NotEnoughItems/pull/308)）
* 修复了大型硅岩反应堆和硅岩燃料精炼厂的NEI配方页面顶部灰条略微错位的问题。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/NotEnoughItems/pull/309)）
* 修复了使用NotEnoughResources Mod会导致`ArrayIndexOutofBoundException`崩溃的bug。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/NotEnoughItems/pull/312)）
* 添加了不优化GUI重叠计算的设置选项，使得某些GUI可以拖动到任意位置而不被NEI原有的GUI部分覆盖。（by miozune [相关pr](https://github.com/GTNewHorizons/NotEnoughItems/pull/314)）
* 只有物品列表真的被修改时，才会将其标记为`dirty`。修复了当安装GT6时，每次打开物品栏，NEI物品列表都会重载的bug。（by makamys [相关pr](https://github.com/GTNewHorizons/NotEnoughItems/pull/316)）
* 修复了单方块硅岩发电机NEI配方左侧的可用机器显示不准确的问题。（by miozune [相关pr](https://github.com/GTNewHorizons/NotEnoughItems/pull/318)）
* 将丹格特蒸馏塔加入了NEI蒸馏室配方左侧的可用机器中。（by miozune [相关pr](https://github.com/GTNewHorizons/NotEnoughItems/pull/319)）
* 修复了NEI部分配方页面（例如木工机）中，“？”图标被配方显示覆盖的bug。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/NotEnoughItems/pull/321)）

### NotEnoughIDs
* 版本号：1.4.3.4 → 1.4.4
* 新建GitHub仓库，加入了反编译的代码。（by boubou19）

### OpenComputers（开放式电脑）
* 版本号：1.8.0.0-GTNH-pre → 1.8.0.1-GTNH
* 加入了一次请求即可获取全部刻时间列表的方法：`getAllTickTimes`。（by boubou19 [相关pr](https://github.com/GTNewHorizons/OpenComputers/pull/82)）
* 更新build script，并且提高了`ScalaCompile`的RAM上限，以防止编译Mod时崩溃。（by eigenraven [相关pr](https://github.com/GTNewHorizons/OpenComputers/pull/83)）

### ProjectRed（红石计划）
* 版本号：4.7.7-GTNH → 4.7.9-GTNH
* 为脉冲发生器加入1 tick脉冲模式。（by greesyB [相关pr](https://github.com/GTNewHorizons/ProjectRed/pull/20)）
* 移除螺丝刀耐久度，但是因为GT5u后来加入了对红石计划螺丝刀的支持，所以又撤回了此更改，相当于未发生改动。（by greesyB [相关pr1](https://github.com/GTNewHorizons/ProjectRed/pull/21) [相关pr2](https://github.com/GTNewHorizons/ProjectRed/pull/22)）

### Railcraft（真实世界生成）
* 版本号：9.13.12 → 9.13.14
* 移除了英语语言文件(en_US.lang)开头的BOM（字节顺序标记）。（by Discreater [相关pr](https://github.com/GTNewHorizons/Railcraft/pull/31)）
* 修复了高级焦炉可以将木炭处理成焦煤的bug。（by Cleptomania [相关pr](https://github.com/GTNewHorizons/Railcraft/pull/32)）

### StorageDrawers（储物抽屉）
* 版本号：1.11.18-GTNH → 1.11.19-GTNH
* 修复了储物抽屉读取库存的方法与其他Mod无法兼容的问题。这个问题会导致T键寻找物品对抽屉失效、懒人厨房无法读取抽屉物品等等。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/StorageDrawers/pull/18)）

### StructureCompat
* 版本号：0.2.0 → 0.3.0
* 修复了与Hodgepodge的兼容性问题。（by Glease [相关commit](https://github.com/GTNewHorizons/StructureCompat/commit/717fc37ce388cbf8e20814faff3d112d979dc9b0)）

### StructureLib
* 版本号：未定
* 加入了Debug结构打印机。比TecTech的同名机器功能更完善。（by matt-159 [相关pr](https://github.com/GTNewHorizons/StructureLib/pull/17)）

### TC4Tweaks
* 版本号：1.4.18 → 1.4.19-GTNH
* 修复了`hashCode`的生成问题。（by Glease [相关commit](https://github.com/GTNewHorizons/TC4Tweaks/commit/3dff3d97e1721cb0405f96a418d09d7a6a8b616b)）
* 不再给假玩家增加扭曲值，以防止崩溃。（by Glease [相关commit](https://github.com/GTNewHorizons/TC4Tweaks/commit/fbb2fd8d57a16d071e957d2053a709720b58cd00)）
* 优化了`canNodeBeSeen`，解决了潜在的突发高延迟问题。（by Glease [相关commit](https://github.com/GTNewHorizons/TC4Tweaks/commit/25e776c0d0486406241d81d42f548ca0206225f9)）
* 允许使用滚轮滚动研究页面。（by Glease [相关commit1](https://github.com/GTNewHorizons/TC4Tweaks/commit/8bde2dfcf45d9c2b508223494d75fc89a1794bbd) [相关commit2](https://github.com/GTNewHorizons/TC4Tweaks/commit/25e776c0d0486406241d81d42f548ca0206225f9)）

### TCNEIAdditions
* 版本号：1.1.1.5 → 1.1.1.7
* 使设置选项能够本地化。（by miozune [相关pr](https://github.com/GTNewHorizons/TCNEIAdditions/pull/15)）
* 将鼠标移动至NEI神秘时代相关配方页面“研究名称”(Research name)词条上，会显示解锁该研究所需的所有前置条件和完成情况。（by iouter [相关pr](https://github.com/GTNewHorizons/TCNEIAdditions/pull/16)）

### TecTech
* 版本号：5.0.42 → 5.0.52
* 将高阶电路板制造配方中的小型线圈换成贴片电感。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/TecTech/pull/105)）
* 修复了末影流体覆盖板无法正确处理存储信息导致不断发送日志的bug。（by Glease [相关pr](https://github.com/GTNewHorizons/TecTech/pull/107)）
* 对数据访问仓使用了新的API，解决了延迟问题。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/TecTech/pull/108)）
* 移除了UHV部分部件的装配线配方需求的润滑油。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/TecTech/pull/110)）
* 修复了末影流体覆盖板可以跨存档传输流体的bug。（by minecraft7771 [相关pr1](https://github.com/GTNewHorizons/TecTech/pull/112) [相关pr2](https://github.com/GTNewHorizons/TecTech/pull/113)）
* 加入了完整方块版本的光缆、激光真空管、量子隧道。（by minecraft7771 [相关pr](https://github.com/GTNewHorizons/TecTech/pull/111)）
* 使用ModularUI重写了GUI。（by miozune [相关pr](https://github.com/GTNewHorizons/TecTech/pull/114)）
* 加入了UMV多安动力仓/能源仓和UIV/UMV激光仓的合成配方。（by BlueWeabo [相关pr](https://github.com/GTNewHorizons/TecTech/pull/115)）

[^16]: 参见NewHorizonsCoreMod更新内容。

### ThaumicEnergistics（神秘能源）
* 版本号：1.3.19-GTNH → 1.3.21-GTNH
* 修复了与源质冷凝器的交互会导致物品复制的bug。[^17]（by repo-alt [相关pr](https://github.com/GTNewHorizons/ThaumicEnergistics/pull/24)）
* 为源质存储元件加入了过滤源质种类信息的tooltip。（by dipo33 [相关pr](https://github.com/GTNewHorizons/ThaumicEnergistics/pull/25)）
* 允许多个奥术装配室并行处理同一个配方。（by greesyB [相关pr](https://github.com/GTNewHorizons/ThaumicEnergistics/pull/27)）

[^17]: 参见Applied Energistics 2 Unofficial（AE2）更新内容。

### ThaumicHorizons（神秘视界）
* 版本号：1.2.1.7 → 1.2.1.8
* 移除了`getStackTrace`检测，以修复服务器卡顿的问题。（by pulsemageadvocate [相关pr](https://github.com/GTNewHorizons/ThaumicHorizons/pull/37)）

### Thaumic Insurgence（神秘革命）
* 版本号：0.0.6 → 0.0.8
* 修正了英语语言文件(en_US.lang)的文本错误。(by Alastors [相关commit](https://github.com/GTNewHorizons/thaumicinsurgence/commit/3f4f5ed408dc6864fdab07e916b0af9e3bd20c5a))
* 精简了注魔截流者(infusion inteceptor)的代码，并且buff了注魔截流者，使其能够1 tick输出所有源质。（by greesyB [相关pr](https://github.com/GTNewHorizons/thaumicinsurgence/pull/12)）

### TinkersConstruct（匠魂）
* 版本号：1.9.6-GTNH → 1.9.7-GTNH
* 修复了粘土铸件覆盖了铝黄铜铸件的注册名的问题。（by DrParadox7 [相关pr](https://github.com/GTNewHorizons/TinkersConstruct/pull/58)）
* 加入了熔融石英的材质。（by DrParadox7 [相关pr](https://github.com/GTNewHorizons/TinkersConstruct/pull/58)）

### TinkersGregworks
* 暂时未发布新版本。
* 修复了匠魂器具的本地化问题。（by iouter [相关pr])(https://github.com/GTNewHorizons/TinkersGregworks/pull/10)）

### TX Loader
* 版本号：1.1（新Mod）
* 该Mod会创建两个特殊的目录，可以用于加载资源。
  * `./config/txloader/load/`与资源包的作用相同。
  * `./config/txloader/forceload/`中的文件可以覆盖Minecraft `assets`对应位置的文件。

### VisualProspecting
* 版本号：1.0.34 → 1.0.36
* 移除了IFU相关的mixin，改用本地集成。（by mitchej123 [相关pr](https://github.com/GTNewHorizons/VisualProspecting/pull/22)）
* 更新了build script，并应用了GTNHMixins。（by dipo33 [相关pr](https://github.com/GTNewHorizons/VisualProspecting/pull/23)）

## 任务书及配置文件更新
* 大量修正任务书内容。（by chochem & Steelux8 [相关pr1](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11653) [相关pr2](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11672) [相关pr3](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11722) [相关pr4](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11741) [相关pr5](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11787) [相关pr6](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11852) [相关pr7](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11878)）
* 增加了工业锻造锤、工业3D打印机、工业碎石机的任务。（by chochem [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11852)）
* 将蜂箱升级配方从配置文件中移除，移至NewHorizonsCoreMod中。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11588)）
* 大量更改路由管道(Logistics Pipe)的配方，主要是降低造价。（by Glease & Steelux8 [相关pr1](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11597) [相关pr2](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11642) [相关pr3](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11643)）
* 更新了任务书中升级框架的id，因为该物品已从Gendustry（基因工业）移动至GT5u。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11600)）
* 将AE2压印器的配方移动至配置文件脚本中。（by miozune [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11635)）
* 加入了使用石英岩粉制造EIO石英玻璃的配方。（by Dream-Master [相关commit1](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/commit/53918e9688c7e5ddffbabb98b7b10c3715ed89fa) [相关commit2](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/commit/e7d432a10c37f13b29d68ac2cc398f8e49febdd0) [相关commit3](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/commit/89b3e59f6014b6d0e9e715020d47e4314bce2260)）
* 将蜂窝的矿辞配置移至GT5u。（by kuba6000 [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11660)）
* 修正了关于水域菜园的一个加载界面提示。（by miozune [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11659)）
* 在自述文件中加入了discord频道的链接。（by boubou19 [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11690)）
* 将脚本部分改为I18N本地化。（by iouter [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11693)）
* 修正了`motd`值拼写错误。（by ihatewindows [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11707)）
* 临时在脚本中加入了EnderIO电容的配方。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11742)）
* 修复了ingameinfo（IGI，游戏信息显示）显示错误的群系温度和适度的问题。（by iouter [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11745)）
* 降低了LuV/ZPM/UV太阳能覆盖板的造价，主要降低了需求的电路板等级和超导数量。（by Tyrantgtnh [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11777)）
* 禁用了碲/钡/镧/铈/镨/钆/镝/钬/铒/铥/镱粒的炼金复制配方。（by GlodBlock [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11802)）
* 将部分物品配方中的混沌核心改为觉醒核心，因为混沌核心现在需要UMV材料制造。（by GDCloudStrike [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11800)）
* 在GregTech.cfg中加入了EV/IV燃气轮机的相关内容。（by Dream-Master [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11827)）
* 更新了defaultserverlist.json，加入了一个新的服务器。（by superhealing & glowredman [相关pr1](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11851) [相关pr2](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11853)）
* 修改了部分ProjectRed（红石计划）的配方，以保持配方一致性。（by miozune [相关pr](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack/pull/11889)）



> 参考文本：
> * All pull requests and commits from [GTNewHorizons repositories](https://github.com/GTNewHorizons)
[![中文](https://img.shields.io/badge/语言-中文-red)](README.zh.md)
[![English](https://img.shields.io/badge/lang-English-blue)](README.md)

# Steadfast – Minecraft Java 版光影包

Steadfast 是一款极其流畅且毫不突兀的光影包，在细节上精益求精。它既赏心悦目，又不会给电脑带来沉重负担，能显著提升 Minecraft 的图形质量和真实感，同时丝毫不影响游戏本身的游玩体验。

Steadfast 是由 coderbot 开发的免费开源软件，可从以下地址下载：  
[https://modrinth.com/shader/steadfast-shaders](https://modrinth.com/shader/steadfast-shaders)（Modrinth）、  
[https://www.curseforge.com/minecraft/shaders/steadfast](https://www.curseforge.com/minecraft/shaders/steadfast)（CurseForge）或  
[https://github.com/coderbot16/Steadfast](https://github.com/coderbot16/Steadfast)（GitHub）。  
任何人都可以根据 GNU 通用公共许可证第 3 版的规定修改和分发它。

## 究竟有多快？

即使在 5 年以上的中端笔记本电脑上，Steadfast 也能流畅运行。默认的“高”配置在大多数能运行 Minecraft 的电脑上都能稳定达到 60+ FPS。在配备高端独立显卡的电脑上，Steadfast 更是飞速运行，即使是“高”配置也能轻松达到 250–500 FPS。如果选用更低配置，甚至在树莓派上也能勉强游玩！

Steadfast 专为移动/集成显卡硬件设计，对显存带宽要求极低，只需中等图形算力即可。

## 功能特性

- 半写实的大气效果，包含高品质的天空和雾气
- 太阳和月亮投射的实时阴影
- 随风摇曳的植被，并具有次表面散射效果
- 精心调校的光照，营造出明亮阳光、较暗夜晚和室内的错觉，但不会过度改变亮度或对比度，也没有令人不适的自动曝光效果
- 太阳和月亮产生的近似光柱（“上帝光”）
- 细节极为丰富的水波，具有真实的视觉深度、反射、折射，以及基于水深度的逼真吸收效果
- 水和冰可以反射屏幕上可见的任何物体
- 阳光和月光在水下表面投射出明亮的焦散效果
- 风吹拂的高空卷云，同时支持 Minecraft 原版方块云
- 通过 Minecraft 内置的平滑光照实现环境光遮蔽
- 与 Distant Horizons 和 Voxy 模组集成，可提供极远渲染距离且无明显性能损失
- 广泛兼容其他模组和整合包，包括支持 Create 等模组中的高性能渲染路径（通过 Colorwheel 附加模组）

## 平台兼容性

Steadfast 支持以下硬件和基础平台：

- NVIDIA、AMD 和 Intel 显卡
- macOS，包括 Apple Silicon
- Linux，包括通过开源 Mesa 图形驱动支持的大多数硬件，如树莓派和 Steam Deck
- Minecraft 1.18.2 及以上版本，使用 Iris 光影模组（Iris 1.5 或更新版本）
- Minecraft 1.7.10，使用 Angelica 光影模组

## 当前限制

Steadfast 目前存在一些值得注意的限制，我希望在未来解决：

- 目前不支持任何版本的 OptiFine。
  - Steadfast 将大量计算转移到 CPU，但实现此功能所用的特性（“自定义 uniform”）在 OptiFine 和 Iris 中的工作机制有所不同，因此移植需要大量工作。
- 除主世界外，不支持任何其他维度，包括对下界和末地缺乏精细调校的支持。
  - 要支持其他维度，基本上需要为光影创建新的视觉风格，这可能需要数月时间才能做好。
  - 当前下界/末地的表现完全可以游玩，并且没有通常光影包缺乏维度支持时可能出现的严重 Bug，但优化和调校未达到主世界那样的品质。换句话说，它基本上只是碰巧能运行。
- 目前不支持彩色光照。
  - 要在高性能和高品质下实现这一点非常困难，但我正在研究，幸运的是社区中已有先例。

## 支持政策

- 我致力于在软件中保持高标准的质量，Beta 测试阶段的目标是发现并修复任何 Bug、风格问题和类似缺陷。
- 请尽量避免重复提交 Bug 报告，并自行判断 Bug 是出现在 Steadfast、Iris、Minecraft、其他模组还是您的显卡驱动/系统中，但如果您不确定，也欢迎提交报告。
- 我们无法帮助您在运行 Android 或 iOS 的手机和移动设备上（即使使用 PojavLauncher 等软件）让 Steadfast 正常工作，因为图形驱动和兼容层普遍存在正确性和 Bug 问题。

## 致谢

- Steadfast 在视觉上深受 Sonic Ether 的 Unbelievable Shaders（SEUS，特别是 SEUS Renewed）以及 Chocapic13 的部分光影作品启发。SEUS 是一款出色的光影包，希望您会喜欢这个具有类似视觉风格的实现！
- Steadfast 离不开 Iris 光影加载器，尤其是 IMS212 的持续开发和维护，使得 Steadfast 能够在许多 Minecraft 版本上轻松运行，而无需在 Steadfast 这边费太多功夫。
- 我还要感谢我的专注测试人员，他们在 Steadfast 开发过程中帮助发现和修复了许多 Bug 和问题！

# Minecraft 竞速任务挑战赛</br>—— 蛋白后宫同款修改版
***Made by* JupiterLyr**

## 游戏版本
Minecraft Java 版 `1.19.x`

## 所需 Mod
自定义局域网联机 `Lan Server Properties`：用于配置联机。

## 数据包打包方法
将 `data` 文件夹和 `pack.mcmeta` 文件选中，直接压缩为 ZIP 格式。注意，打开压缩包应该直接看到这二者，不能嵌套在子文件夹内

## 数据包使用方法
1. 将文件打压缩包，格式为 `*.zip`。
2. 将文件放置于 `datapacks` 文件夹中，并移动到存档地图文件夹中；或者在创建新地图时，将这个压缩包拖入游戏窗口。
3. 在游戏中，使用 `/reload` 指令重载数据包。
4. 调整到**创造模式**，打开物品栏，跟随指引设置游戏并开始。

## 开源文件说明
- 文件 `pack.mcmeta` 是包描述文件，更新时建议同步修改其内版本号。
- 文件夹 `functions` 下的 `*.mcfuntion` 文件都是游戏内容的配置文件，其内的 `tast` 和 `new_tast` 中存放了可能随机到的任务。修改任务时，要同时修改 `getscore.mcfunction` 和 `load.mcfunction` 中的计分板名称及游戏检测事件。
- 文件夹 `functions` 下的 `rand_task_easy.mcfunction`、 `rand_task_normal.mcfunction`、 `rand_task_hard.mcfunction` 文件，分别设定了简单、普通、困难难度下的随机数与随机任务的映射关系。
- 文件夹 `loot_tables` 中的 `*.json` 文件设定了不同随机方式的随机数上下限。注意，随机数上下限应与映射的涵盖范围一致！

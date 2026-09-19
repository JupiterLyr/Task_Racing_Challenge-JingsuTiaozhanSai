# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).</br>

---

## [1.1.6] —— 2026-09-19 15:00
### Changed
- 调整了部分可能分配到的随机任务
### Fixed
- 规范化了部分文件的命名
- 修复了 `creative_inventory_ui.mcfunction` 和 `inventory_ui.mcfunction` 的 `bee_spawn_egg` NBT标签中 `EntityTag` 缺失 `id` 字段的问题
- `load.mcfuntion` 中 `ac_rand:install` 未定义，现已去除

## [1.1.5.11808] —— 2025-08-12 18:00
### Fixed
- 修复了个别任务的错误文字显示，完善了工程部分文件的规范性

## [1.1.5] —— 2025-07-02 23:30
累积更新 v1.1.3 ~ v1.1.5
### Changed
- 重写了 `ingame.mcfunction` 的 `#tasks` 处的新任务获取方式，规范了三种难度等级的随机任务生成方法
### Fixed
- 修复了计分板不正常显示的Bug，以及个别不正确的函数配置
- 修复了个别任务完成的判定机制（识别个数等）

## [1.1.2] —— 2025-07-02 20:30
### Changed
- 修改了 `tast` 中的部分任务，暂时屏蔽了 `new_tast` 中的部分高难度任务

| 文件 | 原任务 | 修改任务 | 难度 |
| :---: | :---: | :---: | :---: |
| `tast/27.mcfunction` | 制作一把弩 | 制作一把弓 | **↓** |
| `tast/28.mcfunction` | 制作一个遮光玻璃 | 制作红石火把 | **↓↓↓** |
| `tast/29.mcfunction` | 制作一个望远镜 | 制作火把 | **↓↓↓** |
| `tast/38.mcfunction` | 制作一个皮革马铠 | 制作一块萤石 | **↑↑** |
| `tast/62.mcfunction` | 丢掉一把三叉戟 | 丢掉一把金稿 | **↓↓** |
| `tast/64.mcfunction` | 制作一个阳光感测器 | 制作白桦木台阶 | **↓↓↓** |

- 修改了上述任务对应的 `getscore.mcfunction` 的任务重置栏目
- 修改了上述任务对应的 `load.mcfunction` 的计分板设置栏目，其内容在 `#task's scoreboard` 下方
- 将 `loot_tables` 文件夹中 `random_normal.json` 文件的随机数最大取值调整为 `64`，扩增了“普通”难度的随机数取值范围，并在 `rand_task_normal.mcfunction` 中调整了随机数到任务的映射关系
- 将游戏设置 `settings.mcfunction` 中 `DayLight command matches 2` 的指令调整为从早晨开始而非正午

## [1.0.7]
### Changed
修改了部分任务的文字描述

## [1.0.6]
接收的初始版本
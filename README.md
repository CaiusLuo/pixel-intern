# pixel-intern · 像素实习生

戴银灰方框眼镜、背斜挎包的像素实习生，陪你一起完成 Codex 任务。

Pixel Intern is an AI-assisted pixel-art companion with silver-gray glasses and a crossbody satchel.

[![Download on Petdex](https://img.shields.io/badge/Petdex-下载像素实习生-6366f1)](https://assets.petdex.dev/pets/pixel-intern-94afbffaae0e/zip.zip)
[![GitHub release](https://img.shields.io/github/v/release/CaiusLuo/pixel-intern)](https://github.com/CaiusLuo/pixel-intern/releases/latest)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## 快捷下载

- **[Petdex 直接下载 ZIP](https://assets.petdex.dev/pets/pixel-intern-94afbffaae0e/zip.zip)**：与 Petdex 的 “Download ZIP” 按钮使用同一下载地址。
- [Petdex 宠物详情页](https://petdex.dev/pets/pixel-intern)
- **[GitHub 最新宠物包 ZIP](https://github.com/CaiusLuo/pixel-intern/releases/latest/download/pixel-intern.zip)**：解压后得到 `pet.json` 和 `spritesheet.webp`。
- [直接下载精灵图](https://github.com/CaiusLuo/pixel-intern/releases/latest/download/spritesheet.webp)

### 一条命令安装

```bash
npx petdex install pixel-intern
```

Petdex 投稿目前正在审核，命令安装和公开详情页可能需审核通过后才能使用；可以先通过上面的 ZIP 直链下载。

## 动画预览

| 待机 | 向右跑 | 向左跑 |
| --- | --- | --- |
| ![待机](previews/idle.gif) | ![向右跑](previews/running-right.gif) | ![向左跑](previews/running-left.gif) |
| 挥手 | 跳跃 | 失败 |
| ![挥手](previews/waving.gif) | ![跳跃](previews/jumping.gif) | ![失败](previews/failed.gif) |
| 等待确认 | 执行任务 | 检查 |
| ![等待确认](previews/waiting.gif) | ![执行任务](previews/running.gif) | ![检查](previews/review.gif) |

### 16 个看向方向

![16 个看向方向](previews/look-directions.png)

## 安装

1. 下载并解压 `pixel-intern.zip`。
2. 将 `pet.json` 和 `spritesheet.webp` 放入 `~/.codex/pets/pixel-intern/`（macOS / Linux）。已有同名目录时先备份。
3. 在支持自定义宠物的 Codex 版本中刷新宠物列表或重启应用，然后选择“像素实习生”。

ZIP 内只有两个根目录文件，无须安装依赖或运行脚本。

## 当前版本

本仓库提供最终 **V2 优化版**：九种动画状态，加上十六个看向方向。保留初版动画，新增方向帧，修正上下左右方向，并处理边缘色溢。

| 项目 | 值 |
| --- | --- |
| 宠物 ID | `pixel-intern` |
| 图集布局版本 | `spriteVersionNumber: 2` |
| 格式 | 透明 RGBA WebP |
| 尺寸 | 1536 × 2288 |
| 网格 | 8 列 × 11 行 |
| 单帧尺寸 | 192 × 208 |

`v1.0.0` 是仓库的首次公开发布版本；`spriteVersionNumber: 2` 是图集布局版本，两者含义不同。

发布前已核对本地安装包、最终优化包和 Petdex 下载包，精灵图 SHA-256 一致：

```text
07da9082ef4cc43e7b98980f6acccb14c44e7d194c28e19a87d3307c60d28201
```

已有制作检查记录通过图集、透明度和方向检查。部分动作仍使用较明显的逐帧切换，少数中间方向的朝向提示较轻微。

## 使用与署名

按 [MIT 许可证](LICENSE) 开放使用、修改和分发，允许商业使用；分发时保留许可证和版权声明。

这是 AI 辅助制作的自定义像素角色。发布者：[@CaiusLuo](https://github.com/CaiusLuo)。项目与 OpenAI、Codex 和 Petdex 无官方关联。详见 [制作说明](CREDITS.md) 和 [版本记录](CHANGELOG.md)。

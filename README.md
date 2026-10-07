# 音乐播放器穿插

作者：**理智画** · [GitHub @liuzihe849-png](https://github.com/liuzihe849-png)

使用 `$music-player-photo-weave`，把用户自己的照片制作成对应视觉效果。包内已附原创参考样片，执行时需读取参考与规则；用户无需重新提供同一张风格参考。

![原创参考样片](assets/reference-original.png)

## 安装与使用

将本仓库整个文件夹放到你的 Skills 目录，保留 `SKILL.md`、`references/`、`assets/` 及存在的 `scripts/`，然后在新对话调用：

```text
$music-player-photo-weave
上传我的原照片；提供：歌名、歌手
```

也可让 Skill Installer 从 https://github.com/liuzihe849-png/music-player-photo-weave 安装。运行所需图像工具必须在用户环境可用；本仓库不是独立生图模型或免费 API。

## 当前状态

本次发布为预览版本。修正过的播放器样片；新的照片需重新选择遮挡区域，右臂后置不是所有照片的固定要求。

先前完成过独立新对话单图测试，但本次替换原创参考后的版本尚未完成重新下载视觉验收，不保证每次同图同像素。验收以实际成图及用户审核为准。

## 署名与素材

Skill 设计、流程整理和样片制作：**理智画**。参考样片是创作结果，不是新用户的身份来源。外网博主原始照片、私人对话、原始输入照片和临时文件未放入本次发布包。素材说明见 [CREDITS.md](CREDITS.md)，代码与文档许可见 [LICENSE](LICENSE)。

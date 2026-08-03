# Soviet Jokes Asset Library

用于“苏联笑话系列”短视频的公开人物与场景参考素材库。公开托管的目的，是让 HFSY 等生成 API 能通过 HTTPS URL 读取参考图。

## 目录结构

- `characters/character-NNN/main.*`：人物主图
- `characters/character-NNN/full.*`：人物三视图
- `scenes/scene-NNN/main.*`：场景主图
- `scenes/scene-NNN/full.*`：场景多视图
- `references/`：公开的画风与分镜布局参考，不代表具体人物或剧情素材
- `asset_catalog.json`：中文名称、本地原始相对路径、尺寸和 Raw URL 的机器可读索引

当前共有 29 个人物、25 个场景和 107 张图片。人物“年轻工人”目前只有主图，尚缺三视图；其余人物和场景均已配对。

## API 引用

请从 `asset_catalog.json` 中读取 `main.raw_url` 或 `supplement.raw_url`。例如：

```text
https://raw.githubusercontent.com/zycui211382-a11y/sovietjokes-assets/main/characters/character-001/main.jpg
```

这些链接直接返回图片内容，可放入 HFSY 视频或图像接口的参考图片数组。调用第三方生成 API 可能产生费用，素材下载本身不触发模型调用。

## 权利说明

本仓库未授予开源或再分发许可。素材权利归仓库所有者保留。

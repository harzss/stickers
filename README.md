# Claire Stickers

Claire's Parlor 的表情包创作仓库。这里记录「像素奶茶小猫」和「低清奶茶小猫」两条风格线的设计语言、提示词、场景库和部分成品素材。

## Packs

- `packs/pixel-mini-cat/`：微型像素表情，透明背景，小动作、小道具，适合日常聊天和亲密互动。
- `packs/low-res-meme-cat/`：低清猫图二创、微信群聊梗图、JPEG 糊图、精神状态抽象。

## Repository Structure

```text
stickers/
├── README.md
├── LICENSE
├── assets/
│   └── source-cat/             # 自有小猫参考照片
└── packs/
    ├── low-res-meme-cat/
    │   ├── README.md
    │   ├── docs/               # 设计语言、提示词、场景库
    │   └── stickers/           # 成品或待生成素材
    └── pixel-mini-cat/
        ├── README.md
        ├── docs/               # 设计语言、提示词、场景库、赞赏图提示词
        ├── previews/           # 预览图 / sheet
        └── stickers/           # 分批表情图与平台素材
```

本地草稿、外部参考图、生成临时图放在 `.workbench/` 或 `reference/`，这些目录被 `.gitignore` 忽略，不进入公开仓库。

## 使用方式

1. 进入 `packs/<pack-name>/`。
2. 阅读 `docs/design.md`，确认角色、画面和审美边界。
3. 从 `docs/scenes.md` 选择一个场景，放进 `docs/prompt.md` 的模板。
4. 生成后把最终可公开的成品放进 `stickers/`。

## License

本仓库统一使用 Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)，见 `LICENSE`。

你可以非商业分享、学习和改编这里的文档、提示词、场景描述与表情素材。商业使用、售卖、上架表情包或用于商业模型训练前，请先获得授权。

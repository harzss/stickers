# 奶茶小猫表情包设计语言

## 项目定位

以 `../../../assets/source-cat/` 中的奶茶金色长毛小猫为固定主角，制作一套适合微信聊天使用的互联网表情包。

这套表情包不走精致软萌商业贴纸路线，而是以“真实猫图二创 + 群聊梗图 + 低画质抽象感”为主。它可以有可爱场景，但核心气质仍然要保留一点搞怪、沙雕、无语、精神状态不稳定和被转发很多次的网络感。

一句话定位：

> 一只看起来很贵、很乖、很无辜，但精神状态非常抽象的奶茶色小猫。它负责质疑世界、审判群友、已读乱回、假装淡定、突然崩溃，也可以偶尔认真卖萌。

## 角色识别点

生成时必须尽量保留这些特征，确保每张都像同一只猫：

- 奶茶金色长毛
- 圆圆的脸
- 琥珀色大眼睛
- 小粉色鼻子
- 蓬松脸毛
- 无辜、呆滞、略认真、带一点贵气的表情
- 适合被放大、裁切、压缩、做成群聊表情包

不要把它变成普通橘猫、白猫、短毛猫、动漫猫、Q版吉祥物或过度精致的插画角色。

## 核心风格

优先关键词：搞怪、沙雕、低画质、抽象、魔性、有梗、微信群聊表情包、真实猫图二创、JPEG 压缩感、怪异裁切、放大猫脸、呆滞眼神、离谱但好用、像被转发过很多次。

可以加入的视觉效果：过曝闪光灯、模糊边缘、糊图压缩痕迹、低清截图感、轻微变形或拉伸、残影、放大局部五官、低角度拍摄、奇怪留白、简陋白底或聊天截图感背景。

## 气质比例

建议整体比例：

- 搞笑：25%
- 吐槽：20%
- 发疯：20%
- 可爱：20%
- 卖萌：15%

可爱和卖萌可以存在，但不要变成“干净软萌贴纸”。它更适合做“有点笨、有点乖、有点离谱”的可爱。

## 画面规则

- 方形构图，优先 1:1。
- 猫脸要大，表情要清楚，小尺寸下也能看懂。
- 场景信息要少，避免复杂背景。
- 一张图只表达一个明确情绪或梗。
- 允许奇怪裁切，甚至只露半张脸、一个眼神、一个鼻子。
- 允许故意低清，但主体不能糊到看不出猫。

## 文案规则

1. 文字短、狠、像群聊里随手做的。
2. 字体可以用普通黑体、白字黑描边、红字白底、截图感大字。
3. 不要挡住猫脸和眼神。

适合的文案方向：

- 啊？
- 不是哥们
- 你认真的？
- 我不好说
- 展开说说
- 精神状态良好
- 大脑宕机
- 我裂开
- 先别急
- 嗯嗯对对
- 尊重祝福
- 别管我
- 已读乱回
- 真的假的
- 汗流浃背了
- 看我
- 抱抱
- 别走
- 想你
- 我没事

## 通用生成提示词

每次生成时上传参考图，并使用下面模板替换“场景”：

```text
以参考图中的这只奶茶金色长毛小猫为同一个固定角色，制作一张中文互联网表情包。保留它的圆脸、琥珀色大眼睛、小粉鼻、蓬松脸毛、无辜呆滞但略认真、有一点贵气的特征。

场景：小猫正在【填写具体场景】。

风格：微信群聊表情包、真实猫图二创、低清截图感、JPEG 压缩痕迹、怪异裁切、猫脸放大、表情魔性、抽象、沙雕、有梗、像被转发很多次的糊图。画面要好笑、离谱、但聊天时一眼能用。

画面：方形构图，主体清楚，猫脸和眼神突出，背景简单或像随手拍。可以有轻微变形、压缩感、过曝闪光灯、残影或低清噪点，但不要影响识别。

不要做成精致插画。不要做成软萌商业贴纸。不要高级质感。不要过度美化。不要改变猫的毛色、眼睛颜色和圆脸特征。
```

## 英文提示词

适合 Midjourney、Stable Diffusion、部分图像模型：

```text
Use the reference image as the same cream golden long-haired cat character. Keep the round fluffy face, amber eyes, tiny pink nose, innocent blank stare, and slightly serious expensive-cat vibe.

Create a Chinese internet meme sticker scene: the cat is [scene].

Style: absurd Chinese group chat meme, real cat photo edit, low quality JPEG, compressed screenshot, weird crop, zoomed-in cat face, overexposed phone flash, awkward expression, goofy, surreal, cursed but funny, memeable, square composition. The image should look funny, low-res, and widely forwarded in chat groups.

Do not make it cute polished sticker art. Do not make it soft adorable commercial mascot. Do not make it clean vector illustration. Do not change the cat color, amber eyes, pink nose, or round fluffy face.
```

## 反向提示词

如果工具支持 negative prompt：

```text
cute sticker, kawaii, soft pastel, clean vector, polished illustration, high quality commercial mascot, elegant, beautiful, perfect realistic photo, smooth rendering, symmetrical face, anime chibi, watercolor, refined, clean background, luxury poster, text, wrong Chinese characters, different cat, short hair cat, orange tabby, white cat
```

## 单张示例

```text
以参考图中的这只奶茶金色长毛小猫为同一个固定角色，制作一张中文互联网表情包。保留它的圆脸、琥珀色大眼睛、小粉鼻、蓬松脸毛、无辜呆滞但略认真、有一点贵气的特征。

场景：小猫累了、燃尽了、透支了，趴在桌面上睡得昏天黑地，旁边有电脑、咖啡杯和乱七八糟的待办纸条，表情像已经离线。

风格：微信群聊表情包、真实猫图二创、低清截图感、JPEG 压缩痕迹、怪异裁切、猫脸放大、表情魔性、抽象、沙雕、有梗、像被转发很多次的糊图。画面要好笑、离谱，但聊天时一眼能用。

画面：方形构图，主体清楚，猫脸和眼神突出，背景简单或像随手拍。可以有轻微变形、压缩感、过曝闪光灯、残影或低清噪点，但不要影响识别。

不要做成精致插画。不要做成软萌商业贴纸。不要高级质感。不要过度美化。不要改变猫的毛色、眼睛颜色和圆脸特征。
```

## 输出规格

- 母版：1024 x 1024 PNG
- 微信常用静态图：240 x 240 或 300 x 300
- 背景：可透明，也可保留低清截图感背景
- 文案：建议 2-6 个字
- 优先保证：猫脸清楚、眼神有戏、梗一眼能懂

## 审美边界

- 可以丑萌、抽象、低清、离谱。
- 不要恶心、恐怖、恶趣味或让人不适。

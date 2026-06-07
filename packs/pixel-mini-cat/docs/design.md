# 像素奶茶小猫表情包设计语言

## 系列定位

这条线和 `../../low-res-meme-cat/docs/design.md` 里的“低清猫图二创”分开做。

原主包是：真实猫图、群聊梗图、JPEG 糊图、精神状态抽象。

像素版是：参考图那种微型像素表情 sheet，带一点红白机 / 掌机年代感，透明背景、小动作、小道具、适合情侣和日常聊天。

这条线的第一优先级是**微型像素表情感**，不是照片相似度，也不是大号现代像素贴纸。`../../../assets/source-cat/` 只用来锚定“浅奶茶小鹿色、圆脸、粉鼻子、呆呆的气质”，不要追求真实猫毛、真实光影、真实五官或毛发纹理。

暂定系列名：**像素奶茶小猫**。

一句话定位：

> 一只像从早期掌机 / 老网页像素表情包里跳出来的浅奶茶小鹿色小猫，用几个硬像素完成贴贴、想你、收到、晚安和一点点发呆。

## 参考图方向：微型像素表情

这套要像参考图里的小角色：黑底预览、角色很小、动作靠剪影和小道具表达。它可以带一点红白机 / 掌机年代感，但不是硬核战斗游戏 sprite，也不是现代高清像素贴纸。

这批参考图真正好看的地方不是“像素很多”，而是**元素极少但情绪明确**：两颗点眼、一个鼻点、短短的手脚，再配一个很清楚的小道具。画面不要讲故事，只做一个能立刻读懂的小反应。

关键词：

- `tiny pixel emoji`
- `pixel emoji sheet`
- `Tamagotchi-style sprite`
- `old web pixel icon`
- `Japanese deco-mail pixel emoji`
- `16x16 or 24x24 mini sprite`
- `black preview background, transparent final PNG`
- `limited 4-color palette`
- `clean dark outline`
- `no anti-aliasing`
- `no gradients`

视觉判断：把图缩到 `24 x 24` 仍然像一个小表情图标，而不是一张被缩小的可爱插画。

## 简单元素公式

每张都按这个公式做：

```text
1 个微型角色 / 2 个贴贴角色 + 1 个简单道具或符号 + 1 个明确情绪
```

适合的道具和符号：

- 爱心：想你、贴贴、喜欢。
- 蓝色眼泪柱：哭哭、委屈。
- 小花：谢谢、送你、害羞。
- 小门：来了、别走、躲一下。
- 小电脑 / 小牌牌：收到、忙着、OK。
- 小被子 / Zzz：晚安、困了。
- 光环 / 小翅膀：乖、安慰、天使感。
- 花瓣圆框：被包住、害羞、开花。

不要加完整背景。参考图里的“桌子、门、床、电脑”都只是几块简单色块，不是一个场景插画。道具要服务情绪，不要抢角色。

## 角色识别点

主角仍然来自 `../../../assets/source-cat/` 的浅奶茶小鹿色小猫，但必须重画成微型像素表情 sprite。

必须保留：

- 浅奶茶小鹿色的块面身体，不要偏纯白、冷白或深金色
- 圆圆的大头
- 小小三角耳朵
- 深色小眼睛，用 1 到 2 个像素点表达；不要画高光眼睛
- 粉色小鼻子，用 1 到 2 个像素点表达
- 脸侧特征只靠轮廓表达：脸侧最多各 1 个小毛尖，不画毛发纹理
- 无辜、认真、呆呆的表情，用极少像素表达

白底安全规则：眼睛、鼻子、嘴巴和轮廓都必须是 100% 不透明色块。不要让模型把黑底预览当成眼睛颜色，把眼睛挖成透明洞；这种图放黑底像有眼睛，换白底眼睛就会消失。

不要画成：普通白猫、橘猫、短毛猫、熊、兔子、狗、动漫吉祥物、平滑矢量贴纸、写实猫照片、半写实毛绒玩具。

## 细节预算

像素版的猫要像一个微型像素表情 sprite，不像一张被像素化的猫照片，也不像现代 Q 版贴纸。角色识别只靠这些显著特征：

- 浅奶茶小鹿色块面身体
- 圆头
- 三角耳朵
- 粉鼻点
- 两颗深色眼点
- 脸侧各 1 个小毛尖

猫身内部尽量保持纯色块。最多只允许 1 块浅米色阴影，不画毛丝、条纹、斑点、复杂胡须、毛绒边缘或多层高光。

## 伴侣角色

可以加一只固定互动角色，适合参考图里的双角色贴贴感。

建议设定：**浅可可棕小猫**。

- 体型和奶茶小猫一致
- 毛色是低饱和奶茶棕
- 眼睛用深棕或黑色小像素
- 只用于互动，不抢主角
- 常见动作：一起躺、抱心、躲门后、递花、并排睡觉、互相看一眼

如果生成模型容易把双角色画乱，先做单角色，再补双角色。

## 像素规则

### 画布

- 推荐源画布：`16 x 16`、`24 x 24` 或 `32 x 32`。
- 单角色优先 `24 x 24`，最多 `32 x 32`。
- 双角色或复杂道具最多用 `48 x 48`，不要再上更高细节。
- 如果最终需要 `300 x 300`，先生成或重绘低分辨率源图，再用 nearest-neighbor 放大。
- 成品导出时使用 nearest-neighbor 放大，保留硬边像素。
- 黑底只用于预览，正式成品优先透明背景。

判断标准：缩到 `24 x 24` 仍然成立，放大到 `300 x 300` 时能明显看见大块像素。

### 线条

- 外轮廓用 1 像素深色描边，优先黑色或深棕。
- 轮廓要硬、干净、像小图标，不要现代插画式柔和描边。
- 不要抗锯齿，不要柔边，不要平滑过渡。
- 不画毛丝、毛绒纹理、真实高光、真实阴影。
- 耳朵、爪子、尾巴都用块面和台阶边，不用圆滑曲线。

### 色盘

每张控制在 4 到 6 个主色以内。单个角色尽量像参考图那样：**3 到 4 个角色色 + 透明**。猫本体优先只用：轮廓色、主毛色、1 个阴影色、眼鼻色。

推荐基础色：

- 主毛色：浅奶茶小鹿色 `#F5DDC4`
- 高光：浅奶油鹿色 `#FFF2E2`
- 阴影：浅鹿色奶茶棕 `#E2C6AA`
- 轮廓：深灰棕 `#3A322C`
- 眼睛：深棕或黑 `#2C2522`
- 鼻子/爱心：软粉 `#F5A6BC`
- 可可棕角色：`#B9A092`

不要做大面积渐变。阴影最多 1 块平铺色，不用柔光、环境光、照片质感或毛发层次。颜色可以柔和，但必须是纯色块，不要渐变渲染。

### 构图

- 主体居中，四周留 4 到 8 像素呼吸空间。
- 小尺寸下先看动作剪影，再看五官。
- 一张只做一个动作或情绪。
- 道具只用一个：爱心、花、门、枕头、手机、信封、被子、小牌牌。
- 道具必须比脸更简单，不能抢主角。
- 构图优先微型表情图标角度：正面、侧面、极简 3/4。不要真实手机拍摄视角，不要大头贴纸海报构图。

### 输出归一化

最终 `stickers/` 源图统一为 `1024 x 1024` 透明 PNG。后处理时用实心主体区域（alpha >= 160）判断尺寸，把主体最长边统一到约 `620px`，居中放回透明画布。这样宣传图、微信预览和后续打包时不会忽大忽小。

### 文案

像素版优先无字。


如果要加字：

- 只写 1 到 4 个字。
- 建议后期手动加，不让模型直接生成中文。
- 字不要挤进 48px 源图里，可以在放大版底部另排。
- 常用字：想你、贴贴、收到、晚安、来了、抱抱、好耶、OK。

## 气质比例

- 贴贴：30%
- 日常回复：25%
- 可爱发呆：20%
- 安慰陪伴：15%
- 小小发疯：10%

这条线可以可爱，但不要变成很精致的大号商业软萌贴纸。它要像参考图那种小小的像素表情，被放大后拿来当聊天表情。

## 像素优先提示词原则

生成时不要说“真实猫”“照片”“长毛细节”“眼睛亮亮”“毛发蓬松真实”。这些词会让模型变写实。

要多说：

- `tiny pixel emoji`
- `pixel emoji sheet`
- `Tamagotchi-style sprite`
- `old web pixel icon`
- `Japanese deco-mail pixel emoji`
- `16x16 sprite`
- `24x24 sprite`
- `32x32 sprite`
- `black preview background`
- `transparent final PNG`
- `pixelated block shapes`
- `no anti-aliasing`
- `nearest-neighbor upscale`
- `visible square pixels`
- `limited palette`
- `flat solid color body`
- `minimal feature anchors`

参考图相关描述只保留一句：**参考图只用于角色配色和气质，不要复制成照片或半写实插画。**

## 常见跑偏：大号现代像素贴纸感

如果生成结果像“高清可爱插画被套了马赛克滤镜”或“现代软萌 pixel sticker”，就不合格。常见表现：

- 角色很大，像海报或商业贴纸，不像小 sprite。
- 眼睛有复杂反光、渐变和多层高光。
- 爱心有渐变、体积感或光泽。
- 猫脸、身体、耳朵里有很多碎色块，看起来像毛发纹理。
- 边缘有黑色噪点、脏边、透明残影或随机碎像素。
- 画面用了十几种颜色，像像素化后的高清图。
- 轮廓太圆润，整体像手机大贴纸，不像参考图里的小像素表情。
- 色彩用渐变渲染，而不是参考图那种纯色小块。

正确方向：先想象一张 `24 x 24` 源图。整只猫加道具只占 18 到 24 像素宽，放大后才看到方块。每个像素块都应该是有意摆放的，不是滤镜噪点。

## 常见跑偏：白底眼睛消失

如果黑底预览里看起来有黑眼睛，但放到白底后眼睛不见了，通常说明模型没有真正画深色眼点，而是把眼睛做成了透明挖空洞。黑底只是透出来了，所以误以为是黑眼睛。

修正提示词时优先加这几句：

```text
white-safe transparent PNG, transparent background outside the cat silhouette only.
The eyes, nose, mouth, and outline are opaque colored pixels, not transparent holes.
Two filled dark brown/black eye pixels must stay visible on a white background.
```

对应反向词：

```text
transparent eyes, hollow eyes, cutout eyes, white eyes, missing eyes, eyes made from background holes
```

如果仍然不稳，生成时先用浅蓝或浅灰纯色背景，而不是黑底；确认眼睛和轮廓都是真实深色像素后，再抠掉角色外部背景。不要在同一句里强强调 `black preview background` 和 `transparent final PNG`，模型容易把黑底当成透明孔洞的一部分。

## 通用生成提示词

```text
制作一张参考图风格的微型像素小猫表情 sprite，透明背景。参考图只用于角色配色、尺寸感和小表情气质，不要复制成照片。角色是一只浅奶茶小鹿色像素小猫：圆圆大头、小小身体、三角耳朵、两颗不透明深棕/黑色实心眼点、1 个不透明粉色鼻点、脸侧各 1 个小毛尖。猫身内部保持纯色块，不画纹理。

场景：小猫正在【填写具体动作或情绪】。

风格：tiny pixel emoji, pixel emoji sheet, Tamagotchi-style sprite, old web pixel icon, Japanese deco-mail pixel emoji, native 24x24 pixel art, white-safe transparent PNG, transparent background outside the cat silhouette only, limited 4-color palette, visible square pixels, chunky block shapes, flat solid color body, minimal feature anchors, clean dark outline, no anti-aliasing, nearest-neighbor upscale, centered composition, simple silhouette.

画面：主体清楚，小尺寸下动作一眼能懂。只保留一个小道具，不要复杂背景。猫的识别靠轮廓和几个关键像素点，不靠纹理。所有细节都由清晰像素块组成。透明通道只能出现在角色和道具外部，眼睛、鼻子、嘴巴和轮廓必须是不透明色块；换成白色背景时眼睛仍然清楚可见。

不要写文字，不要现代 pixel sticker，不要软萌商业贴纸，不要平滑插画，不要半写实贴纸，不要毛绒质感，不要真实毛发，不要毛丝，不要条纹，不要斑点，不要复杂胡须，不要真实光影，不要 3D，不要渐变，不要抗锯齿，不要复杂背景，不要真实照片，不要把猫画成陌生角色，不要透明眼睛，不要挖空眼睛，不要空白眼睛，不要用背景色当眼睛。
```

## 反向提示词

```text
modern pixel sticker, cute pixel sticker, soft kawaii sticker, pixel filter, mosaic filter, high-resolution pixelated illustration, oversized mascot illustration, poster sticker, black noisy outline, dirty transparent edges, random pixel noise, transparent eyes, hollow eyes, cutout eyes, white eyes, missing eyes, eyes made from background holes, glossy eyes, gradient heart, shiny heart, smooth illustration, vector sticker, semi-realistic sticker, plush toy, furry texture, realistic fur, fur strands, stripes, spots, complex whiskers, detailed eyes, soft lighting, realistic shadow, 3d render, realistic photo, anime chibi, watercolor, soft gradient, anti-aliasing, blurry, detailed background, complex scene, too many colors, large text, wrong Chinese characters, dog, rabbit, bear, orange tabby, pure white cat, different character
```

## 输出规格

- 源文件：`16x16`、`24x24` 或 `32x32` 透明 PNG；双角色最多 `48x48`。
- 预览文件：黑底或深灰底，方便看白色角色边缘。
- 聊天成品：`240x240`、`300x300` 或 `320x320` PNG。
- 放大方式：nearest-neighbor，不要双线性插值。
- 文件命名：`pixel-01-xiang-ni.png`、`pixel-02-tie-tie.png` 这种短拼音。

## 检查清单

生成后逐张检查：

- 透明背景是否干净。
- 放大后边缘是不是硬像素。
- 放大后是否能明显看到方块像素，而不是平滑贴纸。
- 小尺寸下能不能看懂动作。
- 奶茶小猫的毛色、圆脸、粉鼻子是否还在。
- 是否像原生小 sprite，而不是高清插画套像素滤镜。
- 有没有真实毛发、毛丝、条纹、斑点、复杂胡须、柔光、渐变、圆滑曲线；有就重做。
- 有没有黑色噪点边、脏透明边、随机碎像素；有就重做。
- 道具有没有抢主角。
- 有没有多余文字、乱码或奇怪肢体。
- 黑底预览和微信白底聊天里都能看清。

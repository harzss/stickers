# 像素奶茶小猫生成提示词

## 核心方向

目标不是大号像素贴纸，也不是硬核游戏角色，而是参考图那种**微型像素表情 sheet**：小、简单、可爱、情绪明确。

每张图只做一个小反应：

```text
1 个微型角色 / 2 个贴贴角色 + 1 个简单道具或符号 + 1 个明确情绪
```

表情不要复杂。靠两颗深色点眼、一个粉鼻点、短爪位置、一个道具或符号来表达。

## 输出归一化

生成后统一做后处理：输出为 `1024 x 1024` 透明 PNG，实心主体区域（alpha >= 160）的最长边约 `620px`，主体居中。不要让同一套里有的图占满画布、有的图只占中间一小块。

## 单角色无字模板

```text
制作一张参考图风格的原生 24x24 微型像素表情 sprite，透明背景。不是大号现代 pixel sticker，不是高清插画，不是像素滤镜，不是马赛克滤镜。最终可以放大预览，但源图必须像白底预览里的小像素表情图标。

角色是一只浅奶茶小鹿色像素小猫，主毛色接近 `#F5DDC4`，高光接近 `#FFF2E2`，阴影接近 `#E2C6AA`，不要偏纯白、冷白或深金色。整只小猫加道具总宽度控制在 18 到 24 像素左右，像参考图里的小图标，不像大头海报。只保留显著特征：圆头、小身体、两个三角耳、两颗不透明深棕/黑色实心眼点、1 个不透明粉色鼻点、脸侧各 1 个小毛尖、两块短前爪。猫身内部保持纯色块，不画纹理。

场景：小猫端坐，眼睛只用两个小点，嘴巴是一条短线，头顶飘一个紫色小问号。

风格：tiny pixel emoji, pixel emoji sheet, Told web pixel icon,  native 24x24 pixel art, hand-placed pixels, white-safe transparent PNG, transparent background outside the cat silhouette only, visible square pixels, chunky block shapes, flat solid color body, minimal feature anchors, limited 4-color palette, clean dark outline, no anti-aliasing, nearest-neighbor upscale.

画面：主体清楚，小尺寸下一眼能懂。所有边缘干净，像素块有意摆放。不要随机碎像素，不要脏透明边。眼睛只是两个深色实心像素点，不要反光和复杂瞳孔。透明通道只能出现在角色外部，不能把眼睛、嘴巴或轮廓挖空成透明洞；换成白色背景时眼睛仍然必须清楚可见。

不要文字，不要大号现代 pixel sticker，不要高清插画像素化，不要大尺寸吉祥物贴纸，不要渐变，不要阴影堆叠，不要眼睛高光，不要毛丝，不要条纹，不要斑点，不要复杂胡须，不要毛绒质感，不要真实光影，不要 3D，不要抗锯齿，不要复杂背景，不要透明眼睛，不要挖空眼睛，不要空白眼睛，不要用背景色当眼睛。
```

## 示例：想你

```text
制作一张参考图风格的原生 24x24 微型像素表情 sprite，透明背景。不是大号现代 pixel sticker，不是高清插画，不是像素滤镜，不是马赛克滤镜。最终可以放大预览，但源图必须像黑底预览里的小像素表情图标。

角色是一只浅奶茶小鹿色像素小猫，主毛色接近 `#F5DDC4`，高光接近 `#FFF2E2`，阴影接近 `#E2C6AA`，不要偏纯白、冷白或深金色。整只小猫加道具总宽度控制在 18 到 24 像素左右。只保留显著特征：圆头、小身体、两个三角耳、两颗不透明深棕/黑色实心眼点、1 个不透明粉色鼻点、脸侧各 1 个小毛尖、两块短前爪。猫身内部保持纯色块，不画纹理。

场景：小猫用两块短前爪夹住一颗 5 到 7 像素的纯粉色爱心，身体向前偏一格。爱心是纯色像素块，不要渐变和光泽。

风格：tiny pixel emoji, pixel emoji sheet, Tamagotchi-style sprite, old web pixel icon, Japanese deco-mail pixel emoji, native 24x24 pixel art, hand-placed pixels, white-safe transparent PNG, transparent background outside the cat silhouette only, visible square pixels, chunky block shapes, flat solid color body, minimal feature anchors, limited 4-color palette, clean dark outline, no anti-aliasing, nearest-neighbor upscale.

画面：主体清楚，小尺寸下一眼能懂。不要完整背景，不要额外装饰。所有边缘干净，像素块有意摆放。眼睛只是两个深色实心像素点，不要反光和复杂瞳孔。透明通道只能出现在角色外部，不能把眼睛、嘴巴或轮廓挖空成透明洞；换成白色背景时眼睛仍然必须清楚可见。

不要文字，不要大号现代 pixel sticker，不要高清插画像素化，不要渐变，不要阴影堆叠，不要眼睛高光，不要毛丝，不要条纹，不要斑点，不要复杂胡须，不要毛绒质感，不要真实光影，不要 3D，不要抗锯齿，不要复杂背景，不要透明眼睛，不要挖空眼睛，不要空白眼睛，不要用背景色当眼睛。
```

## 双角色互动模板

```text
制作一张参考图风格的微型像素双角色表情 sprite，透明背景。参考图只用于角色配色、尺寸感和小表情气质。不是大号现代 pixel sticker，不是高清插画，不是像素滤镜。

画面里有两只固定像素角色：一只是浅奶茶小鹿色像素小猫，主毛色接近 `#F5DDC4`，另一只是浅可可棕像素小猫。两只都只保留圆头、小身体、三角耳、两颗不透明深棕/黑色实心眼点、1 个不透明鼻点、短爪和纯色块身体，不画纹理。

场景：两只小猫正在【填写互动动作，例如并排贴贴、中间飘一颗小粉心、一起睡觉、从门后探头】。

表达方式：只用一个简单道具或符号表达关系，例如小粉心、枕头、小门、Zzz。不要完整背景。

风格：tiny pixel emoji, pixel emoji sheet, Tamagotchi-style sprite, old web pixel icon, Japanese deco-mail pixel emoji, native 32x32 or 48x48 two-character pixel art, white-safe transparent PNG, transparent background outside the characters only, limited 4-color palette per character, visible square pixels, chunky block shapes, flat solid color body, minimal feature anchors, clean dark outline, no anti-aliasing, nearest-neighbor upscale.

画面：两只角色要清楚分开，动作一眼能懂。不要随机碎像素，不要脏透明边，不要复杂场景。透明通道只能出现在角色和道具外部，不能把眼睛、嘴巴或轮廓挖空成透明洞；换成白色背景时眼睛仍然必须清楚可见。
```

## 带短字模板

优先不让模型写中文。如果必须让模型带字，用这个版本，只写 1 到 4 个字。

```text
制作一张参考图风格的微型像素中文聊天表情包，透明背景。主体是一只浅奶茶小鹿色像素小猫，主毛色接近 `#F5DDC4`，圆头、小身体、三角耳、两颗不透明深棕/黑色实心眼点、1 个不透明粉色鼻点、短爪和纯色块身体。

短字：【想你】
场景：小猫正在【填写具体动作或情绪】。

风格：tiny pixel emoji, pixel emoji sheet, Tamagotchi-style sprite, old web pixel icon, Japanese deco-mail pixel emoji, native 32x32 or 48x48 sprite with text area, white-safe transparent PNG, transparent background outside the cat silhouette only, limited 4-color palette, visible square pixels, chunky block shapes, flat solid color body, minimal feature anchors, clean dark outline, no anti-aliasing, nearest-neighbor upscale. 中文短字放在底部，字少、清楚、不要挡住小猫。透明通道只能出现在角色外部，不能把眼睛、嘴巴或轮廓挖空成透明洞。

不要乱码，不要错别字，不要长句，不要渐变，不要眼睛高光，不要真实毛发，不要复杂背景，不要透明眼睛，不要挖空眼睛，不要空白眼睛，不要用背景色当眼睛。
```

## 英文模板

```text
Create a tiny pixel emoji cat sprite with a transparent background, matching the attached pixel emoji sheet reference. Use the reference only for the small-size feeling, simple props, and clear emotion; do not copy it as a photo or semi-realistic illustration.

The character is a pale milk-tea fawn pixel cat, with the main fur color close to #F5DDC4, highlights close to #FFF2E2, and shadows close to #E2C6AA. It must not look pure white, cool white, or deep golden. It has a round head, tiny body, triangle ears, two opaque dark brown/black filled eye pixels, one opaque pink nose pixel, one tiny cheek point on each side, and short blocky paws. Keep the body as flat solid color blocks with no texture.

Scene: the cat is [specific action or emotion]. Use only one simple prop or symbol, such as a heart, tear, flower, small door, laptop, blanket, Zzz, halo, or tiny wings. No full background.

Style: tiny pixel emoji, pixel emoji sheet, Tamagotchi-style sprite, old web pixel icon, Japanese deco-mail pixel emoji, native 24x24 pixel art, white-safe transparent PNG, transparent background outside the cat silhouette only, limited 4-color palette, visible square pixels, chunky block shapes, flat solid color body, minimal feature anchors, clean dark outline, no anti-aliasing, nearest-neighbor upscale.

The action must be readable at very small size. Alpha transparency is allowed only outside the character and props. The eyes, mouth, nose, and outline must be painted as opaque colored pixels, never transparent holes or background cutouts. The eyes must stay visible on a white background. No text, no modern pixel sticker, no soft kawaii sticker, no smooth illustration, no semi-realistic sticker, no plush texture, no realistic fur, no fur strands, no stripes, no spots, no complex whiskers, no realistic lighting, no 3D, no gradients, no anti-aliasing, no realistic photo, no complex scene.
```

## 反向提示词

```text
modern pixel sticker, cute pixel sticker, soft kawaii sticker, pixel filter, mosaic filter, high-resolution pixelated illustration, oversized mascot illustration, poster sticker, black noisy outline, dirty transparent edges, random pixel noise, transparent eyes, hollow eyes, cutout eyes, white eyes, missing eyes, eyes made from background holes, glossy eyes, gradient heart, shiny heart, smooth illustration, vector sticker, semi-realistic sticker, plush toy, furry texture, realistic fur, fur strands, stripes, spots, complex whiskers, detailed eyes, soft lighting, realistic shadow, 3d render, realistic photo, anime chibi, watercolor, soft gradient, anti-aliasing, blurry, detailed background, complex scene, too many colors, large text, wrong Chinese characters, dog, rabbit, bear, orange tabby, pure white cat, different character
```

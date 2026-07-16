# 生图提示词模板

每张图单独生成。调用 `image_gen` 时，根据选角传入对应角色设定图的绝对路径。

```text
Generate one standalone 16:9 horizontal Chinese article illustration as a single narrative scene.

Reference-image rule:
Use the supplied character sheet image(s) as the highest-priority identity, hairstyle, costume, color, proportion, and hand-drawn texture reference. Do not copy the turnaround layout, multiple-view lineup, white-sheet composition, or pose sequence. Do not redesign the characters from unrelated animation, live-action, game, or web references.

Selected cast:
{韩立 / 南宫婉 / 韩立与南宫婉}

Casting reason:
{为什么这个主题需要该角色；若双人同场，说明必须表达的互补、权衡或协作}

Character identity:
- 韩立: a chibi young male cultivator with long black hair tied in a top bun by a slim gold hairpin, remaining hair down the back, dark navy-blue outer robe with gold trim, pale blue water-pattern inner robe, calm focused eyes, controlled posture.
- 南宫婉: a chibi young female cultivator with long black hair, an ornate silver-blue floral crown with blue ribbons and pearl details, a small red forehead flower mark, layered pale-blue and white hanfu with dark-blue sash and embroidered wide sleeves, bright but composed expression.
Include only the selected character or characters. Never swap their hair ornaments, costume colors, or personality cues. Do not add generic companions or character clones.

Theme:
{正文配图主题}

Core idea:
{这张图要表达的唯一核心意思}

Structure:
{输入输出 / 系统局部 / 前后对比 / 角色状态 / 概念隐喻 / 方法分层 / 地图路线 / 双角色协作}

Character action:
{每个入镜角色正在做什么；必须是解释概念的核心动作}

Character interaction:
{双角色时必填：谁先行动、对方如何回应、结构因此发生什么变化；单角色写 none}

Composition:
{主体位置、主要物件、信息流向、留白区域}

Chinese handwritten labels:
{3-5 个短标注，每个 2-8 个字}

Visual DNA:
Pure white background. Clean chibi cultivation-themed hand-drawn illustration. Slightly wobbly blue-black pencil or crayon linework with visible tactile grain. Preserve the characters' blue, pale-blue, silver-blue, navy, gold, and tiny red identity accents. Keep surrounding objects mostly sparse line art. Lots of empty white space. Clear concept first, cultivation flavor second.

Color semantics:
Blue-black for structure and text. Navy for stable systems and Han Li's costume. Pale or silver blue for connection, feedback, and Nangong Wan's costume. Gold only for decisive actions, useful paths, or tiny highlights. Red only for warnings, failures, or fixed identity details such as Nangong Wan's forehead mark.

Relationship rule:
Han Li and Nangong Wan are equal, restrained, mutually trusting cultivation partners. If both appear, give both independent agency and a visible conceptual interaction. Do not default to romance, rescue, hand-holding, gazing, hearts, or pink atmosphere. Nangong Wan must not be reduced to a cute spectator; Han Li must not make every decision for her.

Constraints:
One image, one core structure, one coherent scene. Main subject around 40%-60% of the canvas with at least 35% clean white space. Use 3-5 short readable Chinese labels. No title in the top-left. No PPT infographic, formal flowchart, course slide, dense explainer, realistic UI, anime screenshot, live-action likeness, 3D render, game key art, ornate palace background, giant magic circle, character sheet, turnaround, lineup, collage, or repeated character views. Cute and lively is allowed; childish mascot, sticker, emoji, or exaggerated moe styling is not.
```

## 图像编辑：去除标题

```text
Edit the provided image. Remove only the handwritten title "{要删除的文字}" and its underline. Fill the area with clean white background. Preserve the characters, identity details, labels, paths, line texture, composition, aspect ratio, and image quality. Add nothing new.
```

## 角色纠错

```text
Regenerate the same single-scene illustration using the supplied character sheet as the strict identity reference. Correct the hairstyle, hair ornament, costume layers, color palette, forehead mark if applicable, and body proportions. Preserve the core idea and layout. Do not output a turnaround sheet, lineup, or extra character.
```

## 双角色互动纠错

```text
Regenerate with the same core idea, but give Han Li and Nangong Wan distinct, equally necessary actions. Show a clear cause-and-response interaction. Remove romantic posing and passive spectatorship. Preserve their individual reference-sheet appearance and the sparse white-background hand-drawn style.
```

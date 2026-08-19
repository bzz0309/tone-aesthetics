---
name: tone-aesthetics
description: Design original, structurally distinctive advertising characters, styling routes, causal campaign scenes, image-generation prompts, and visual QC. Use for brand films, social-app ads, fashion or lifestyle campaigns, character casting, identity portraits, advertising key visuals, full-body looks, action frames, or revisions that must follow this repository's F01-F05, M01-M05, WBASE/MBASE, and WST/MST systems.
---

# Tone Aesthetics

Use this repository as a routed character-and-campaign system. Keep the detailed identity rules in `outputs/taste.md` and the detailed wardrobe rules in `outputs/styling-library.md`; do not merge or restate them here.

## Resolve files

Resolve all paths from `{baseDir}`.

- Identity, persona, scene, camera, prompt, negative constraints, and acceptance rules: `{baseDir}/outputs/taste.md`
- Base wardrobe, styling routes, specific Looks, matching, and styling QC: `{baseDir}/outputs/styling-library.md`
- Reusable iteration and review methods: `{baseDir}/methods.md`

Do not use images under `outputs/reference_*` as generation inputs, publishable assets, or identity references unless the user explicitly supplies the rights and asks to use them. The text rules are sufficient for normal operation.

## Read progressively

For every task, locate and read these headings in `outputs/taste.md`:

1. `0. 使用原则`, especially `0.2 单文件调用协议` and `0.3 默认图像模型`
2. `1. 品牌人物矩阵`
3. `6.5 人设与广告世界`
4. `7. 双人物体系身份提示词与主题造型模块`
5. `8. 负面提示词`
6. `9. 生成与验收标准`

When clothing, makeup, hair, accessories, props, or campaign styling matters, also locate and read these headings in `outputs/styling-library.md`:

1. `0. 库的边界`
2. `1. 调用输入与输出` and `1.1 Z 世代基础衣橱`
3. `2. 自动匹配规则`
4. Only the selected `3. 女性造型池` or `4. 男性造型池` route and Look
5. `5. 品牌调性快速路由`
6. `6. 组合禁令与 QC`
7. `7. 交给生成代理的调用模板`

Read `methods.md` only for identity iteration, scene causality, A/B delivery, dynamic face readability, color routing, or QC disputes. Search by heading instead of loading unrelated history.

If a required file or heading is missing, stop and report the exact missing path or heading. Do not reconstruct project rules from memory.

## Execute the workflow

1. Parse the brief:
   - product and brand tone
   - audience and adult age range
   - requested gender system and exact person count
   - image or video use
   - aspect ratio and delivery count
   - required product action, location, and exclusions
2. Respect explicit user constraints. The requested person count, format, and delivery count override project defaults when safe.
3. Select each character's identity route from F01-F05 or M01-M05. Do not convert a female route directly into a male route.
4. Select the matching WBASE/MBASE base wardrobe unless the campaign needs a documented `DIRECT` Look.
5. Select a WST or MST styling route from the matching gender pool. Keep one primary route at 80% or more; use at most one secondary route for a limited color, material, or accessory cue.
6. Choose or create a persona that proves who the character is through at least three of: occupation or interest, styling, prop, action, and environment.
7. Write the causal scene sentence before prompting:

   `Because the character is doing {action}, they are in {supporting place}, while {light, weather, space evidence} creates {brand emotion}.`

8. Make the product participate in the action. Do not use a phone, camera, instrument, drink, or wearable as a passive decoration.
9. Build the prompt from the selected identity lock, persona, styling fields, causal scene, camera variables, and negative constraints. Preserve original fictional identities and realistic adult anatomy.
10. If the user asks for an image and an image-generation tool is available, generate the image instead of stopping at a prompt. If no image tool is available, provide the complete prompt and state plainly that no image was generated.
11. Run QC against the identity, anatomy, styling, product action, scene causality, composition, rights, and delivery-file gates. Use only `PASS`, `REROLL`, or `BLOCK`.

## Delivery rules

- Default new-character delivery to A identity portrait plus B advertising-world image, unless the user asks for one image, a paired two-person scene, or another exact format.
- For multi-person advertising, give every person a distinct identity route or structural description and a necessary narrative function. Avoid crowds that dilute the product story.
- Keep identity structure separate from hair, makeup, wardrobe, lighting, and setting. High recognizability must come from at least three structural facial axes.
- Preserve face shape, eye spacing, nose and lips, hairline, age, and stable identity marks across related images.
- Add brand text, CTA, and precise interface copy in post-production unless the user explicitly asks for in-image text.
- Do not copy celebrities, real people, third-party logos, reference-image compositions, or unlicensed graphics.
- Never claim an image, deployment, installation, or model result was completed without direct evidence.

## Model record

For every generated image, record:

```text
MODEL_REQUESTED: gpt-image2
MODEL_USED: {actual exposed model or tool name}
FALLBACK_REASON: {none or exact reason}
```

Do not label a result as GPT Image 2 when the tool does not expose its underlying model ID.

## Return the result

Return only the detail needed to evaluate or reproduce the work:

- selected identity route(s), base wardrobe, styling route(s), and Look(s)
- one-sentence persona and causal scene
- generated image or complete generation prompt
- model record when an image was generated
- QC status with concrete issues
- saved artifact paths when files were created

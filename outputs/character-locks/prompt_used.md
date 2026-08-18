# Prompt Set — Dual Character Lock

Generation path: built-in image generation using identity-preserve reference inputs.

## Multi-angle identity sheet — shared prompt

```text
Use case: identity-preserve
Asset type: canonical multi-angle identity sheet for an original adult brand-film character
Primary request: Use Image 1 as the sole canonical identity reference. Create a single clean landscape contact sheet showing the exact same adult woman repeated in six separate, evenly sized head-and-shoulders portrait panels.
Panel layout: 3 columns by 2 rows, consistent panel size and spacing, no overlapping figures.
Required views in reading order: front neutral; subject turned 45 degrees to her left; subject turned 45 degrees to her right; left profile; right profile; front with a restrained closed-mouth micro-smile.
Scene/backdrop: identical seamless warm light-gray studio background in every panel
Style/medium: photorealistic professional casting and character-continuity photography
Lighting: identical large soft directional studio light, neutral exposure, no dramatic mood changes
Wardrobe: the same plain charcoal crew-neck T-shirt in every panel, no logo and no accessories
Invariants: preserve the exact same facial identity from Image 1 in every panel—same apparent age, skull shape, facial width and length, cheekbone placement, jaw, chin, eye shape and spacing, eyelid crease, brows, nose bridge and tip, mouth width and lip structure, ears, hairline, black hair length and texture, skin tone and distinctive mark. Preserve natural realistic asymmetry.
Hair continuity: same natural black jaw-to-collarbone razor-layered bob/lob in all panels; same sparse piecey fringe and same face-framing strands; no hair-length or parting change.
Constraints: exactly one identity repeated six times, adult age 24–28, realistic anatomy, honest pores and hair strands, each full head visible, no cropped crown, no hands, no props, no text, no labels, no graphic borders, no watermark.
Avoid: six different women, identity drift, face averaging, changed age, changed makeup, changed jaw, changed nose, changed eye spacing, changed hairline, changing beauty-mark position, mirrored or duplicated view, beauty filter, influencer face, K-pop styling, doll face, pointed V chin, oversized eyes, porcelain skin, e-commerce makeup lighting.
```

## Full-body validation — shared prompt

```text
Use case: identity-preserve
Asset type: full-body wardrobe validation still for a premium Gen-Z brand film
Input images: Image 1 is the canonical front portrait and Image 2 is the canonical multi-angle identity sheet of the same original fictional adult woman. Preserve this exact identity. Image 3 is wardrobe silhouette and material reference only; do not copy its person, pose, logo, text, brand mark, city landmark or exact garment graphics.
Style/medium: photorealistic premium contemporary fashion editorial, real camera, authentic fabric and skin texture
Composition/framing: vertical full-body portrait, entire head and both shoes fully visible, natural adult proportions, 50mm fashion-editorial perspective, no wide-angle distortion
Identity invariants: exact same face, apparent age, skull shape, facial proportions, eye spacing, nose, mouth, jaw, chin, ears, hairline and stable hair design as Images 1–2; same natural skin tone and realistic asymmetry; no identity blending with Image 3
Garment physics: physically correct layers, seams, pockets, waistline, sleeve openings, fabric weight and folds; no fused clothing, no disappearing layers
Constraints: adult age 24–28, original character, no third-party logo, no copied brand wordmark, no random text, no watermark
Avoid: different face, influencer face, K-pop styling, childlike proportions, exaggerated body, tiny waist filter, plastic skin, long legs caused by wide-angle lens, impossible clothing layers, malformed hands, extra fingers, cropped feet, e-commerce catalog lighting
```

Character-specific identity and wardrobe deltas are recorded in `taste.md` under the dual-character roster and recommended looks.

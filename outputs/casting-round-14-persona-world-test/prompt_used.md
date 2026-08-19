# Round 14 — 人设广告世界测试

## 测试目的

验证 `taste.md v0.11` 能否在不输入真人参考图的情况下，把一条人物骨相路线与人设、妆造、道具、动作和场景组合为可想象的广告视频关键帧。

## 使用组合

- 生成模式：广告角色
- 人物体系：WOMAN
- 人物路线：F02 ANDROGYNOUS SIGNAL / 中性先锋
- 人设：P01 COASTAL ALT MUSICIAN / 海岸公路独立乐手
- 广告适配：耳机、音响、音乐应用、手机、相机、潮流服饰、饮料
- 输入图片：无。用户提供的广告截图只用于抽象组合机制，不作为身份、构图或服装复刻输入。

## 实际提示词

```text
Use case: ads-marketing
Asset type: cinematic 16:9 brand-film character keyframe and casting-world test

Primary request: Create one original fictional adult East Asian woman, age 24–27, as a clearly imagined advertising character rather than a studio model. She is an independent alternative musician who turns an ordinary coastal commute into a temporary rehearsal space. Do not resemble any celebrity or real person.

Identity lock — F02 ANDROGYNOUS SIGNAL: a long rectangular-oval East Asian face, medium-long midface, subtle high lateral cheek planes, broad nearly parallel jaw sides, a longer broad blunt chin with a softly squared U-shaped base, narrow heavy-lidded almond eyes with modest spacing, very low straight brows, a longer ordinary natural nose, upper lip thinner than lower lip, mature softness around the mouth, realistic skin texture and slight natural asymmetry. Adult, striking and structurally distinctive; no pointed chin, no oversized eyes, no influencer or idol template.

Persona — P01 COASTAL ALT MUSICIAN: calm offstage, physically decisive while playing. She has a shoulder-length choppy wolf-lob with natural black roots and a restrained smoky plum-to-ink-blue underlayer revealed by wind. One strong accessory signal only: translucent amber angular prescription glasses. Makeup is not bare and not stage-heavy: softly smoked taupe-plum outer eye, thin horizontal liner, defined natural lashes, muted berry-nude lips, real skin.

Wardrobe: an original unbranded asymmetrical off-shoulder graphic knit layered over a charcoal ribbed tank, loose washed-black carpenter trousers, worn low-profile black leather shoes, one oxidized-silver ear cuff and a narrow belt. The graphic must be abstract with no readable words, copied logos or band marks. Real fabric weight and physically correct layering.

Campaign world: a bright windy East Asian coastal service road beside a concrete sea wall and small harbor structures, late morning, hard blue sky and sunlit sea, youthful but cinematic. This is not a recreation of any supplied screenshot. Her original unbranded deep-red offset-body electric guitar is connected to a compact portable practice amp clipped at her waist.

Action: medium-wide environmental action frame as she steps off the curb and actively tightens a tuning peg with her left hand while striking one testing chord with her right; hands and instrument geometry must be plausible, strap weight visible, hair and loose fabric moving in the sea wind. She glances past the camera with focused, slightly rebellious confidence rather than posing.

Composition: 16:9 cinematic advertising still, low-to-eye-level 45–55mm environmental portrait, three-quarter to nearly full body, subject slightly left of center, sea and road creating motion lines, clean negative space in the upper-right for later campaign typography. Premium music-fashion commercial, crisp daylight, subtle film grain, controlled cobalt / charcoal / deep-red palette.

Constraints: exactly one person; original fictional identity; adult East Asian appearance; meaningful prop use; action-readable hands; no neutral studio, no passive centered pose, no generic black T-shirt, no school uniform, no cosplay, no cheap punk costume, no third-party logo, no readable random text, no watermark, no subtitles, no floating product, no extra instruments, no anatomy errors.
```

## v2 定向重试：降低视觉年龄、更新妆造

用户反馈 v1 的脸和穿搭都显成熟。v2 锁定同一条 F02 × P01 路线，但将屏幕年龄明确为 21–23 岁，并用年轻软组织、轻盈长层次发、彩色镜框、当代运动技术层搭和更有反应的动作替换成熟摇滚语汇。

```text
Use case: ads-marketing
Asset type: cinematic 16:9 Gen-Z brand-film character keyframe

Create one original fictional adult East Asian woman, visibly 21–23 years old, as a contemporary Gen-Z alternative musician in an ad-film world. She must look unmistakably like a young adult, not a teenager and not a mature editorial model. Do not resemble any celebrity or real person.

Identity — youthful F02 ANDROGYNOUS SIGNAL: compact medium-length rectangular-oval East Asian face with softly supported youthful cheeks, subtle lateral cheek planes without hollowness, a broad clean jaw with a softly squared U-shaped chin, a medium rather than long lower face, narrow heavy-lidded almond eyes with alert playful focus, low straight brows, an ordinary natural low-to-medium nose, defined lips with the lower lip slightly fuller, fresh elastic skin with real texture and slight asymmetry. No gauntness, no severe cheekbones, no long dry lower face, no nasolabial folds, no tired eye bags, no pointed chin, no oversized doll eyes, no influencer or idol template.

Persona — COASTAL ALT MUSICIAN: cool but quick to react, playful while performing. Long airy layered hair to the lower chest, natural black at the crown melting into a restrained steel-blue underlayer and thin smoky-lilac face-framing strands, glossy healthy movement rather than dry shag. One accessory signal: bold translucent cobalt rectangular glasses. Youthful editorial makeup: clean skin, soft pink-lilac eye wash, thin horizontal navy liner, fresh diffused cool-rose cheek color, muted berry balm lips; expressive but not stage-heavy.

Wardrobe: lightweight asymmetric cobalt-and-milk-white sporty zip top with curved technical panels over a charcoal fitted rib tank, cropped just above the natural waist; oversized silver-grey parachute cargo trousers with a low visual center but secure adult fit; slim black-red training shoes; one small chrome ear cuff. Clean color blocking only, absolutely no words, logos, band graphics, coarse knitwear, all-black grunge or office tailoring. Contemporary youthful high-low styling with real fabric weight and correct layers.

Campaign world: bright windy East Asian coastal street beside a concrete sea wall, compact harbor buildings and a distant elevated rail line, intense blue sky, youthful cinematic daylight. She wears an original unbranded cherry-red offset electric guitar on a visible strap.

Action: dynamic three-quarter/full-body action frame during a short rehearsal take — one foot landing from a small side-step, right hand actively striking the strings, left hand placed plausibly on the fretboard, guitar cable and strap behaving naturally, hair and lightweight top lifted by sea wind. She looks toward a bandmate outside frame with a quick confident half-smile, not a commercial grin and not a passive pose.

Composition: 16:9 premium Gen-Z music / phone / headphone commercial still, 40–50mm environmental portrait, low-to-eye-level camera, energetic diagonal guitar line, subject left of center, generous blue-sky negative space on the right for later typography, crisp daylight, subtle film grain, cobalt / milk-white / silver-grey / cherry-red palette.

Constraints: exactly one adult East Asian woman; visually age 21–23; clear persona, prop and action; plausible hands and instrument; no copied composition; no neutral studio; no mature model face; no coarse knitwear; no generic black T-shirt; no passive centered pose; no school uniform; no cosplay; no cheap punk costume; no third-party logo; no letters; no random text; no watermark; no subtitles; no floating product; no extra instruments; no anatomy errors.
```

# Handoff

## 项目状态

项目名：调性审美  
核心文件：`outputs/taste.md` v0.18 + `outputs/styling-library.md` v0.5
当前阶段：造型库已扩展到女性 WST01–WST10、男性 MST01–MST06；新增层构街头、日系亚文化、都市朋克、暗黑浪漫与男性日系朋克，可继续用品牌主题做交叉测试。

默认图片模型：GPT Image 2，项目逻辑名称 `gpt-image2`。模型不可用、调用失败或环境只提供其他模型时允许自动切换／降级；生成记录必须保存请求模型、实际模型与回退原因。

发色规则：人物路线优先于广告主题。F02 中性先锋、F05 灵动甜酷适合主动使用银灰、灰金、烟紫、浅金、铜橘或彩色内层；F01 清冷极简、F03 自然淡颜、F04 摩登浓颜以黑色、棕色、蓝黑和低明度酒红棕为主。发色必须与服装主色和场景光线联动；强发色时减少眼妆、印花和大首饰。

## 先看这些文件

1. `outputs/taste.md`
2. `outputs/styling-library.md`
3. `outputs/casting-round-15-identity-ad-pair/prompt_used.md`
4. `outputs/casting-round-15-identity-ad-pair/qc_report.md`
5. `worklog.md`
6. `methods.md`

## 最新可用资产

- `outputs/casting-round-13-male-taste-test/m02-soft-refined-makaron-ad-v1.png`
- `outputs/casting-round-13-male-taste-test/m02-soft-refined-makaron-fullbody-look01-v1.png`
- `outputs/casting-round-14-persona-world-test/f02-p01-coastal-alt-musician-keyframe-v1.png`
- `outputs/casting-round-14-persona-world-test/f02-p01-coastal-alt-musician-keyframe-v2-younger.png`
- `outputs/casting-round-15-identity-ad-pair/f05-p01-identity-portrait-v1.png`
- `outputs/casting-round-15-identity-ad-pair/f05-p01-ad-world-livehouse-street-v1.png`
- `outputs/casting-round-15-identity-ad-pair/f05-p01-ad-world-coastal-performance-v2.png`

## 下一步建议

1. 请用户确认 Round 15 A 与海岸公路 B2 是否是可接受的同一人物，以及 B2 的造型、动作与广告世界是否达到参考图审美。
2. 从 WST07 层构街头、WST08 日系亚文化、WST09 都市朋克、WST10 暗黑浪漫或 MST06 日系朋克中任选一条做双图测试，验证新路线不会互相串味。
3. 正式投放前清理或重试 v2 琴头的疑似字样，并补同身份全身图和动作关键帧。
4. 保留 M02 旧测试作为身份链路证据，不再把灰背景或普通基础款当作最终广告角色默认输出。

## GitHub 状态

- private 仓库：`https://github.com/bzz0309/tone-aesthetics`
- 默认分支：`main`
- 本轮 v0.15、造型库 v0.3、Round 15 v2 与新增资产尚未自动推送；外部同步前确认提交范围。
- 在用户明确要求 public 前，不公开 `outputs/reference_*` 目录。

## 安全与一致性

- 不复制现实人物或明星身份。
- 不把女性人物直接转换为男性版本。
- 不把外部参考图视为可商用资产。
- 不在未通过身份 QC 前批量生成视频镜头。

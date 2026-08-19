# Handoff

## 项目状态

项目名：调性审美  
核心文件：`outputs/taste.md` v0.19 + `outputs/styling-library.md` v0.5
当前阶段：`taste.md` 已完成 skill 路由式精简，造型细节只在 `styling-library.md` 维护；女性 WST01–WST10、男性 MST01–MST06 保持不变，可用同一需求对精简前后版本做 A/B 测试。

安装入口：根目录 `SKILL.md`，skill 名称为 `tone-aesthetics`。入口按任务读取 `taste.md`、`styling-library.md` 和必要的 `methods.md` 章节，不复制详细规范。

默认图片模型：GPT Image 2，项目逻辑名称 `gpt-image2`。模型不可用、调用失败或环境只提供其他模型时允许自动切换／降级；生成记录必须保存请求模型、实际模型与回退原因。

发色规则：人物路线优先于广告主题。F02 中性先锋、F05 灵动甜酷适合主动使用银灰、灰金、烟紫、浅金、铜橘或彩色内层；F01 清冷极简、F03 自然淡颜、F04 摩登浓颜以黑色、棕色、蓝黑和低明度酒红棕为主。发色必须与服装主色和场景光线联动；强发色时减少眼妆、印花和大首饰。

## 先看这些文件

1. `outputs/taste.md`
2. `outputs/styling-library.md`
3. `SKILL.md`
4. `outputs/casting-round-15-identity-ad-pair/prompt_used.md`
5. `outputs/casting-round-15-identity-ad-pair/qc_report.md`
6. `worklog.md`
7. `methods.md`

## 最新可用资产

- `outputs/casting-round-13-male-taste-test/m02-soft-refined-makaron-ad-v1.png`
- `outputs/casting-round-13-male-taste-test/m02-soft-refined-makaron-fullbody-look01-v1.png`
- `outputs/casting-round-14-persona-world-test/f02-p01-coastal-alt-musician-keyframe-v1.png`
- `outputs/casting-round-14-persona-world-test/f02-p01-coastal-alt-musician-keyframe-v2-younger.png`
- `outputs/casting-round-15-identity-ad-pair/f05-p01-identity-portrait-v1.png`
- `outputs/casting-round-15-identity-ad-pair/f05-p01-ad-world-livehouse-street-v1.png`
- `outputs/casting-round-15-identity-ad-pair/f05-p01-ad-world-coastal-performance-v2.png`
- `outputs/social-app-match-test-01/social-app-match-cafe-v1.png`

## 下一步建议

1. 请用户确认 Round 15 A 与海岸公路 B2 是否是可接受的同一人物，以及 B2 的造型、动作与广告世界是否达到参考图审美。
2. 从 WST07 层构街头、WST08 日系亚文化、WST09 都市朋克、WST10 暗黑浪漫或 MST06 日系朋克中任选一条做双图测试，验证新路线不会互相串味。
3. 正式投放前清理或重试 v2 琴头的疑似字样，并补同身份全身图和动作关键帧。
4. 保留 M02 旧测试作为身份链路证据，不再把灰背景或普通基础款当作最终广告角色默认输出。

## GitHub 状态

- 当前公开仓库：`https://github.com/bzz0309/tone-aesthetics`
- 默认分支：`main`
- 根目录 `SKILL.md` 使公开仓库可以通过 `git:bzz0309/tone-aesthetics@main` 安装测试；每次同步状态以 `git status` 和远端 `main` 为准，不在交接文档固化易过期的提交哈希。
- 精简前 v0.18 已备份并推送为标签 `pre-slim-v0.18-20260819`，目标提交为 `ee1fad2a8e219c44b38539afcc4f23141d4ffbb9`。
- A/B 测试时分别安装为 `tone-aesthetics-v018` 与 `tone-aesthetics-v019`，每组使用新会话、同一模型和同一原始提示词。
- `outputs/reference_*` 含研究阶段参考素材。仓库已经公开，应尽快完成权利审查或从公开历史中移除；skill 默认禁止加载这些图片为生成输入。

## 安全与一致性

- 不复制现实人物或明星身份。
- 不把女性人物直接转换为男性版本。
- 不把外部参考图视为可商用资产。
- 不在未通过身份 QC 前批量生成视频镜头。

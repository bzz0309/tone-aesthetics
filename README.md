# 调性审美

面向品牌广告与 Makaron 投放素材的人物调性、妆发、穿搭和图像生成规范项目。

当前核心成果由两份文件组成：[outputs/taste.md](./outputs/taste.md) v0.19 负责原创亚洲成年人物身份、人设与广告世界，[outputs/styling-library.md](./outputs/styling-library.md) v0.5 负责按照性别、品牌调性、人物行为与场景匹配完整造型。两份文件职责分离，造型细节只在造型库维护。

根目录 [SKILL.md](./SKILL.md) 是 OpenClaw/Codex 的轻量执行入口：它按任务读取上述两份规范，而不是把人物与造型规则合并成一个大文件。

默认图片生成模型为 **GPT Image 2**，项目内逻辑名称使用 `gpt-image2`。模型不可用、调用失败或环境只提供其他模型时允许自动切换／降级；每轮必须记录请求模型、实际模型和回退原因。

## 当前能力

- 通过广告主题自动选择人物路线。
- 先按性别进入独立造型池：女性 WST01–WST10，男性 MST01–MST06；两套分类不做机械性别转换。
- 提供男女独立基础衣橱：女性 WBASE01–WBASE07，男性 MBASE01–MBASE04；常规广告先选基础廓形，再叠加风格路线。
- 通过品牌调性在新潮叛逆、Y2K甜酷、韩系运动与 Hot Nerd 四种女性风格原型中路由，再与脸型路线分开组合。
- 从脸型、纵向比例、眼型、鼻形、唇形和真实质感构建原创身份。
- 将人物身份与发型、妆容、服装及 Y2K 等主题模块分开。
- 将学院解构、Y2K牛仔、韩系运动、Balletcore、Hot Nerd、层构街头、日系亚文化、都市朋克、暗黑浪漫与男性日系朋克提炼为可组合造型语法，并强制填写发色、配饰和角色道具。
- 采用“人物路线优先”的发色系统：F02 中性先锋、F05 灵动甜酷开放明显发色，F01 清冷极简、F03 自然淡颜、F04 摩登浓颜保持黑棕及低明度色域；场景只在路线允许范围内选择发色。
- 从八组人设母版中自动选择或组合职业／兴趣、标志物、动作与广告世界。
- 由角色行为反推场景，用空间证据、天气、光线、风和色彩建立可用于 TVC 的氛围，而不是默认套用街巷背景。
- 默认先输出同身份的“A 身份基准肖像 + B 广告世界主视觉”双图，再扩展同场景全身穿搭、动作关键帧和广告适配说明。
- 为连续视频建立多角度身份锁与 QC 门槛。

## 目录

- `outputs/taste.md`：人物身份、人设、广告世界、提示词与 QC 规范源。
- `outputs/styling-library.md`：造型路线、具体 Look、发色、妆容、配饰、道具与自动匹配规则源。
- `outputs/casting-round-*`：历轮人物生成、提示词和质量记录。
- `outputs/casting-round-13-male-taste-test`：男性 M02 单文件链路与全身穿搭测试。
- `outputs/casting-round-14-persona-world-test`：F02 × P01 人设广告世界测试。
- `outputs/casting-round-15-identity-ad-pair`：F05 × P01 身份肖像与广告世界双图测试。
- `outputs/reference_*`：研究阶段的参考素材，仅作内部审美拆解，不代表可对外商用。
- `outputs/character-locks`：已建立的人物身份锁实验。
- `AGENT.md`：项目级协作约束。
- `worklog.md`：事实性工作记录。
- `methods.md`：可复用方法。
- `handoff.md`：下一轮工作交接。

## 使用提示

生成新人物时先阅读 `outputs/taste.md` 锁定身份和人设，再读取 `outputs/styling-library.md` 选择对应性别的造型路线和具体 Look。默认只生成原创亚洲成年人，不复制现实人物或明星身份。参考图只用于抽象结构和造型语言；公开投放前必须重新确认图片、服装图形和品牌资产的使用权。

## OpenClaw 安装测试

公开仓库可以直接安装到当前 OpenClaw 工作区：

```bash
openclaw skills install git:bzz0309/tone-aesthetics@main --as tone-aesthetics
openclaw skills info tone-aesthetics
openclaw skills check
openclaw skills list --eligible
```

安装后开启新会话，再用真实广告需求测试。首次测试不要添加 `--global`、`--force` 或自动发布动作。

精简前的 v0.18 已冻结为 `pre-slim-v0.18-20260819`。需要比较精简前后行为时，用不同名称并存安装：

```bash
openclaw skills install git:bzz0309/tone-aesthetics@pre-slim-v0.18-20260819 --as tone-aesthetics-v018
openclaw skills install git:bzz0309/tone-aesthetics@main --as tone-aesthetics-v019
```

分别开启新会话，固定图片模型、原始需求、宽高比和交付数量，只切换 skill。比较路线选择、因果场景、完整提示词和最终 QC；图片随机性不应被误判为规则变化。

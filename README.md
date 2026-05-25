# 倪海厦skill · nihaixia
[![版本](https://img.shields.io/badge/版本-v2.0.1-blue)](https://github.com/jangviktor-web/nihaixia/releases)
[![开源协议](https://img.shields.io/badge/协议-MulanPSL--2.0-green)](LICENSE)
[![ClawHub](https://img.shields.io/badge/ClawHub-nihaixia-orange)](https://clawhub.ai/skills/nihaixia)
[![OpenClawMP](https://img.shields.io/badge/OpenClawMP-v2.0.1-blueviolet)](https://openclawmp.cc)
[![SkillHub](https://img.shields.io/badge/SkillHub-nihaixia--pro-red)](https://skillhub.cloud.tencent.com/skills/nihaixia-pro)
[![IMA支持](https://img.shields.io/badge/支持-腾讯IMA%20APP-purple)]()

> 「中医很简单，就是阴阳气血。你搞懂了，一通百通。」—— 倪海厦

**将经方大师倪海厦的完整中医思维体系注入 AI Agent，覆盖伤寒论 129 条、金匮 23 篇、黄帝内经 71 篇、针灸教程、神农本草经 345 种、849 个医案、天纪命理体系、梁冬对话，合计 2,452 页原始讲义、3.5M 字精萃内容。**

**仓库精简版**：仅保留运行核心文件（4MB），原始参考资料（110MB）已移除。

---

## 安装指南

### 方式一：ClawHub 一键安装（推荐）

```bash
# 安装 ClawHub CLI
npm install -g clawhub

# 登录
clawhub login

# 安装倪海厦skill
clawhub install nihaixia
```

安装完成后，在 Claude Code 对话中直接说「倪海厦」即可激活。

### 方式二：SkillHub 安装（腾讯云）

```bash
# 访问 SkillHub 网站
# https://skillhub.cloud.tencent.com/skills/nihaixia-pro

# 或使用 CLI 安装
npm install -g skillhub

# 登录
skillhub login

# 安装倪海厦skill
skillhub install nihaixia-pro
```

### 方式三：OpenClaw 安装

```bash
# 安装 OpenClaw CLI
npm install -g openclaw

# 安装本技能
openclaw skills install nihaixia
```

### 方式四：OpenClawMP 安装

```bash
# 安装 OpenClawMP CLI
npm install -g openclawmp

# 搜索倪海厦skill
openclawmp search 倪海厦

# 安装（使用资产ID）
openclawmp install skill/c03b361cb99d4b4ebc6cd17f361741ba
```

### 方式五：手机端快速使用（无需配置 OpenClaw）

如果大家懒得配置 OpenClaw 或者希望在手机上面直接使用，请下载**腾讯 IMA APP**，导入本 SKILL 即可一键使用。

**扫码下载 IMA APP，搜索「倪海厦」即可找到本技能：**

### 知识码导入截图
<img width="408" height="684" alt="【倪海厦skill】知识码" src="https://github.com/user-attachments/assets/3c8ba629-4a81-45b8-aca2-a82f7ac786e5" />

### IMA APP 演示截图
<img width="1458" height="1080" alt="IMA APP演示" src="https://github.com/user-attachments/assets/d70c6a0d-5b87-46b5-9833-fc2002980a02" />

### 方式六：手动安装

1. 克隆仓库：
```bash
git clone https://github.com/jangviktor-web/nihaixia.git
```

2. 将 `SKILL.md` 和 `modules/` 目录复制到你的 Agent 技能目录：
```bash
# Claude Code 用户
cp -r nihaixia/ ~/.claude/skills/nihaixia/

# OpenClaw 用户
cp -r nihaixia/ ~/.openclaw/skills/nihaixia/
```

3. 重启 Agent 会话，在对话中使用触发词激活。

---

## 项目声明
本项目基于开源项目二次开发，遵循开源规范注明所有来源。

## 来源说明
- 基础框架：https://github.com/huoyalong/nihaisha-skill
- 医案数据：https://github.com/9527qingfeng/hantang-nihaixia-follower
- 汉唐文章集锦：倪海厦汉唐中医经典文章医案集（383 页 PDF）
- 倪海厦文集：倪海厦文集及医案最新版（139 页 PDF）

## 是什么
将倪海厦（1954-2012）的中医思维、人纪系列教学内容、临床心法、天纪命理体系蒸馏为可激活的 Agent Skill，使 AI 能以倪海厦的视角分析中医问题、解读症状、给出辨证思路与经方建议，同时具备易经、紫微斗数、阳宅风水等命理学知识。

**直接激活词**：倪海厦 / 海厦视角 / 倪师 / 经方思维 / 倪海厦会怎么看

---

## 使用示例

```
你从倪海厦的角度分析一下：病人肺癌晚期，咳嗽有血，应该怎么处理？
```

```
倪师，小柴胡汤的使用要点是什么？什么情况下可以加减？
```

```
生附子和炮附子有什么区别？分别在什么情况下用？
```

---

## 效果演示

### 1. 六经辨证基础应用（感冒辨证）
<img width="729" height="510" alt="六经辨证" src="https://github.com/user-attachments/assets/98af88a7-fbaa-4a50-ac63-7f10e8c61dbe" />

### 2. 六经传变规律
<img width="726" height="509" alt="六经传变" src="https://github.com/user-attachments/assets/af0fb0c1-944b-4846-8dc2-4aaa2bc5b531" />

### 3. 日常养生与饮食禁忌（五味观）
<img width="731" height="509" alt="饮食养生" src="https://github.com/user-attachments/assets/7c252c14-9497-4a94-be31-4a9670df3afb" />

---

## 核心特色

### 六大经方心法

| 心法 | 内容 |
|---|---|
| **六经辨证** | 太阳→阳明→少阳→太阴→少阴→厥阴，传变规律与欲解时 |
| **阳气论** | 阳气不足先扶阳；阴病用阳药；生附子/生硫磺/炮附子精准区分 |
| **经典至上** | 以《伤寒论》《金匮要略》原文为核心，经方不随意加减 |
| **经方为主** | 温病派滋阴派不用；麻黄、附子、石膏等经方药重获正视 |
| **诊断优先** | 十问为核心，眼诊/舌诊/脉诊/腹诊四诊合参 |
| **治未病** | 节气养生、饮食五味、情志管理贯穿诊疗全程 |

### 十三大内容模块

| 模块 | 内容规模 | 状态 |
|---|---|---|
| **伤寒论** | 条文 1-129 全覆盖，含倪海厦讲义补遗 12 条 | 129/129 |
| **金匮要略** | 23 篇完整蒸馏，419 页讲义验证 | 23/23 |
| **人纪·黄帝内经** | 71 篇完整蒸馏，基于 461 页讲义 PDF | 71 篇 |
| **人纪·针灸教程** | 216 页讲义蒸馏，含十二经络/井荣俞经合/任督要穴 | 完整 |
| **人纪·神农本草经** | 339 页视频同步文稿蒸馏，含三品分类/药性体系 | 完整 |
| **人纪·医案集** | 849 个医案结构化，243 个超长医案已标记 | 849 例 |
| **分类医案库** | 按疾病类型分类：癌症 147/心血管 22/代谢 12/自免 2/神经 3/其他 59 | 245 例 |
| **口述表达DNA** | 倪海厦口语表达风格模块 | 完整 |
| **天纪体系** | 天机道（紫微斗数）/人间道（易经）/地脉道（风水） | 完整 |
| **人纪班闭门课** | 7 大重病专题 + 7 堂弟子课 | 完整 |
| **梁冬对话精华** | 2009 年 12 月 7 期对话录音完整蒸馏 | 完整 |
| **汉唐文章精华** | 10 篇专题文章（乳癌/便秘/心脏病/保养/药害等） | 完整 |
| **汉唐诊疗日志** | 8 则精选医案 + 4 则经典案例 | 完整 |

### 数据来源清单

| 讲义 | 页数 | 提取字符 | 状态 |
|---|---|---|---|
| 伤寒论讲义 | 209 页 | 277K | 全量蒸馏 |
| 金匮要略讲义 | 419 页 | 626K | 全量蒸馏 |
| 黄帝内经讲义 | 461 页 | 227K | 全量蒸馏 |
| 针灸教程讲义 | 216 页 | 347K | 全量蒸馏 |
| 神农本草经文稿 | 339 页 | 843K | 全量蒸馏 |
| 天机道（紫微斗数） | 75 页 | 85K | 全量蒸馏 |
| 人间道（易经） | 146 页 | 164K | 全量蒸馏 |
| 地脉道（风水） | 65 页 | 52K | 全量蒸馏 |
| 汉唐文章集锦 | 383 页 | 670K | 10 篇蒸馏 |
| 倪海厦文集 | 139 页 | 234K | 8 则医案蒸馏 |
| **合计** | **2,452 页** | **3.5M** | |

---

## 核心观点速览

### 生附子 vs 炮附子 vs 生硫磺

| 药物 | 对应证候 | 典型表现 |
|---|---|---|
| **生附子** | 阴寒（病在里、阳气极虚） | 四逆证：脚冷至膝 / 手冷至肘 |
| **炮附子** | 表虚（表阳不固） | 汗出恶风、卫气不固 |
| **生硫磺** | 水中火（命门火衰） | 水肿、关节肿痛、阴寒水肿 |

### 六经传变规律

```
太阳（表）→ 阳明（里热）→ 少阳（半表半里）
         ↓ 失治误治
太阴（脾寒）→ 少阴（心肾阳虚）→ 厥阴（阴阳逆乱 / 上热下寒）
```

### 倪氏六健康标准

1. 一觉到天亮，无失眠
2. 胃口正常，三餐有饱饿感
3. 每天晨起大便
4. 一天小便 5-7 次，淡清黄色
5. 头面冷、手足温热（四季皆然）
6. 晨起阳反应（男勃起 / 女乳房敏感）

### 天纪三才一体

天命（紫微斗数）+ 人事（易经）+ 地理（阳宅风水）= 趋吉避凶

> 「天、人、地各占三分之一，人事上绝佳的医学技术再加上地理优越的位置，占了三分之二，就大于天命了。这就是人与天争。」—— 倪海厦

### 五味饮食观

| 厚味 | 伤害 | 淡味 | 归属 |
|---|---|---|---|
| 咖啡（浓酸） | 伤脾→伤肾→骨伤 | 蔬菜淡苦 | 入心 |
| 牛奶（酸性） | 伤脾/胰 | 天然蔗糖 | 缓急止痛 |
| 重盐 | 伤骨/心 | 天然海盐 | 适量护正 |

---

## 仓库结构

```
nihaixia/
├── SKILL.md                    # 主技能文件（840K，Claude 直接读取）
├── distilled_cases.md          # 849 医案结构化索引
├── expression_style.md         # 倪海厦口语表达风格模块
├── modules/                    # 9 个知识模块（详细内容）
│   ├── 01_shanghan_sun.md      # 伤寒论太阳篇
│   ├── 02_shanghan_other.md    # 伤寒论其他五经
│   ├── 03_yian.md              # 医案集（849 例完整版）
│   ├── 04_jingui.md            # 金匮要略
│   ├── 05_huangdi_neijing.md   # 黄帝内经
│   ├── 06_liangdong.md         # 梁冬对话
│   ├── 07_bimen_hantang.md     # 闭门课+汉唐
│   ├── 08_huangdi_detail.md    # 黄帝内经详注
│   └── 09_zhenjiu_bencao.md    # 针灸+神农本草经
├── cases/                      # 分类医案（按疾病类型）
│   ├── 01_cancer.md            # 147 个癌症医案
│   ├── 02_cardiovascular.md    # 22 个心血管医案
│   ├── 03_metabolic.md         # 12 个代谢病医案
│   ├── 04_autoimmune.md        # 2 个自身免疫医案
│   ├── 05_neurological.md      # 3 个神经精神医案
│   └── 06_other.md             # 59 个其他医案
├── references/research/        # 研究资料
│   ├── combined_reference.md   # 合并参考（生平/表达/教学/临床）
│   ├── 01-writings.md          # 著作总览
│   ├── 02-conversations.md     # 对话风格
│   └── ...                     # 其他研究文件
└── README.md
```

**SKILL.md 目录结构**：
```
一、角色设定 → 身份卡 / 角色扮演规则 / 回答工作流
二、心智模型 → 六经辨证 / 太阳病篇条文1-129 / 其他五经
三、决策启发式 / 表达DNA / 价值观 / 智识谱系
四、伤寒论六经完整解读（条文1-129）
五、金匮要略23篇完整解读
六、人纪·医案集（849 例）+ 汉唐诊疗日志精选
七、人纪班闭门课（7 大重病 + 7 堂弟子课）
八、梁冬对话精华（2009年12月7期）
九、人纪·黄帝内经（71篇完整）
十、人纪·针灸教程 / 神农本草经
十一、天纪体系（天机道/人间道/地脉道）
十二、汉唐文章精华（10篇）
十三、倪海厦推荐书目
十四、口述表达DNA
```

---

## 更新日志

- **v2.0.1** (2026-05-26)：新增分类医案库 cases/（245 例，按疾病类型分类）+ 研究资料 references/；修复 .gitignore 忽略 cases/ 的问题
- **v2.0.0** (2026-05-25)：仓库精简——移除原始参考资料(110MB)、完整版SKILL.full.md、测试报告等非核心文件，仅保留运行必需文件(4MB)；新增仓库结构说明
- **v1.1.2** (2026-05-24)：详情页重写——新增安装教程（ClawHub/OpenClaw/腾讯IMA/手动四种方式）、使用示例
- **v1.1.1** (2026-05-24)：更名为「倪海厦skill」，slug 改为 `nihaixia`；发布至 ClawHub
- **v1.1.0** (2026-05-23 StableV2026.5.23+Bencao)：神农本草经药性体系深度蒸馏；关键词索引全面优化；9 个知识模块检索路径全部校验
- **v1.0.1** (2026-05-02)：结构优化；OCR 校正 13 处；新增汉唐文章精华 10 篇 + 诊疗日志 8 则
- **v1.0.0** (2026-04-14)：初版发布——伤寒论 + 金匮要略 + 黄帝内经 + 医案集 + 闭门课全量蒸馏

---

## 致谢

- 感谢 [huoyalong](https://github.com/huoyalong/nihaisha-skill) 提供 nihaisha-skill 基础框架
- 感谢 [9527qingfeng](https://github.com/9527qingfeng/hantang-nihaixia-follower) 提供医案数据支持

---

## 免责声明

本项目内容仅供中医学习与研究，不替代专业医疗诊断。所有诊疗请务必咨询执业医师。

---

Built with OpenClaw

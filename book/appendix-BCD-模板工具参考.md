# 附录B：文档模板库

> **说明：** 以下所有模板均为**可填空结构**。复制到你的笔记本或文档工具中，按序填写。每个空行都应留下答案、假设或“未知及验证方式”，而不是被无意识地跳过。

---

## B.1 概念要素表模板

> **用途：** 第1步（概念孵化）使用。将灵感翻译为可讨论的书面描述。
> **填写时机：** 创意激荡结束后，竞品研究开始前。

| 字段 | 你的回答 |
|------|---------|
| **游戏名称（暂定）** | |
| **Elevator Pitch（一句话）** | 一句话说明：玩家扮演___，通过___，实现___。 |
| **Design Pillars（核心体验支柱）** | 1.（标注优先级） |
| | 2. |
| | 3. |
| | 4. |
| **Core Mechanic（当前主机制/候选机制）** | 1.（标注验证优先级） |
| | 2. |
| | 3. |
| **Genre（类型）** | |
| **Target Audience（目标玩家）** | 年龄： / 平台： / 游戏习惯： / 他们现在在玩什么： |
| **Market Hypothesis（市场假设）** | "___玩家在玩___时，最大的痛点是___。我的游戏通过___解决了这个问题。" |
| **竞品引用** | 直接竞品： |
| | 间接竞品： |
| **差异化声明（一句话）** | "与___不同，我的游戏___。" |

---

## B.2 一页纸GDD模板

> **用途：** 第2步（轻量设计概要）核心产出。建议控制在一页左右，确保团队能快速复核。
> **原则：** 用篇幅约束促进取舍，但复杂项目可附链接或补充页；能被快速复核比机械满足页数更重要。

```
────────────────────────────────────
游戏名称：
────────────────────────────────────

【Pitch（一句话）】

【Design Pillars】
1.
2.
3.

【Core Loop】

  玩家动作 ──→ 系统反馈 ──→ 状态/资源/信息/空间变化
       ↑                        │
       └────── 新目标/挑战 ←─────┘

【Scope Boundary】
┌──────────────────┬──────────────────┐
│   Must Have     │    Won't Have    │
├──────────────────┼──────────────────┤
│                  │                  │
│                  │                  │
│                  │                  │
│                  │                  │
└──────────────────┴──────────────────┘

【Art Direction（美术方向）】
Art Pillars：
1.
2.
色板（主色调）：
参考图链接（列出足以说明方向的图片）：
反例清单（当前不采用的视觉方向）：
1.
2.

────────────────────────────────────
```

---

## B.3 十页纸设计文档模板

> **用途：** 第4步（设计深化）核心产出。在一页纸通过原型验证后，展开为可执行的详细设计。
> **原则：** 每页独立回答一个问题。写完这十页，你应该能估算出整款游戏的生产头绪。

| 页 | 标题 | 填写内容 |
|----|------|---------|
| 1 | **游戏概述** | Elevator Pitch + Design Pillars（从一页纸升级）。当前版本的一句话描述与变更记录。 |
| 2 | **Core Loop 展开** | 完整核心循环箭头图，含关键状态/资源/信息变化、转化节点和退出条件。附：循环时长范围、节奏条件与未知项。 |
| 3 | **机制清单** | 所有游戏机制的完整枚举。每个机制写：名称、触发条件、系统响应、与其他机制的交互、引入条件和验证状态。 |
| 4 | **内容类型清单** | 所有内容资产的分类枚举。如：敌人类（`Enemy_Melee`, `Enemy_Ranged`, `Boss`）、道具类、环境资产类、UI面板类。每类附数量估算、品质档位和依赖。 |
| 5 | **关卡/进度结构** | Macro Chart：一张总表列出所有关卡/区域/章节的名称、引入机制、节奏假设、难度曲线位置和验证状态。附关卡解锁流程图。 |
| 6 | **系统设计** | 所有非核心系统展开（成长系统、经济系统、存档系统、成就系统、排行榜等）。每个系统写：设计意图、运作规则、数值范围、与其他系统的数据交互。 |
| 7 | **叙事结构** | 故事大纲（如有）、叙事交付方式（对话/环境/文档）、关键叙事节拍与关卡的对应关系。纯机制游戏此页可压缩为"世界观设定"一段。 |
| 8 | **UI/UX 信息架构** | 完整屏幕流程图：主菜单 → 存档选择 → 游戏内HUD → 暂停菜单 → 设置 → 通关画面 → 返回。HUD布局草图（标注每个元素的位置和信息类型）。 |
| 9 | **美术与音频管线** | Art Direction（从一页纸升级版）、资产规范（分辨率/格式/命名约定）、音频清单（音乐类型、音效分类、环境音）。附：资产生产流程（概念→草图→终稿→引擎导入）。 |
| 10 | **Scope Budget** | 内容 × 数量 × 单位成本 = 总工时。记录单位成本依据、依赖、返工风险与情景范围。详细见 B.4 模板。 |

---

## B.4 Scope Budget 计算表模板

> **用途：** 第4步（设计深化）使用。从内容反向估算生产总时间。
> **原则：** 第一次填写时所有数字都是"占位符"。VS之后用真实产能数据替换。

| 内容类型 | 数量 | 单位成本（人·天） | 小计（人·天） | 备注（单位成本依据） |
|----------|------|-------------------|--------------|---------------------|
| **关卡/场景** | | | | 灰盒 → 美术 → Lighting Pass |
| └ 其中：灰盒布局 | | | | |
| └ 其中：终稿美术 | | | | |
| └ 其中：Lighting Pass | | | | |
| **敌人/NPC** | | | | 含行为脚本 + 模型 + 动画 |
| └ 其中：普通敌人 | | | | |
| └ 其中：Boss | | | | |
| └ 其中：NPC/对话角色 | | | | |
| **道具/可收集物品** | | | | 含 2D 图标 + 3D 模型 + 效果脚本 |
| **UI 面板** | | | | 含布局 + 交互逻辑 + 多语言适配 |
| **音效** | | | | 含录制/采购 + 引擎集成 |
| **音乐曲目** | | | | 含创作 + 循环编辑 + 动态分层 |
| **过场/叙事** | | | | 含脚本 + 镜头 + 动画 + 配音（如需） |
| **本地化** | | | | 按语言数 × 文本量估算 |
| **平台适配** | | | | 输入适配 + 性能测试 + 提审修改 |
| **杂项/Bug Fix 预留** | | | | 按历史数据、风险清单或切片产能估算，并说明依据 |
| **总计** | — | — | ____ 人·天 | |

---

## B.5 VS 产能测算表模板

> **用途：** 第5步（垂直切片）的核心数据产出。用覆盖主要内容类型和关键依赖的代表性样本估算全量产能。
> **原则：** 首个样本暴露从零搭建的成本，后续样本检验复用、变化和返工。不要把单一比例当作普遍结论。

| 项目 | 值 | 说明 |
|------|-----|------|
| **切片1（首个完整场景/关卡）** | | |
| └ 切片1内容描述 | | 如"森林主题第一关，含2种敌人 + 1个 Boss + 3种可破坏物" |
| └ 切片1实际耗时（天） | ____ 天 | 从头开始做完的完整时间 |
| └ 切片1涉及内容类型数 | | 敌人/道具/环境资产各多少 |
| **后续代表性样本** | | 可按关卡、敌人、Boss、UI或平台适配等内容类型分别取样 |
| └ 样本内容描述 | | 说明新增资产、复用资产和特殊依赖 |
| └ 样本实际耗时（天） | ____ 天 | 记录开发、沟通、返工和等待依赖的时间 |
| └ 样本涉及新内容类型数 | | |
| **产能分析** | | |
| └ 复用与变化 | | 记录哪些环节变快、持平或变慢，以及原因 |
| └ 单位成本区间 | ____ 天 | 按内容类型、品质档位和依赖分别记录 |
| └ 预计内容量 | | 从 Macro Chart 和 Scope Boundary 取，并标注仍不确定的部分 |
| └ 生产情景 | | 记录基准、保守和收缩范围等情景（如适用） |
| └ **全量生产预估** | **____ 天** | 给出区间、假设和返工/等待风险 |
| **判断** | | |
| └ 可用资源（人·天） | ____ 天 | 记录团队投入、外部依赖和时间窗口 |
| └ 是否有缺口？ | 是 / 否 / 未知 | 有缺口或未知 → 比较砍内容、改方案、增加资源和延后发布等选项 |

---

## B.6 Playtest 记录表模板

> **用途：** 第3步（原型验证）、第7步（迭代打磨）的标准化测试记录。
> **原则：** 不记录等于没测。每个测试者单独一张表。

| 字段 | 记录 |
|------|------|
| **Tester ID** | （保护隐私，用编号代替姓名） |
| **测试日期** | |
| **测试版本** | （Build 号或日期） |
| **测试者画像** | 游戏经历：新手 / 普通 / 核心 / 开发者 |
| | 同类游戏经验：有 / 无 |
| | 当前在玩的游戏： |
| **Play Duration** | ____ 分钟 |
| **Exit Point** | 退出前在做什么： |
| | 退出原因：主动退出 / 游戏结束 / 技术问题 |
| **Confusion Points** | 1. （什么时刻不知道该做什么） |
| | 2. |
| | 3. |
| **Frustration Points** | 1. （什么时刻感到挫败或不公平） |
| | 2. |
| **Favorite Moment** | （最享受的一个时刻） |
| **"Would Continue?"** | 是 / 否 / 可能 |
| | 如果否/可能——最阻碍继续玩的原因： |
| **测试者自由补充** | |
| **观察者备注** | （观察到的表情、自言自语、冷笑话——这些比问卷更真实） |
| **本轮核心变量/改动** | （本轮主要改变了什么；如有联动改动，逐项记录） |
| **改动的效果判断** | 有效 / 无效 / 不确定——依据： |

---

## B.7 通关！奖励关模板索引

> **来源：** Scott Rogers《通关！游戏设计之道》第二版，书末"奖励关"系列（Bonus Levels 1-10）提供了大量可直接套用的空白模板。以下为奖励关内容索引，方便读者在需要时按图索骥。（注：本模板库中的 B.2/B.3 已对 Rogers 的模板做了适配和精简。）

| 奖励关 | 内容 | 适用场景 |
|--------|------|---------|
| 奖励关 1 | **单页说明书模板** | 本书第2步（一页纸GDD）的原型 |
| 奖励关 2 | **十页说明书大纲** | 本书第4步（十页纸）的原型 |
| 奖励关 3 | **完整游戏设计文档大纲**（GDD 结构参考） | 本书第6步（生产开发）的文档骨架 |
| 奖励关 4 | **流程表模板**（Walkthrough 表） | 关卡策划/QA 用——记录每一屏发生什么 |
| 奖励关 5 | **角色设计表** | 第8章（生产开发）的角色模板 |
| 奖励关 6 | **敌人/NPC 设计表** | 第8章（生产开发）的敌人模板 |
| 奖励关 7 | **道具/技能设计表** | 系统设计的项目规模拆解 |
| 奖励关 8 | **关卡设计表** | 第13章（关卡设计）配套 |
| 奖励关 9 | **UI/菜单/HUD 设计表** | 第14章（UI/UX设计）配套 |
| 奖励关 10 | **计费点（Monetization Points）设计表** | 第16章（商业模式与发布）配套 |

---

# 附录C：工具箱

> **说明：** 以下工具按本书七步流程的使用阶段分组。每个工具标注名称、用途、费用（Free / Freemium / Paid）、最常用步骤、零预算替代方案。
>
> **选择原则：** 先选零预算工具。只有在确信付费工具能节省大量时间时才升级。

---

## C.1 设计工具

| 工具 | 用途 | 费用 | 用在哪一步 | 零预算替代 |
|------|------|------|-----------|-----------|
| **Miro** | 在线白板：头脑风暴、流程图、信息架构、情绪板 | Freemium（3块免费白板） | Step 1, 2, 4, 14 | 实体白板+拍照 / Excalidraw（免费） |
| **Excalidraw** | 开源手绘风格白板，极适合箭头图和流程图 | Free | Step 1, 2, 4, 14 | —（本身就是零预算首选） |
| **Notion** | 文档写作、知识库、看板、数据库合并 | Freemium | 全部步骤 | Obsidian（免费本地）/ 纯 Markdown + 文件夹 |
| **Obsidian** | 本地Markdown知识库，双向链接，图视图 | Free（个人用） | 全部步骤 | — |
| **PureRef** | 参考图管理：拖放图片、自由排列、始终置顶 | Free（可捐款） | Step 2, 4, 5, 10-14 | 文件夹 + 系统预览 / Figma（免费层级） |
| **Figma / FigJam** | 矢量设计 + 协作白板 | Freemium | Step 2, 4, 14 | Penpot（开源） |
| **Google Sheets / Excel** | 数值平衡、Scope Budget、Macro Chart、经济模拟 | Free / Paid | Step 3, 4, 6, 7, 15 | LibreOffice Calc |
| **draw.io (diagrams.net)** | 流程图、系统架构图、箭头图 | Free | Step 2, 4, 11, 14 | — |
| **Xmind / MindNode** | 思维导图 | Freemium | Step 1, 3 | 纸笔 / Excalidraw |

---

## C.2 原型工具

| 工具 | 用途 | 费用 | 用在哪一步 | 零预算替代 |
|------|------|------|-----------|-----------|
| **纸 + 笔 + 骰子 + 筹码/代币** | 纸上原型（A阶段）：验证核心规则和数值感觉 | 几乎免费 | Step 3 | —（本身就是零预算首选） |
| **Google Sheets** | 电子表格原型：回合制、经济系统、概率模拟 | Free | Step 3 | LibreOffice Calc |
| **Unity Engine** | 通用游戏引擎，2D/3D，资源商店庞大 | Free（Personal） | Step 3, 5, 6, 7 | Godot（开源免费） |
| **Godot Engine** | 开源游戏引擎，轻量，2D/3D，MIT许可证 | Free | Step 3, 5, 6, 7 | —（本身就是零预算首选之一） |
| **Unreal Engine** | 高端3D引擎，蓝图可视化脚本 | Free（royalty门槛后收费） | Step 3, 5, 6, 7 | Godot / Unity（更轻量的替代） |
| **GameMaker Studio 2** | 2D游戏专用引擎，快速原型 | Freemium | Step 3, 5, 6, 7 | Godot |
| **PICO-8 / TIC-80** | 虚拟幻想游戏机，内置代码/美术/音效全工具 | Paid（$15） / Free | Step 3 | TIC-80（免费开源） |
| **Construct 3** | 浏览器端无代码2D引擎 | Freemium | Step 3 | GDevelop（免费开源） |
| **Twine** | 交互叙事/文字冒险原型工具 | Free | Step 3（叙事原型） | — |
| **Machinations.io** | 游戏经济/系统循环可视化模拟 | Freemium | Step 3, 11, 15 | 纸笔 + Google Sheets |

---

## C.3 项目管理

| 工具 | 用途 | 费用 | 用在哪一步 | 零预算替代 |
|------|------|------|-----------|-----------|
| **Trello** | 看板式任务管理 | Freemium（10块免费看板） | Step 4-8 | 实体便签墙 / Notion看板 |
| **Notion** | 数据库+看板+日历+文档合体 | Freemium | 全部步骤 | — |
| **GitHub Projects** | 代码仓库自带看板，Issues关联 | Free | Step 5-8, 16 | — |
| **GitLab** | 自托管代码仓库 + CI/CD + 项目管理 | Free（社区版） | Step 5-8, 16 | — |
| **HacknPlan** | 专为游戏设计的项目管理（设计文档+任务整合） | Freemium | Step 4-8 | Trello + 手动关联 |
| **Linear** | 现代软件开发项目管理 | Freemium | Step 5-8 | GitHub Issues |
| **Jira** | 大型团队项目管理 | Paid（10人以下免费） | Step 5-8 | Trello / GitHub Projects |
| **Google Calendar** | 里程碑时间线 | Free | 全部步骤 | — |

---

## C.4 美术工具

| 工具 | 用途 | 费用 | 用在哪一步 | 零预算替代 |
|------|------|------|-----------|-----------|
| **Aseprite** | 像素动画精灵表编辑器 | Paid（$20，可自行编译开源版） | Step 4-8 | LibreSprite（开源分叉） |
| **Krita** | 开源数字绘画（概念图、贴图、UI资产） | Free | Step 2, 4-8 | — |
| **GIMP** | 开源图像处理（贴图编辑、批量处理） | Free | Step 4-8 | — |
| **Inkscape** | 开源矢量图形（UI图标、logo） | Free | Step 4-8, 14 | — |
| **Blender** | 完整3D管线：建模、雕刻、绑定、动画、渲染 | Free | Step 4-8 | — |
| **Procreate** | iPad数字绘画（概念图、贴图手绘） | Paid（$13一次性） | Step 2, 4-8 | Krita（桌面端）/ Sketchbook（免费） |
| **Affinity Designer / Photo** | 矢量/位图设计（Adobe替代） | Paid（一次性，非订阅） | Step 4-8 | Inkscape + GIMP |
| **MagicaVoxel** | 轻量体素建模+渲染 | Free | Step 4-6 | — |
| **Blockbench** | 低多边形3D模型编辑器（Minecraft风/通用） | Free | Step 4-6 | Blender |
| **Material Maker / ArmorPaint** | 程序化材质/PBR贴图绘制 | Free / Paid | Step 4-6 | — |

---

## C.5 音频工具

| 工具 | 用途 | 费用 | 用在哪一步 | 零预算替代 |
|------|------|------|-----------|-----------|
| **Audacity** | 开源音频录制和编辑 | Free | Step 5-7 | — |
| **LMMS** | 开源数字音频工作站（作曲） | Free | Step 5-7 | — |
| **Reaper** | 专业数字音频工作站 | Paid（$60折扣许可，可无限试用） | Step 5-7 | LMMS / Audacity |
| **BFXR / jsfxr / ChipTone** | 复古8-bit音效生成器（浏览器/桌面） | Free | Step 5-7 | — |
| **Bosca Ceoil** | 极简芯片音乐作曲（Terry Cavanagh监制） | Free | Step 5-7 | — |
| **Freesound.org** | 免费音效素材库（CC许可） | Free | Step 5-7 | — |
| **FMOD / Wwise** | 游戏音频中间件（动态音乐、交互音效） | Free（预算<$200k） | Step 6-7 | 引擎自带音频系统 |

---

## C.6 营销与发布工具

| 工具 | 用途 | 费用 | 用在哪一步 | 零预算替代 |
|------|------|------|-----------|-----------|
| **Steamworks** | Steam上架、成就、云存档、愿望单 | $100/游戏（可回收） | Step 6-7, 16 | itch.io（免费上架） |
| **itch.io** | 独立游戏发布平台，支持pay-what-you-want | Free | Step 6-7, 16 | — |
| **OBS Studio** | 开源录屏/直播（制作预告片、devlog） | Free | Step 6-7, 16 | — |
| **DaVinci Resolve** | 专业视频编辑/调色（预告片、devlog） | Free（标准版） | Step 6-7, 16 | — |
| **Canva** | 简易平面设计（宣传图、社媒图） | Freemium | Step 6-7, 16 | GIMP / Krita |
| **X/Twitter, Bluesky, TikTok, Bilibili** | 社交媒体：DevLog、GIF分享、愿望单引流 | Free | Step 1, 6-7, 16 | — |
| **Discord** | 社区服务器搭建（玩家反馈、测试者管理） | Free | Step 6-7, 16 | — |
| **Mailchimp / ConvertKit** | 邮件列表（发布通知） | Freemium | Step 6-7, 16 | — |
| **Presskit() (Rami Ismail)** | 媒体工具包一键生成 | Free | Step 16 | — |
| **HowLongToBeat** | 玩家社群通关时长数据库（竞品研究用） | Free | Step 1 | — |
| **SteamDB** | Steam数据追踪（愿望单、销售趋势估算） | Free | Step 1, 6, 16 | — |
| **VG Insights / Game Discover Co** | 市场数据/竞品销量估算 | Freemium | Step 1, 6, 16 | SteamDB + 手动收集 |

---

## C.7 分析工具

| 工具 | 用途 | 费用 | 用在哪一步 | 零预算替代 |
|------|------|------|-----------|-----------|
| **Unity Analytics / Godot Analytics** | 引擎内置游戏数据追踪 | Free | Step 7, 16 | 自建 CSV 日志 |
| **GameAnalytics** | 跨引擎免费分析（留存、流失、关卡通过率） | Free | Step 7, 16 | — |
| **PlaytestCloud** | 远程玩家测试（录屏+语音反馈） | Paid | Step 7 | 本地面对面测试 + OBS录屏 |
| **Steam Playtest** | Steam官方免费Playtest功能（Beta分支分发） | Free | Step 7 | — |

---

# 附录D：推荐阅读与引用来源

> **说明：** 以下分为六个分类。标注 ★ 的为本书核心参考书（在正文中频繁引用）。在线资源截至 2026 年 6 月有效；URL 可能变化，搜索资源名称即可找到最新入口。

---

## D.1 游戏设计理论

| 书目 | 作者 | 出版年份 | 推荐理由 |
|------|------|---------|---------|
| ★ ***Rules of Play: Game Design Fundamentals*** | Katie Salen & Eric Zimmerman | 2003 | 游戏设计学术基石。本书第1章、第10-11章频繁引用其"有意义的选择""涌现""魔法圈""信息水平"等核心概念。适合需要理论框架的设计者。 |
| ★ ***Game Design Workshop: A Playcentric Approach to Creating Innovative Games*** | Tracy Fullerton | 2004/2024 (5th Ed.) | 以原型为核心驱动设计教学。本书第5章原型验证的方法论来源之一。第5版更新了独立游戏和移动游戏内容。 |
| ***The Art of Game Design: A Book of Lenses*** | Jesse Schell | 2008/2019 (3rd Ed.) | 100+个"透镜"作为设计的分析视角。本书第10章机制设计的分类法来源。适合设计卡壳时翻一两个透镜换思路。 |
| ***A Theory of Fun for Game Design*** | Raph Koster | 2004/2013 (2nd Ed.) | 薄而精：为什么"学习"是乐趣的核心。2-3小时读完。适合理解"乐趣从哪来"的第一本书。 |
| ***Game Feel: A Game Designer's Guide to Virtual Sensation*** | Steve Swink | 2008 | 唯一专讲"手感"的书。本书第0章"血肉层"的理论来源。适合在意操作手感的动作游戏设计者。 |
| ***Level Up! The Guide to Great Video Game Design*** | Scott Rogers | 2010/2014 (2nd Ed.) | 中文版《通关！游戏设计之道》。本书最重要的技法参考书。详见 D.2。 |
| ***Characteristics of Games*** | George Skaff Elias, Richard Garfield & K. Robert Gutschera | 2012 | 从特性维度分析游戏，补充 *Rules of Play* 的视角。适合有设计经验后回头深读。 |
| ***Homo Ludens*** | Johan Huizinga | 1938 | "魔法圈"概念的原始出处。不是游戏设计书，但帮你理解"玩"在人类文化中的位置。 |

---

## D.2 实践设计方法

| 书目 | 作者 | 出版年份 | 推荐理由 |
|------|------|---------|---------|
| ★ ***Practical Game Design: A Modern and Comprehensive Guide to Video Game Design*** | Adam Kramarzewski & Ennio De Nucci | 2018 | 本书最核心的流程参考书。覆盖七步流程中的具体操作：概念文档、原型、GDD、关卡设计、经济平衡、发布checklist。 |
| ★ ***《通关！游戏设计之道》*** (Level Up!) | Scott Rogers | 2010/2014 | 本书最重要的技法参考书。第6-15关的镜头、关卡、战斗、敌人、道具、多人、计费等章节为本书第10-16章提供大量实操框架。奖励关的模板库是附录B的原始来源。 |
| ★ ***Video Game Design For Dummies*** | Alex Williams | 未标注 | 大道至简的入门指南。本书第3章概念建立、第9章打磨、第16章发布营销的核心简化方法来源。特别适合"不想读300页理论，想马上知道怎么做"的读者。 |
| ***Game Mechanics: Advanced Game Design*** | Ernest Adams & Joris Dormans | 2012 | 用 Machinations 工具可视化模拟游戏经济/资源系统。适合第11章（系统设计）和第15章（平衡设计）的补充阅读。 |
| ***Fundamentals of Game Design*** | Ernest Adams | 2006/2013 (3rd Ed.) | 按游戏类型编写的设计教科书。适合需要快速了解某一类型设计范式的读者。 |
| ***Designing Games: A Guide to Engineering Experiences*** | Tynan Sylvester | 2013 | 《RimWorld》作者写的设计工程方法论。对涌现叙事和系统交互的理解极深。适合做沙盒/模拟/策略类游戏的读者。 |
| ***Spelunky*** (Boss Fight Books) | Derek Yu | 2016 | 不是设计教科书，但作为单人开发者的"全流程实录"极有参考价值。从 Game Maker 原型到 XBLA 到 PC，展示了独立开发的全周期。 |

---

## D.3 入门友好

| 书目 | 作者 | 出版年份 | 推荐理由 |
|------|------|---------|---------|
| ★ ***Video Game Design For Dummies*** | Alex Williams | 未标注 | （见 D.2）最推荐的入门书。如果只读一本入门书，读这本。 |
| ★ ***《通关！游戏设计之道》*** | Scott Rogers | 2010/2014 | （见 D.2）中文化程度最好的游戏设计入门书。幽默、插图多、每个概念都配游戏案例。 |
| ***Reality is Broken: Why Games Make Us Better*** | Jane McGonigal | 2011 | 从心理学和社会学角度解释游戏为何有力量。不是设计工具书，但帮你建立"为什么做游戏有意义"的信念。适合自我怀疑时翻两章。 |
| ***Blood, Sweat, and Pixels*** | Jason Schreier | 2017 | 游戏开发幕后故事集。不是方法论书，但让你知道"所有人都在挣扎"，是独立开发者最好的心理辅导读物。 |
| ***Press Reset: Ruin and Recovery in the Video Game Industry*** | Jason Schreier | 2021 | 同上系列的后续。聚焦游戏行业的人事动荡与职业生存。 |

---

## D.4 关键 GDC 演讲推荐

> **说明：** 以下演讲均可在 GDC Vault (gdcvault.com) 或 YouTube (GDC 官方频道) 找到。部分较老的演讲需要 GDC Vault 会员；大部分近年演讲免费发布在 YouTube。

| 演讲标题 | 演讲者 | 年份 | 主题 | 与本书的关系 |
|---------|--------|------|------|------------|
| **How to Prototype a Game in Under 7 Days** | Kyle Gabler, Kyle Gray, Matt Kucic, Shalin Shodhan (CMU Experimental Gameplay Project) | 2006 | 7天原型方法论：限制时间以激发创造力、零成功率头脑风暴 | 本书第5章（原型验证）核心方法来源 |
| **You Don't Need a Fucking Publisher** | Rami Ismail (Vlambeer) | 2014/2015 | 独立开发者如何不依赖发行商完成从制作到发行的全流程 | 本书第7章（VS产能测算）的"两切片测产能"方法来源；第16章（发布）的独立发行策略 |
| **Prototyping Based Design** | Cliff Bleszinski | 2007 | 以原型为驱动的设计流程：从粗糙到精美的迭代哲学 | 本书第5章（原型验证） |
| **Designing Around a Core Mechanic** | — | GDC 2012 | 从单一核心机制出发构建整款游戏的方法 | 本书第3章（概念孵化）和第10章（核心机制设计） |
| **The Design of Journey** | Jenova Chen (thatgamecompany) | 2013 | 以情绪目标驱动设计：《Journey》的完整设计回顾 | 本书第0章（分析学习/灵魂层）和第12章（叙事设计） |
| **The Art of Celeste** | Maddy Thorson, Noel Berry, Amora Bettany (Extremely OK Games) | 2019 | 从 Game Jam 原型到完整产品的关卡设计、辅助功能设计哲学 | 本书第13章（关卡设计）、附录E案例 |
| **50 Game Camera Mistakes** | John Nesky (thatgamecompany) | 2014 | 镜头设计中被反复踩的50个坑 | 本书第14章（UI/UX设计）及第10章（3C设计） |
| **Practical Techniques for Implementing Emergent Gameplay** | Tynan Sylvester | 2015 | 《RimWorld》的涌现叙事系统设计与实现 | 本书第10章（涌现式设计）和第12章（叙事设计） |
| **Magic: The Gathering — 20 Years, 20 Lessons Learned** | Mark Rosewater (Wizards of the Coast) | 2016 | 从20年卡牌设计中提炼的设计哲学：约束激发创意、少即是多、玩家总能找到你没想到的玩法 | 本书第1章（设计科学）、第11章（系统设计）、第15章（平衡） |
| **Cursed Problems in Game Design** | Alex Jaffe (Riot Games) | 2019 | 某些设计矛盾是无法解决的"诅咒问题"——识别它比硬解决更重要 | 本书第2章（双螺旋/Kill Criteria哲学）——与Kill Criteria的"什么时候该停止"高度共鸣 |

---

## D.5 在线资源

| 资源名称 | 类型 | 网址 | 说明 |
|---------|------|------|------|
| **GDC Vault** | 演讲视频/幻灯片库 | gdcvault.com | GDC历年演讲存档。部分免费，全部需要会员。YouTube 的 GDC 官方频道同步了大量近年演讲。 |
| **Game Developer** (原 Gamasutra) | 行业媒体/Blog | gamedeveloper.com | 游戏开发文章最丰富的英文媒体。搜索任何设计概念都能找到相关实践文章。 |
| **Game Design Skills** | 教学博客 | gamedesignskills.com | Design Pillars 的系统化讲解、原型方法论等实操内容。 |
| **Directing Video Games** | 博客 | directingvideogames.com | 专注游戏制作人视角的实践指南。 |
| **Raph Koster's Website** | 设计师博客 | raphkoster.com | 《A Theory of Fun》作者的持续写作，聚焦游戏设计本质。 |
| **Rami Ismail's Blog & LTPF** | 独立开发者博客 | ltpf.ramiismail.com | Vlambeer 联合创始人的独立开发实战指南。 |
| **GDC YouTube Channel** | 视频 | youtube.com/@GDC | GDC 官方频道，每年免费发布大量演讲录像。 |
| **Game Maker's Toolkit (GMTK)** | YouTube 频道 | youtube.com/@GMTK | Mark Brown 的游戏设计分析频道。适合通过案例理解设计概念。 |
| **Design Doc** | YouTube 频道 | youtube.com/@DesignDoc | 短小精悍的游戏设计分析。 |
| **80.lv** | 行业媒体 | 80.lv | 游戏美术与技术综合媒体，专访和案例丰富。 |
| **HowLongToBeat** | 数据库 | howlongtobeat.com | 玩家通关时长数据库。竞品研究时估算目标体量的重要参考。 |
| **SteamDB** | 数据库 | steamdb.info | Steam 数据追踪。愿望单估算、销量趋势分析。 |
| **itch.io** | 发布平台 / 社区 | itch.io | 独立游戏发布平台，同时也是寻找游戏 Jam 和获取灵感的上佳社区。 |
| **Ludum Dare** | 游戏 Jam | ldjam.com | 最老牌的线上游戏 Jam（48h solo / 72h team）。本书鼓励读者每年参加至少一次游戏 Jam。 |
| **Machinations** | 工具 / 社区 | machinations.io | 游戏经济/系统循环可视化模拟工具，配套社区和教程。 |
| **Ziva.sh** | 独立设计师博客 | ziva.sh | GDD 写作方法论等实操内容。 |

---

## D.6 本书完整引用来源

> 以下按首次在本书中出现的顺序列出全部引用来源。每章末尾的"参考资料"为该章的引用子集。

### 核心参考书

1. Salen, K. & Zimmerman, E. (2003). *Rules of Play: Game Design Fundamentals*. The MIT Press.
2. Kramarzewski, A. & De Nucci, E. (2018). *Practical Game Design: A Modern and Comprehensive Guide to Video Game Design*. Packt Publishing.
3. Williams, A. (n.d.). *Video Game Design For Dummies*. Wiley.
4. Rogers, S. (2010/2014, 2nd Ed.). *Level Up! The Guide to Great Video Game Design*. Wiley. （中文版：孙懿、高济润 译，《通关！游戏设计之道》，人民邮电出版社）
5. Fullerton, T. (2024, 5th Ed.). *Game Design Workshop: A Playcentric Approach to Creating Innovative Games*. CRC Press.

### 学术论文与在线文章

6. Hagen, U. (2009). "Where Do Game Design Ideas Come From? Innovation and Recycling in Games." *Proceedings of DiGRA 2009*.
7. Gabler, K., Gray, K., Kucic, M. & Shodhan, S. (2005). "How to Prototype a Game in Under 7 Days." *Experimental Gameplay Project, CMU Entertainment Technology Center*. GDC 2006. https://www.gamedeveloper.com/game-platforms/how-to-prototype-a-game-in-under-7-days
8. Jenkins, H. (2004). "Game Design as Narrative Architecture." In *First Person: New Media as Story, Performance, and Game*. The MIT Press.
9. Koster, R. (2005/2010). "How to Prototype a Game" / "Fundamentals of Game Design." https://www.raphkoster.com/
10. Pears, M. (2017). "Design Pillars – The Core of Your Game." *Game Developer*. https://www.gamedeveloper.com/design/design-pillars-the-core-of-your-game
11. Game Design Skills (2023). "Game Design Pillars." https://gamedesignskills.com/game-design/design-pillars/
12. Ziva.sh (2026). "How to Write a GDD That You Will Actually Use." https://ziva.sh/blogs/game-design-document
13. Ismail, R. (2022). "Prototypes & Vertical Slice." https://ltpf.ramiismail.com/prototypes-and-vertical-slice/
14. Wayline. "The Vertical Slice Deception: A Pact with the Devil." https://www.wayline.io/blog/the-vertical-slice-deception-a-pact-with-the-devil
15. Ellenor, G. (2014). "Don't Over-Focus on the Vertical Slice." https://gellenor.medium.com/dont-over-focus-on-the-vertical-slice-c304964ed747
16. Cardoso, S. (2026). "The 7 Phases of Game Development." *Game Studio Unlocked*. https://gamestudiounlocked.substack.com/p/game-development-phases-indie-guide
17. Margaris, J. (2025). "Prototyping is Often a Waste of Time." https://jmargaris.substack.com/p/prototyping-is-often-a-waste-of-time
18. Game Developer (2012). "Designing Around a Core Mechanic." https://www.gamedeveloper.com/design/designing-around-a-core-mechanic
19. GDKeys (2024). "Game Development Process." https://gdkeys.com/game-development-process/

### GDC 演讲

20. Gabler, K., Gray, K., Kucic, M. & Shodhan, S. (2006). "How to Prototype a Game in Under 7 Days." GDC 2006.
21. Bleszinski, C. (2007). "Prototyping Based Design." GDC 2007. GDC Vault.
22. Chen, J. (2013). "The Design of Journey." GDC 2013.
23. Ismail, R. (2014/2015). "You Don't Need a Fucking Publisher." GDC 2014 / Independent Games Summit.
24. Nesky, J. (2014). "50 Game Camera Mistakes." GDC 2014.
25. Sylvester, T. (2015). "Practical Techniques for Implementing Emergent Gameplay." GDC 2015.
26. Rosewater, M. (2016). "Magic: The Gathering — 20 Years, 20 Lessons Learned." GDC 2016.
27. Thorson, M., Berry, N. & Bettany, A. (2019). "The Art of Celeste." GDC 2019.
28. Jaffe, A. (2019). "Cursed Problems in Game Design." GDC 2019.

### 游戏案例引用（正文分析中引用，非参考书）

- *Balatro* (LocalThunk, 2024) — Playstack
- *Stardew Valley* (Eric Barone / ConcernedApe, 2016)
- *Celeste* (Maddy Makes Games / Extremely OK Games, 2018)
- *Hollow Knight* (Team Cherry, 2017)
- *Dark Souls* (FromSoftware, 2011)
- *Journey* (thatgamecompany, 2012)
- *Portal* (Valve, 2007)
- *Flappy Bird* (Dong Nguyen, 2013)
- *Tetris* (Alexey Pajitnov, 1984)
- *The Legend of Zelda: Breath of the Wild* (Nintendo, 2017)
- *RimWorld* (Ludeon Studios, 2018)
- *Spelunky* (Derek Yu / Mossmouth, 2008/2013)
- *Hades* (Supergiant Games, 2020)
- *Braid* (Jonathan Blow / Number None, 2008)
- *FTL: Faster Than Light* (Subset Games, 2012)

---

> **附录B/C/D 结束。**
>
> - 附录A（七步速查卡）与附录E（案例研究）参见各自单独文件。
> - 本书所有模板以 CC0 协议授权：可自由复制、修改、用于商业项目，无需署名。

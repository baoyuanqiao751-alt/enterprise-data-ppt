# 风格与预览规范

第2步读取；第3步以本规范生成可比较的图片。参考图存在时先检查实际图片。风格选择不能覆盖已确认的首尾页、正文图标、右上角标识和素材生成设置。

## 风格菜单

| 编号 | 风格 | 主色 / 强调 / 底色 | 设计语言及适用场景 |
|---|---|---|---|
| A | 商务蓝 | #163B66 / #3478DB / #F5F7FB | 白底、大标题、明确网格，正式汇报、提案与项目介绍 |
| B | 科技青 | #075C64 / #16B6BF / #F2FAFA | 青色细线、结构示意、适量深色页，技术方案、科普与数字产品 |
| C | 深色高级 | #111B2B / #D7B56D / #0B1220 | 深海军蓝、克制金色、大字与主视觉，发布会、路演与主题演讲 |
| D | 清新绿色 | #176348 / #79B889 / #F4F8F3 | 浅底、柔和分区、清楚层级，培训教学、自然健康与公益主题 |
| E | 极简黑白 | #20252B / #5F7082 / #FFFFFF | 编辑式排版、细分隔线、大幅作品图，学术、摄影、设计与人文分享 |
| F | 靛紫现代 | #43388B / #9A7BE8 / #F7F5FC | 非对称标题、留白、少量柔和渐变，产品、创意与创新主题 |
| G | 暖灰橙 | #514B45 / #E17E36 / #F8F5F0 | 暖色底、醒目重点、亲近的图文编排，故事、文化、生活与案例教学 |
| H | 主题/品牌定制 | 从Logo、模板、参考图或主题提取 | 可定制学术、童趣、手绘、复古等方向；没有参考时确认主色或描述 |

这是8种起始方向，不是适用主题的限制；按受众和用途推荐1–4种。无偏好时默认组合为A/B/C/D四张，只有用户授权后才生成。不能因为菜单有8项就自动生成8套。各方案在构图、明暗、图文密度、版式节奏和分隔元素上形成差异，保留一致内容；用户要求同样版式仅换色时遵从。

## 每张图片的结构

- 像PowerPoint幻灯片浏览视图：平面正视、多页网格、统一间距、清晰编号；无设备外框、斜透视或浏览器装饰。
- 每个缩略图保持约定比例，默认16:9；整张拼图比例由网格决定，不必与单页相同。
- 12页默认4列×3行；页面主题使用已确认提纲，按用途和首尾配置分配，参考内容规范中的类型框架。
- ≤12页尽量全部展示；>12页默认展示12张代表页，并明确“代表页，非最终总页数”。用户要求全页预览时按总页数调整网格和图片数量。
- 各方案使用同一主题、材料摘录及顺序。数据页只在相关时出现；缺少时间数据时，不编造趋势。
- 代表页覆盖本次真实内容类型：教学可含概念、案例与练习，产品可含场景、功能与演示，故事可含人物、转折与点题，数据分析再含KPI、对比与诊断。只在用户选用时展示独立封面和收尾页，不额外增加页数。
- 标题使用约定语言，默认简短中文，少量辅助英文；减少微小文字。不填入虚构事实、引语、产品能力、研究成果或数字。非数据主题无需填“示意数据”。

## 图标与首尾页一致性

- 内容图标与右上角标识分开控制。无图标模式不添加装饰图标，正常的数据标记、必要的流程或概念图节点不受影响。
- 图标统一线性或面性风格、粗细和尺度；仅用于辅助含义，避免把每句话都配图标。
- 右上角按约定范围、位置、尺寸、页边距执行；正式Logo保留比例，不变形、不生成替代品。预览工具不能准确嵌入时，使用已授权且标明的占位，正式成品替换原件。
- 明确右上角留空时，所有方案都保持留空；各方案不能为了视觉差异擅自增删标识。
- 封面/末页选择原生版式时，预览可以表现该版式，但后续不额外调用模型制作这两页素材。选择生成背景时，才在正式制作阶段生成对应素材。

## 图像提示词骨架

每种方案独立调用，替换所有方括号；无参考图则删除对应行。

```text
Use case: productivity-visual
Asset type: PowerPoint slide-sorter contact sheet
Create ONE image showing [12] consistent [16:9 or agreed aspect ratio] slide thumbnails in a [4-column x 3-row] grid.
Theme: [编号、风格名、色值、字体方向与构图语言].
Audience, subject and purpose: [受众、主题、演示用途与目标].
Ordered slide subjects: [页面主题，顺序与其他方案一致].
Cover and closing configuration: [是否有独立封面、收尾方式、各自原生版式或生成背景；严格遵循总页数].
Content icons: [关闭、少量或指定风格].
Top-right mark: [留空或指定素材/标识；适用页面范围与排版要求].
Verified content and assets: [真实文字摘录、案例、素材或概念；涉及数字时含核实的标签、单位与期间；无关时不添加数据].
Visual references: [已查看的图片及需要继承的元素].
Presentation tone: [适合主题与受众的正式、亲切、学术、活泼或叙事语气].
Intentional whitespace; clear content hierarchy; varied but coherent compositions.
Each slide communicates one main idea with a suitable visual: [diagram, photograph, artwork, illustration, text, or chart only when supported by data].
Short legible headings in [约定语言，默认中文]; auxiliary text only when useful.
Flat front view; equal gutters; no device frame, perspective mockup or fake interactive controls.
This is a visual concept preview. Add no unsupported facts, quotations, product capabilities, research findings, numbers, logos or fabricated claims.
```

## 展示与修改

实际展示图片，图外标清编号、名称和一行差异。文字/数字有偏差时说明仅供选型，正式成品从核实的内容与原始素材重建；影响选型的布局或主题错误应先修复。

“C的布局配A的颜色”：复述组合并生成修订预览；只有用户明确要求直接制作才跳过修订图。已授权修订无需重复询问。

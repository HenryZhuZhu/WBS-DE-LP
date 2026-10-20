# DE-WBS 用户使用手册

**更新日期：2026-10-20**

本手册按日常操作介绍系统功能，界面上的英文名称保持不变，方便查找。**不包含 Fullchip 总览中的“资源跟踪”部分。**

> **使用提醒：** 当前为演示原型。切换项目或表格可以保留本次操作，但刷新、关闭页面后，修改和附件可能丢失。请另外保管正式数据；保存 HTML 文件不等于保存已填写的数据。

## 目录

1. [认识页面与切换表格](#1-认识页面与切换表格)
2. [新建项目与表格](#2-新建项目与表格)
3. [表格中的常用操作](#3-表格中的常用操作)
4. [新增、改名与删除 Block](#4-新增改名与删除-block)
5. [查看和新增 Version](#5-查看和新增-version)
6. [设置负责人、分类与参考项目](#6-设置负责人分类与参考项目)
7. [填写 Schematic](#7-填写-schematic)
8. [填写 Layout](#8-填写-layout)
9. [填写 SPF](#9-填写-spf)
10. [完成检查项](#10-完成检查项)
11. [查看详情与添加材料](#11-查看详情与添加材料)
12. [使用 IO IP 和 Analog IP](#12-使用-io-ip-和-analog-ip)
13. [管理下拉选项](#13-管理下拉选项)
14. [通过 Excel 导入新表](#14-通过-excel-导入新表)
15. [查看总览、延期与修改记录](#15-查看总览延期与修改记录)
16. [常见问题](#16-常见问题)

---

## 1. 认识页面与切换表格

打开系统后，先确认顶部的 **Project（项目）** 和 **WBS 表名**，再开始查看或填写。

左侧有三个主要页面：

| 页面 | 用来做什么 |
|---|---|
| Fullchip 总览 | 看当前表的检查完成情况和延期摘要 |
| WBS Hierarchy | 新增 Block、填写日期、负责人、检查及其他工作信息 |
| Delay 监控 | 查看延期明细，定位需要处理的 Block |

**切换方法：**

- 点击顶部 Project 名称选择项目。
- 点击顶部 ChanEdgel、ChanLeft、ChanMid、LPTOP5 等表名切换表格。
- 在设计类表中，点击 **Schematic / Layout** 切换填写内容。
- SPF 在独立表中维护，默认示例表为 **LPTOP5**。
- IO IP、Analog IP 各有独立表，不在 Schematic/Layout 标签内。

Schematic 和 Layout 使用相同的 Block 列表和版本，但各自的日期与检查分开填写。切换标签只是换一个查看角度，不代表提交或完成工作。

**其他入口：**

- 左侧栏底部按钮：展开或收起侧边栏。
- 右上角用户区：查看当前用户与角色。
- 通知图标：当前仅显示示例通知提示。
- “系统建议”：可展开“提交反馈”“一键入群”；当前尚未连接真实反馈和入群地址。

---

## 2. 新建项目与表格

### 新建项目

1. 点击顶部 Project 旁的 `+`。
2. 输入项目名称，确认创建。
3. 系统进入新项目，再创建需要的表格。

新项目开始时是空的，不复制默认项目的表格、人员和示例数据。项目名称不能为空，也不能与已有项目重名。

### 新建表格

1. 点击顶部 WBS 表名旁的 `+`。
2. 输入新表名称。
3. 选择 **Schematic / Layout** 或 **SPF**。
4. 确认后，系统进入新表，并直接打开第一条 Block 的填写行。
5. 输入 Block 名称后保存；暂时不填可取消，空表仍保留。

**注意：**

- 同一项目内表名不能重复，大小写不同也不能用来区分重名表。
- SPF 表可以有多张，不必都叫 LPTOP5。
- IO IP、Analog IP 不在这里创建；给普通 Block 设置对应分类后，系统会显示相应入口。
- 新建表保存第一条 Block 后，不会自动连续新增下一条。
- 切换项目或表格时，如提示有未保存内容，先决定继续编辑还是放弃。

---

## 3. 表格中的常用操作

| 想做什么 | 怎么操作 |
|---|---|
| 修改单元格 | 鼠标移到单元格或用键盘选中，出现输入框后填写或选择，完成选择或移出输入框后检查结果 |
| 展开/收起下级 | 点击 Block 前的小箭头；没有下级的行不显示箭头 |
| 查找某个 Block | 鼠标移到 Block 列标题，点击筛选按钮，在弹出的搜索框中查找并勾选 |
| 筛选负责人、分类等 | 打开对应列筛选，勾选需要的值，再点击应用 |
| 查看空值 | 在列筛选中选择“空白” |
| 恢复全部数据 | 清除对应列筛选，或恢复全选 |
| 调整列宽 | 拖动表头右边界的竖线 |
| 查看右侧内容 | 在表格内横向滚动，左侧关键列会保持可见 |
| 放大表格 | 点击表格上方最右侧放大图标；点缩小图标或按 Esc 返回 |
| 查看计算说明 | 鼠标移到字段标题旁的说明图标；点击可固定说明 |

**使用筛选时：**

- 同时设置多个筛选，结果必须满足所有条件。
- 日期列和“最近修改”没有普通列筛选。
- 当前没有单独的整页搜索框，找 Block 请使用 Block 列筛选。
- 切换表格会清除筛选。筛选只改变当前展示，不删除数据，也不改变总览的统计范围。
- 看不到某行时，先检查筛选和上级是否收起。

普通单元格修改不需要整页保存，但**新增 Block/Version 的填写行必须点击确认**。输入尚未完成时，不要急着切换页面。

---

## 4. 新增、改名与删除 Block

### 新增 Block

1. 鼠标移到作为位置参照的 Block 行。
2. 点击名称旁的 `+`。
3. 选择 **添加 Block**。
4. 填写 Block 名称，按需填写其他信息。
5. 选择新增位置，确认保存。

| 新增位置 | 保存后在哪里 |
|---|---|
| 同级 | 放在所点 Block 及其全部下级之后 |
| 下一级 | 放在所点 Block 下方，成为它的第一个直接下级 |

Block 名称必填，Version 可暂时不填。新 Block 首次填写 Version 时只能选 1st。到达允许的最深层级后，只能添加同级。

空表可以通过创建入口新增；SPF 顶部一直保留一个空白创建行，点击其中 `+` 即可。

### 修改名称

普通 Schematic/Layout/SPF 中：

1. 点击 Block 名称打开详情。
2. 点击标题旁的铅笔，直接修改标题。
3. 按 Enter 或移出输入框保存，Esc 取消。
4. 有多个 Version 时，按提示确认整组改名。

不允许空名称，也不能造成同一表内“名称、层级、Version 完全相同”的重复记录。Schematic/Layout 的名称会一起更新。

### 删除 Block

1. 鼠标移到目标行，点击名称旁的垃圾桶。
2. 查看提示中的 Block 与 Version。
3. 确认后删除，取消则保留。

**有下级 Block 时，不能直接删除整个上级。** 请先处理下级。Schematic/Layout 的 Block 删除会同时影响两侧，不是只清除其中一侧的内容。

多版本删除方法见下一章；IO/Analog 的删除还会影响来源分类，见第 12 章。

---

## 5. 查看和新增 Version

### 查看已有版本

- 每个 Block 在表格中只显示一行。
- 鼠标移到 Version 单元格，选择已有版本，整行内容随之切换。
- 也可以打开详情，通过顶部版本标签切换。
- Schematic/Layout 同步切换版本；SPF 单独维护。
- 选择旧版只是查看，不会新增或改名。

### 新增版本

1. 点击 Block 行的 `+`。
2. 选择 **添加 Version**。
3. 根据“下一版”提示选择版本。
4. 填写需要的信息，确认保存；取消会返回原版本。

只能按 **1st → 2nd → 3rd → 4th → 5th** 往后新增，以该 Block 已有的最高版为准。

例如：已有 1st、2nd、3rd，即使正在查看 1st，下一版仍是 4th。达到 5th 后不能继续新增。已有非空版本标签不能直接改成其他版本。

新版本沿用原 Block 的层级和负责人，其他业务内容保存后请重新核对，不要假定旧版日期和检查全部复制。

### 删除版本

多版本 Block 点击垃圾桶后，可以选择要删除的版本，但必须**从最高版开始连续向下选**。

例如已有 1st–4th：

- 可以删 4th，或 4th、3rd；
- 不能只删 2nd，也不能跳过 3rd 删除 4th、2nd；
- 选中全部版本等于删除整个 Block，需确认且不能有下级；
- 删除当前显示版后，系统显示最早的剩余版。

Excel 导入的历史版本可能不连续，这是允许的。IO/Analog 中暂时隐藏的版本也可能占用版本名额，不能靠隐藏绕过新增和删除限制。

---

## 6. 设置负责人、分类与参考项目

| 字段 | 如何填写 | 需要注意 |
|---|---|---|
| Schematic Owner | 搜索并选择设计负责人 | 与 Layout Owner 分开维护 |
| Layout Owner | 搜索并选择版图负责人 | 与 Schematic Owner 分开维护 |
| Block Category | 搜索并选择已有分类 | 选择 IO IP/Analog IP 会让对应版本进入特殊表 |
| Reference project | 搜索并选择已有参考项目 | 不会自动复制参考项目的数据 |

**新增负责人：** 搜索不到姓名时，确认输入无误，再点击 **新增并使用**。清空可取消分配。

**新增分类或参考项目：** 不能直接在单元格里创建，请到 **WBS字段配置** 新增，再回来选择。

**几个重要规则：**

- 同一 Block 的各 Version 共用 Schematic Owner，也共用 Layout Owner；修改任意版，会同步该角色到其他版。
- 两种负责人相互独立，修改设计负责人不会自动改版图负责人。
- 同一项目的表格共用可选名单；不同项目分开。
- SPF 有两种 Owner，但没有 Block Category、Reference project。
- IO/Analog 可以填写 Reference project 和两种 Owner，但不再显示 Block Category 列。

---

## 7. 填写 Schematic

进入设计类表，点击 **Schematic**，按以下顺序更新：

1. 确认 Block 和 Version。
2. 设置 Schematic Owner、Block Category、Reference project。
3. 填 **Planned release**（计划日期）。
4. 按实际结果勾选 **Check item**。
5. 实际完成释放后，填 **Actual release**。
6. 核对状态，必要时在详情补充材料和备注。

### 日期与状态

| 字段 | 使用说明 |
|---|---|
| Planned release | 默认锁定；空值可首次填写，已有日期修改通常需 PL/LPL 解锁 |
| Actual release | 填真实释放日期，可清空 |
| Schematic Progress | 系统计算，不能手选 |
| Schematic check status | 五项检查全部完成为 Done，否则 Ongoing |
| Layout Progress | 查看对应 Layout 排期状态，不能在这里手填 |

Progress 的显示规则：

- 没有计划日期：**Not started**；
- 实际日期晚于计划：**Delay**；
- 其他情况：**On schedule**。

> **注意：** 实际日期没填时，当前不会因为“今天已过计划”就自动显示 Delay。On schedule 不等于工作已经完成。

需要修改已有 Planned release 时，请按团队要求让 PL/LPL 解锁，修改后重新锁定。当前原型锁定时仍允许清空再填，不应把它当作正式审批。

五项检查为 Power mapping、ERC、Fanout、CN marker、Verification (Verilog & Finesim)。

---

## 8. 填写 Layout

进入设计类表，点击 **Layout**：

1. 确认 Block、Version，设置 Layout Owner。
2. 填 **Plan workdays**（计划工作天数）。
3. 填 **Resource**，默认值为 1。
4. 填 **Start date**（开始日期）。
5. 查看系统生成的 **Plan finish**。
6. 完成后填 **Actual finish**，并更新检查项。
7. 实际工作天数 **Actual workdays** 在 Block 详情中维护。

### 自动完成日期

**Plan finish 由开始日期、计划工作天数和 Resource 自动计算，不能直接修改。**

简单理解：计划工作天数 ÷ Resource 得到所需天数，再按中国工作日往后计算，跳过休息日、包含调休补班。

例如：10 天 ÷ 2 = 5 个工作日。

如果 Plan finish 为空，请检查：

- 开始日期、计划工作天数是否已填；
- 计划工作天数是否为非负整数；
- Resource 是否为有效正数；
- 相除后是否出现小数天数，例如 5 ÷ 2 = 2.5，目前暂不计算；
- 所需年度的工作日历是否可用。

清空开始日期后，自动完成日期也会清空。

### 状态与检查

- 没有 Plan finish：Not started；
- Actual finish 晚于 Plan finish：Delay；
- 其他情况：On schedule。

四项 Layout 检查全部完成，Layout check status 才显示 Done：

Floorplan Reviewed、IO 满足上层需求、Power 合理并满足上层需求、Verification (DRC/LVS)。

请按实际情况并与 KR 确认后勾选。当前没有额外的 KR 审批按钮。Layout 的日期为开始/完成日期，不是 release 日期。

---

## 9. 填写 SPF

选择 **LPTOP5** 或其他 SPF 表：

1. 确认 Block 和 Version。
2. 填 Schematic Owner、Layout Owner。
3. 填 **LVS path、cdl、gds**。
4. 填 **Planned SPF release**。
5. 完成对应检查后勾选 Check item。
6. 实际发布后填 **Actual SPF release**。

五项 SPF 检查为：UT DRC、MRC / shielding check、LN net、LRC、Duplicate pin。全部完成后，SPF check status 显示 Done，否则为 Ongoing。

SPF 独立维护，不会自动复制普通设计表的 Block、版本或检查。LVS path、cdl、gds 目前由用户填写，系统不会自动验证文件是否存在或内容是否正确。

---

## 10. 完成检查项

检查可以在 **WBS 表格、Block 详情、Fullchip 的 Check item 明细**中更新，三个位置的结果同步。

### 上级为什么不能勾完

如果点击某一项会让上级 Block 的所有检查都完成，系统会先检查它的直接下级。

1. 下级未全部完成时，弹窗列出需要处理的 Block 和未完成项。
2. 点击弹窗中的 Block 名称，打开详情处理。
3. 下级完成后，再回来完成上级最后一项。

已完成的下级重新取消检查时，已完成的上级也会重新变为未完成，避免仍显示全部完成。

### 同名 Block 的提示

不同层级可能有同名 Block。修改检查时，系统可能询问：

- **仅当前 Block**：只修改当前对象；
- **同步其他层级**：一起修改提示中列出的同名 Block。

请核对名单再选择，不要默认全部同步。

**新增下级后的提醒：** 当前仍需人工复核上级检查，确认原来的完成标记是否继续成立。

---

## 11. 查看详情与添加材料

点击 Block 名称打开右侧详情。先核对名称与 Version；多个版本可用上方标签切换。切换表格或主页面后，旧详情会关闭。

普通 Block 详情可以查看或维护对应日期、检查、实际工作天数等内容。

### AI Routing

在 Back up 上方选择 **Yes / No**。当前只保存选择，不会启动自动布线或其他 AI 任务。

### Materials 与 Comments

在 **Materials** 分组中可以：

- 写文字说明；
- 填 HTTP/HTTPS 链接，点击打开；
- 上传多个 PPT/PPTX、XLS/XLSX、DOC/DOCX 附件；
- 点击附件打开或下载，点 `×` 移除。

**Comments** 在 Materials 外，用于填写备注。当前附件不会永久保存，请另外保管原文件。

### IO/Analog 详情的区别

- IO IP：大部分内容只读，**Review AI** 可以在详情的多行文本框编辑，移出后保存。
- Analog IP：详情用于查看，需要修改时回到表格。
- IO 的 Review AI 只是文字记录，不会自动生成 AI 分析；它与 AI Routing 不是同一个功能。

---

## 12. 使用 IO IP 和 Analog IP

### 让 Block 进入对应表

1. 回到普通设计表，选好 Block 和 Version。
2. 将 **Block Category** 设为 **IO IP** 或 **Analog IP**。
3. 保存后，点击顶部对应表名。
4. 核对 **Source（来源表）**、Block 路径和 Version，再填写流程信息。

只会加入所选分类的版本。例如 1st 为 IO IP、2nd 分类为空，查看来源 2nd 不会自动把它也加入 IO 表。

没有相关记录时，对应表入口可能隐藏；默认示例项目已有记录，所以通常可以直接看到。

### 阅读 Block 与来源

- 来源 Block 可以显示为 `T1 CE_TOP/T2 CORE_ARRAY/T3 BITCELL`，方便查找原位置。
- 路径太长时显示省略号；移到名称上、键盘选中或打开详情可看全文。
- 拉宽 Block 列可显示更多内容，但不会无限拉宽。
- Source 会把连续相同来源合并显示。手工新增的 Block 本身没有来源，不会因此自动变成普通表的记录。
- 特殊表的展开箭头只控制实际手工添加的下级，不会把路径中另一个独立来源 Block 一起收起。

### IO IP 填写内容

按表格分组逐步填写：

| 分组 | 主要操作 |
|---|---|
| Hookup、Spec&Reviewb | 填 Deadline 和 Status |
| Pre_sim result CRC review | 填 Deadline、流程状态、Review AI 文字及对应状态 |
| SCH release for Layout | 填计划和实际完成日期，Status 自动计算 |
| Schematic and Layout Co-work flow Check | 填邮件确认、Floorplan、Layout 状态、Routing 检查等 |
| Layout finish status | 填计划和实际完成日期，Status 自动计算 |
| Layout modify email E3 | 选择 Yes、No 或空白 |
| Layout quality check | 填检查负责人、Deadline、Status |
| Post_sim result CRC review | 填 Deadline 和 Status |

Review AI 长文字可在单元格预览，也可进入详情编辑。Layout routing check with design 当前直接填文字。

### Analog IP 填写内容

| 分组 | 主要操作 |
|---|---|
| Release for layout drawing | 填计划、实际日期及状态文字 |
| Schematic and Layout Co-work flow Check | 填邮件、Floorplan、Routing 确认 |
| Layout finish status | 填计划和实际完成日期，Status 自动计算 |
| Layout modify email E3 | 选择 Yes、No 或空白 |
| Layout quality check | 填检查负责人、Deadline、Status |
| DC EM | 填 Deadline 和 Status |
| PDC share & CM description | 选择状态 |
| Spf-sim finish review | 填计划和实际完成日期，Status 自动计算 |
| Comment | 填结论或备注 |
| All check done & final review | 填计划和实际完成日期，Status 自动计算 |

### 怎样填写状态

- 普通流程状态可选空白、Ongoing、Done、Ongoing（delay）。
- 邮件确认等字段可选空白、Yes、No。
- 自动日期状态：两日期都填后，实际晚于计划为 Delay，否则为 On schedule；缺任一日期时为空。
- Analog 的 Release for layout drawing Status 当前是手填文字，不自动计算。
- E3 的 Yes/No 只表示该字段选择，不会新增、删除 Block 或触发其他行操作。

### 来源修改会怎样

来源普通表真正修改名称、参考项目或负责人时，对应内容会单向更新到特殊表。普通表的检查和日期不会自动复制为特殊表各流程的检查和日期。

在特殊表修改内容不会反向更改普通表；只切表或查看已有版本，也不会重新覆盖特殊表里已填的工作内容。

如果特殊表本地改过参考项目等公共内容，之后来源又真正修改了同一字段，特殊表该字段会跟随来源更新。

### 暂时移出与删除的区别

| 你想做什么 | 正确操作 | 结果 |
|---|---|---|
| 暂时不在 IO/Analog 跟踪 | 回来源表修改对应 Version 的 Category | 隐藏并保留已填数据；改回分类可恢复 |
| 确实不要这份特殊表记录 | 点击特殊行垃圾桶并确认 | 删除工作内容；来源分类恢复到本次进入前的值 |

暂时移出时，同组还有其他有效版本就保留它们；整组都移出时，手工下级也一起隐藏保留，不必先删除下级。IO 和 Analog 的工作内容分别保留，不会互相转换。

**主动删除后再加入，会得到新的空白工作内容，不是恢复旧数据。** 有实际手工下级时不能直接删除整个上级。多版本删除按系统提示处理，并在完成后核对剩余版本和来源分类。

### 在特殊表中新增

已有行旁的 `+` 同样提供“添加 Version / 添加 Block”：

- 新版本沿用当前 Block 信息，流程内容从空白开始；
- 新 Block 可以添加同级或下一级；
- 本地新增不会在普通表自动新增 Block 或 Version。

---

## 13. 管理下拉选项

**入口：WBS Hierarchy → WBS字段配置。**

页面中分别管理 **Block Category** 和 **Reference project**，点击“返回 WBS Hierarchy”返回表格。

| 操作 | 使用方法 |
|---|---|
| 新增 | 点对应新增按钮，填名称并确认，再回表格选择 |
| 重命名 | 点击目标选项的重命名操作，输入新名称并确认 |
| 删除未使用选项 | 点击删除并确认 |
| 删除正在使用的选项 | 先选另一个已有选项替换，再确认 |

**注意：**

- 配置影响当前项目的所有适用表，不只影响正在看的这一张。
- 使用数量可能包含其他表和多个版本，不等于当前屏幕行数。
- IO IP、Analog IP 为系统保留选项，不能改名或删除。
- 重命名或替换会同步当前数据，但不会把过去修改记录中的旧文字全部改写。
- 负责人不在此页面管理，在 Owner 单元格中使用“新增并使用”。
- 操作失败时按提示重试，不要反复点击确认。

---

## 14. 通过 Excel 导入新表

**导入只创建新表，不会追加或覆盖已有表。**

### 操作步骤

1. 确认当前 Project，点击 **导入 Excel 表格**。
2. 选择 Schematic / Layout 或 SPF，填写新表名称。
3. 下载对应模板。
4. 按模板填写，保留原 Sheet 名称、完整表头和列顺序。
5. 点击“选择已填写模板”，上传 `.xlsx` 或 `.xls`。
6. 等待读取后，点击 **导入并创建新表**。
7. 成功后直接进入新表；失败时按页面列出的 Sheet、行号、字段和原因修改，重新上传。

| 选择类型 | 下载模板 | 填写要求 |
|---|---|---|
| Schematic / Layout | WBS_Schematic_Layout_Import_Template.xlsx | 保留 Schematic、Layout 两张表；可以只填一侧，另一侧保留表头 |
| SPF | WBS_SPF_Import_Template.xlsx | SPF 至少填写一条 Block |

不要使用旧的三类业务混合模板，也不要额外增加业务 Sheet。切换导入类型后，需重新上传对应文件。

### 填写要点

- 每行填写一个 Block，放在对应的 Tier 列；上级必须排在下级前面。
- 设计表支持 Tier1–Tier6，SPF 支持 Tier1–Tier4。
- Version 必填，只能用 1st–5th；允许历史版本不连续。
- 同一张表内名称、层级、Version 完全相同的记录不能重复。
- 分类、参考项目和 Owner 必须已在当前项目中登记；未知选项先在系统中新增。
- 日期填 `YYYY-MM-DD`；工作天数填整数，Resource 填有效数值。
- 检查完成可填 `1`、Yes、Done 或 `✓`；未完成填 `0`、No 或留空。
- Schematic/Layout 相同 Block 的上级、分类和参考项目不要相互矛盾。
- Layout 的 Plan finish 仍按系统公式计算，不由 Excel 手填值覆盖。

第一次下载或上传可能需要联网加载 Excel 组件。加载失败时检查网络后重试，**不要优先刷新整个页面，以免丢失已编辑内容**。

---

## 15. 查看总览、延期与修改记录

### Fullchip 总览

先选好顶部表名，再进入 Fullchip。这里显示的是**当前所选表**的结果，不是所有项目、所有表的合计。

- 设计表：显示 Schematic/Layout 检查完成与 Delay。
- SPF 表：显示 SPF 检查完成与 Delay。
- IO/Analog：显示两侧 Delay，并在卡片内列出各 Source 的数量。

**检查完成数**表示检查全部完成的记录数量；**Check item 进度**表示已完成检查项占全部检查项的比例。状态和百分比由填写结果计算，不手工输入。

普通设计/SPF 总览可能统计同一 Block 的多个版本，因此数量不一定等于表格可见行数。

“需要关注”显示部分延期摘要，“查看全部”进入完整 Delay 页面。“刷新状态”用于重算显示，不是保存业务数据。

### Check item 明细

1. 在 Fullchip 的 Check item 进度中点击某一行，或点击“查看全部”。
2. 选择对应 Schematic、Layout 或 SPF。
3. 用列筛选定位 Block。
4. 直接点击检查方格更新；点击 Block 名称可打开详情复核。

这里每个 Block 显示当前选中的版本，**只有检查方格可直接修改**，其他文字只供查看。要切换版本或改负责人，请回 WBS 对应入口。

### Delay 监控

1. 点击左侧 Delay 监控。
2. 选择 Schematic Delay、Layout Delay 或 SPF Delay。
3. IO/Analog 可再选择 Source。
4. 查看计划、实际和延误天数，点击查看 Block 的操作打开详情。

当前自动 Delay 的判断是：**计划与实际日期都有值，且实际晚于计划。** 未填实际日期不会仅因超过今天而自动计入，手选 Ongoing（delay）也不会直接计入自动延期。

延误天数按实际日期减计划日期计算，按日历天显示；列表默认从延误最多的开始排列。

IO/Analog 还需注意：

- 每个 Block 只按最高的有效版本统计，不受当前正在查看哪一版影响。
- 新版日期为空，不会继承旧版 Delay；暂时隐藏的版本不计入。
- IO 的 SCH release for Layout 属于 Schematic Delay，Layout finish 属于 Layout Delay。
- Analog 的 Spf-sim finish review 属于 Schematic Delay；Layout finish、final review 属于 Layout Delay。
- 同一个 Analog Block 两个 Layout 阶段都延期时，卡片算一个 Block，明细可以列两行。
- 选择 Source 会缩小 Delay 明细范围，切回“全部 Source”恢复查看；不改变总览的合计。

### 最近修改与 Block变更记录

| 想查看什么 | 入口 |
|---|---|
| 当前版本最近改了什么 | 鼠标移到该行，点击“最近修改”列的时钟 |
| 更多行修改记录 | 弹出的记录中点击“查看全部修改记录” |
| 新增、删除 Block/版本等变化 | 点击“最近修改”表头中的 Block变更记录图标 |

行记录显示操作人、修改字段、前后值和时间，默认最新五条，可查看更多至二十条。“最近修改”列可收起，再通过边缘箭头展开。

普通表只记录部分字段，例如负责人、分类和计划日期等，**不是每次编辑都会出现在这里**；没有记录不代表没有改过。IO/Analog 的直接编辑按对应记录查看。

---

## 16. 常见问题

| 遇到的情况 | 怎么处理 |
|---|---|
| 找不到某个 Block | 确认项目和表名，清除列筛选，展开上级，再检查版本 |
| ChanEdgel 没有 SPF 标签 | 切换到 LPTOP5 或其他 SPF 表 |
| 新项目里没有默认表 | 先新建表，或使用 Excel 导入 |
| 找不到 IO/Analog 表 | 在普通表正确版本上保存对应 Category |
| 想新增分类但单元格没反应 | 到 WBS字段配置新增；输入陌生文字不会自动创建 |
| 改一个版本的负责人，其他版本也变了 | 正常行为，同一 Block 各版共用对应负责人 |
| Plan finish 为空 | 检查开始日期、整数工作天数、正数 Resource、小数天数及日历提示 |
| 计划已过，但没有 Delay | 当前要填了实际日期且晚于计划才计入，请另外关注未完成工作 |
| 检查全完成，仍显示 Delay | 检查完成与日期延期是两回事，核对真实日期即可 |
| 上级最后一项无法勾选 | 按弹窗处理未完成的下级检查 |
| 删除提示还有下级 | 先处理下级；不要为了隐藏特殊记录而删除整组 |
| IO/Analog 改回分类后旧内容又出现 | 分类移出是隐藏保留；这与主动删除不同 |
| 不能新增某个版本或单删中间版 | 按最高版的下一版新增，删除从最高版连续向下选 |
| 路径显示省略号 | 移到名称上查看全文，或打开详情 |
| Excel 报错 | 按 Sheet、行号、字段修正；保留模板结构，并先登记候选选项 |
| Excel 组件加载失败 | 检查网络后重试，避免直接刷新丢失数据 |
| 详情提示对象已变化 | 从当前表重新打开目标 Block |
| 刷新后修改或附件不见了 | 当前是演示原型，请另行保管正式数据 |

**建议每次结束操作前：** 再核对项目、表名、Block 和 Version，确认日期与检查正确。遇到异常先记录提示和截图，不要通过随意删除或填写不真实日期来消除提示。

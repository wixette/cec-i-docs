# 中华学习机 CEC-I 历史文献数字化工程 (CEC-I Manuals Digitalization)

本项目旨在抢救性数字化并永久保存 20 世纪 80 年代末在中国普及率极高（累计销量约 300 万台）的经典八位微机——**中华学习机 (CEC-I, China Educational Computer)** 的四部核心原始技术手册与专著。

原始扫描 PDF 存放于 `scanned_oringinal_docs/`（由 `.gitignore` 忽略），数字化后的现代 Markdown 文档与插图存放于 [`docs/`](docs/) 目录下。

---

## 书籍目录 (Books Catalog)

| 编号 | 书名 | 出版社 / 年份 | 页数 | 数字化目录 | 状态 |
| :--- | :--- | :--- | :---: | :--- | :--- |
| **01** | **《CEC-I 型中华学习机用户使用手册》** | 电子工业出版社 (1988年9月第2版) | 265 | [`docs/01-user-manual/`](docs/01-user-manual/README.md) | ✅ 100% 完成 (8,312行, 33图) |
| **02** | **《中华学习机系统原理使用及维修》** | 清华大学出版社 (邵祖英、王秉湖、付强、高小华 编著) | 269 | [`docs/02-system-principles-maintenance/`](docs/02-system-principles-maintenance/README.md) | ✅ 100% 完成 (全9章+附录图样, 46图) |
| **03** | **《中华学习机 CEC-I 技术参考手册（软件）》** | 清华大学出版社 (中华学习机联合设计组 编) | 306 | [`docs/03-software-reference/`](docs/03-software-reference/README.md) | ✅ 100% 完成 (全5部分9篇, 6,342行, 121图) |
| **04** | **《中华学习机 CEC-I 技术参考手册（硬件）》** | 清华大学出版社 (中华学习机联合设计组 编) | 227 | [`docs/04-hardware-reference/`](docs/04-hardware-reference/README.md) | ✅ 100% 完成 (全3章+附录图样, 4,309行, 118图) |

---

## 仓库目录结构 (Repository Structure)

```text
cec-i-manuals/
├── README.md                                  # 项目总览与书籍导航
├── scanned_oringinal_docs/                    # 原始扫描 PDF（Git 忽略）
└── docs/
    ├── 01-user-manual/                        # 《CEC-I 型中华学习机用户使用手册》
    │   ├── README.md                          # 版权信息与全书总目录
    │   ├── ch01-introduction.md               # 第一章 CEC-I 中华学习机简介
    │   ├── ch02-operation.md                  # 第二章 CEC-I 中华学习机的操作使用
    │   ├── ch03a-basic-part1.md               # 第三章 CEC-BASIC 语言程序设计（3.1~3.5 基础）
    │   ├── ch03b-basic-part2.md               # 第三章 CEC-BASIC 语言程序设计（3.6~3.8 绘图与声音）
    │   ├── ch03c-basic-part3.md               # 第三章 CEC-BASIC 语言程序设计（3.9 向量作图）
    │   ├── ch04a-logo-part1.md                # 第四章 CEC-LOGO 语言程序设计（4.1~4.3 基础与作图）
    │   ├── ch04b-logo-part2.md                # 第四章 CEC-LOGO 语言程序设计（4.4~4.7 过程与声音）
    │   ├── ch05-monitor-assembler.md          # 第五章 监控系统和小汇编系统的使用
    │   ├── ch06-disk-files.md                 # 第六章 程序中磁盘文件的使用
    │   ├── ch07-printer.md                    # 第七章 打印机输出控制
    │   ├── appendices-1-6.md                  # 附录 1 ~ 附录 6（基础数据、ASCII、保留字、错误表）
    │   ├── appendices-7-11.md                 # 附录 7 ~ 附录 11（6502指令、软开关、常用子程序）
    │   └── images/                            # 裁剪清理后的原书插图与接口图（33幅）
    ├── 02-system-principles-maintenance/      # 《中华学习机系统原理使用及维修》
    │   ├── README.md                          # 版权信息与全书总目录
    │   ├── ch01-02-fundamentals.md            # 第一章 概述 & 第二章 计算机基本知识
    │   ├── ch03a-6502-part1.md                # 第三章 微处理器 6502 及其指令系统（前半）
    │   ├── ch03b-6502-part2.md                # 第三章 微处理器 6502 及其指令系统（后半与程序举例）
    │   ├── ch04a1-motherboard-part1a.md       # 第四章 主板工作原理（§4-1~§4-3 主板框图/CPU/存储器）
    │   ├── ch04a2-motherboard-part1b.md       # 第四章 主板工作原理（§4-4~§4-6 时钟/扩展槽/键盘）
    │   ├── ch04b-motherboard-part2.md         # 第四章 主板工作原理（§4-7~§4-12 各外设接口与汉字电路）
    │   ├── ch05-monitor.md                    # 第五章 监控程序原理
    │   ├── ch06-dos.md                        # 第六章 DOS 磁盘操作系统原理
    │   ├── ch07-editor-assembler.md           # 第七章 编辑汇编系统
    │   ├── ch08a-display-part1.md             # 第八章 显示器接口电路原理与维修
    │   ├── ch08b-display-printer-part2.md     # 第八章 打印机接口电路原理与维修
    │   ├── ch09-maintenance-schematics.md     # 第九章 整机维修 & 附录全套母板折页电路原理图
    │   └── images/                            # 裁剪清理后的芯片引脚、逻辑图与折页原理图（46幅）
    ├── 03-software-reference/                 # 《中华学习机 CEC-I 技术参考手册（软件）》
    │   ├── README.md                          # 版权信息与全书总目录
    │   ├── part1a-basic-ch01-ch03a.md         # 第一部分 CEC-BASIC（特点、变量规则与 3.1~3.5 语句）
    │   ├── part1b-basic-ch03b.md              # 第一部分 CEC-BASIC（3.6~3.10 绘图、向量作图与命令）
    │   ├── part1c-basic-appendices.md         # 第一部分 附录 A ~ 附录 G（出错、保留字内码、参考卡）
    │   ├── part2-monitor.md                   # 第二部分 系统监控（命令全集、结构分析与小汇编）
    │   ├── part3a-dos-ch01-ch03a.md           # 第三部分 DOS 磁盘操作系统（引言、引导与基础命令）
    │   ├── part3b-dos-ch03b-ch04-app.md       # 第三部分 DOS 磁盘操作系统（文本/二进制文件与实用程序）
    │   ├── part4-chinese-system.md            # 第四部分 CEC 汉字系统（输入法、内码、子程序调用与框图）
    │   ├── part5a-dos-analysis-ch01-ch03.md   # 第五部分 DOS 3.3 分析报告（引导链、VTOC 表与命令扫描）
    │   ├── part5b-dos-analysis-ch04-ch05-app.md # 第五部分 DOS 3.3 分析报告（文件管理、软驱与 GCR 驱动）
    │   └── images/                            # 裁剪清理后的系统框图、波形图与程序流程图（121幅）
    └── 04-hardware-reference/                 # 《中华学习机 CEC-I 技术参考手册（硬件）》
        ├── README.md                          # 版权信息与全书总目录
        ├── ch01-ch02-intro-operations.md      # 第一章 简介 & 第二章 操作指南（系统连接、自检与LOGO）
        ├── ch03a-motherboard-cpu-memory-io.md # 第三章 硬件介绍（3.1~3.4 主板框图、CPU、存储系统与I/O）
        ├── ch03b-display-circuits.md          # 第三章 硬件介绍（3.5 字符/图形显示电路原理与PAL色度调制）
        ├── ch03c-interfaces-asic.md           # 第三章 硬件介绍（3.6~3.13 键盘/录音机/软驱/汉字/ASIC/打印机）
        ├── appendices-instruction-set-schematics.md # 附录 A~D（指令表、显示码表与整机逻辑电路图纸）
        └── images/                            # 裁剪清理后的波形时序图、ASIC结构与全页电路图纸（118幅）
```

## 数字化规范 (Digitalization Standards)

1. **忠实原文与勘误标注**：严格对照原书扫描页逐页核对。原书明显排印错误（如将启动提示写成 `ZHON HUA XUE XI JI`）保留原貌或以注释形式说明。
2. **结构化排版**：
   - 章节标题统一映射为 Markdown 多级标题（`#`、`##`、`###`）。
   - 引脚定义、内存映射、指令集、对照表统一转换为标准 Markdown 表格。
   - BASIC、LOGO、6502 汇编程序及屏幕输出统一使用代码块（Fenced Code Blocks）。
3. **插图与框图处理**：
   - **外观图、连接示意图、复杂原理图**：从高清扫描页精确裁剪并清理，保存在各书 `images/` 目录下。
   - **逻辑框图、流程图、引脚对照**：除保留原图外，提供重绘的 ASCII/Mermaid 框图或结构化引脚表，方便检索与现代阅读。

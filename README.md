# 中华学习机 CEC-I 历史文献数字化工程 (CEC-I Manuals Digitalization)

本项目旨在抢救性数字化并永久保存 20 世纪 80 年代末在中国普及率极高（累计销量约 300 万台）的经典八位微机——**中华学习机 (CEC-I, China Educational Computer)** 的四部核心原始技术手册与专著。

原始扫描 PDF 存放于 `scanned_oringinal_docs/`（由 `.gitignore` 忽略），数字化后的现代 Markdown 文档与插图存放于 [`docs/`](docs/) 目录下。

---

## 书籍目录 (Books Catalog)

| 编号 | 书名 | 出版社 / 年份 | 页数 | 数字化目录 | 状态 |
| :--- | :--- | :--- | :---: | :--- | :--- |
| **01** | **《CEC-I 型中华学习机用户使用手册》** | 电子工业出版社 (1988年9月第2版) | 265 | [`docs/01-user-manual/`](docs/01-user-manual/README.md) | 🚧 样章已完成 (Ch.1 + Ch.2.1–2.3) |
| **02** | **《中华学习机系统原理使用及维修》** | 清华大学出版社 (邵祖英、王秉湖、付强、高小华 编著) | 269 | [`docs/02-system-principles-maintenance/`](docs/02-system-principles-maintenance/) | ⏳ 待处理 |
| **03** | **《中华学习机 CEC-I 技术参考手册（软件）》** | 清华大学出版社 (中华学习机联合设计组 编) | 306 | [`docs/03-software-reference/`](docs/03-software-reference/) | ⏳ 待处理 |
| **04** | **《中华学习机实用大全 2：汉字处理与数据库技术》** | 电子工业出版社 (1990年，韩仲清 主编) | 373 | [`docs/04-chinese-processing-database/`](docs/04-chinese-processing-database/) | ⏳ 待处理 |

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
    │   ├── ch03-basic.md                      # 第三章 CEC-BASIC 语言程序设计
    │   ├── ch04-logo.md                       # 第四章 CEC-LOGO 语言程序设计
    │   ├── ch05-monitor-assembler.md          # 第五章 监控系统和小汇编系统的使用
    │   ├── ch06-disk-files.md                 # 第六章 程序中磁盘文件的使用
    │   ├── ch07-printer.md                    # 第七章 打印机输出控制
    │   ├── appendices.md                      # 附录 1 ~ 附录 11
    │   └── images/                            # 裁剪清理后的原书插图与电路/接口图
    ├── 02-system-principles-maintenance/      # 《中华学习机系统原理使用及维修》
    │   ├── README.md
    │   └── images/
    ├── 03-software-reference/                 # 《中华学习机 CEC-I 技术参考手册（软件）》
    │   ├── README.md
    │   └── images/
    └── 04-chinese-processing-database/        # 《中华学习机实用大全 2：汉字处理与数据库技术》
        ├── README.md
        └── images/
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

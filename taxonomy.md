# 顶层分类与归属规则

本文说明十条知识域从何而来、如何对照公开课程体系，以及跨域内容怎么归主归属。

## 设计原则（摘要）

- 知识在前，资料在后；资料有独立主档，主题页只引用。
- 树是分类，路径是视图；学习顺序不做成目录树。
- 由广及深四层（L0–L3）；当前只填到 L1，并列出 L2 子类名称。
- 目录英文短横线，标题和正文中文，术语保留英文。
- **一个概念一个主归属**：跨域内容在主归属页写，其他域用链接指过去。

## 十条域

| 编号 | 目录 | 名称 | 边界摘要 |
|------|------|------|----------|
| 01 | `01-computing-foundations` | 计算基础 | 最小数学与信息表示；不收通用数学课 |
| 02 | `02-algorithms` | 算法与数据结构 | 复杂度与设计范式；不放具体语言的 STL |
| 03 | `03-computer-systems` | 计算机系统 | 组成、OS、网络协议栈主归属、并发与内存 |
| 04 | `04-programming-languages` | 编程语言 | 语言本身；不是框架教程库 |
| 05 | `05-software-engineering` | 软件工程 | 可维护软件；设计模式归这里 |
| 06 | `06-data-systems` | 数据系统 | 建模、关系库、事务、NoSQL、数据工程入门 |
| 07 | `07-internet-applications` | 互联网与应用 | Web/浏览器/前后端/移动；HTTP 协议机制链回 03 |
| 08 | `08-infrastructure` | 基础设施与分布式 | Linux、容器、云、分布式、可观测性 |
| 09 | `09-security` | 安全 | 攻防与工程化安全；不做漏洞利用手册 |
| 10 | `10-artificial-intelligence` | 人工智能 | ML/DL/任务地图/大模型工程；MLOps 主归属在此 |

刻意不升为顶层：性能优化、开源协作、面试与职业、区块链、游戏、嵌入式。挂到最接近的域（嵌入式 → 03，区块链共识 → 08），或必要时写进 `00-map/`。

## 分类依据与对照

没有一份公开分类正好用这十个名字。这十条是把 **CS2023** 的 17 个知识域折叠后，再用自学路线和从业路线补上「互联网应用」和「基础设施」。下列合并是本图谱的判断，不是原文。

### 主文献

- [ACM/IEEE-CS/AAAI CS2023 Knowledge Areas](https://csed.acm.org/knowledge-areas/)：17 个知识域。能力方向收成 Software、Systems、Applications 三块，Software 是后两块的先修（见 [知识模型说明](https://csed.acm.org/wp-content/uploads/2024/04/1.3-Introduction-to-Knowledge-Model.pdf)）。
- [SWEBOK Guide V4](https://www.computer.org/education/bodies-of-knowledge/software-engineering/topics)：18 个知识域。软件工程自成体系，并单独列出 Software Architecture、Software Engineering Operations、Software Security，以及 Computing / Mathematical Foundations。
- 教育部《计算机类教学质量国家标准》：学科基础覆盖程序设计、数据结构、计算机组成、操作系统、计算机网络、信息管理；计算机科学与技术专业知识再加系统结构、算法、程序设计语言、软件工程、并行分布计算、智能技术等（转载：[博客园整理](https://www.cnblogs.com/rocedu/p/9721863.html)）。
- [Teach Yourself Computer Science](https://teachyourselfcs.com/)：九门自学科目，顺序是编程、体系结构、算法、数学、操作系统、网络、数据库、语言与编译、分布式系统。
- [roadmap.sh](https://roadmap.sh/)：按角色把 Frontend / Backend、DevOps、Cyber Security、AI 与数据拆开，用来支撑 07、08、09、10，而不是用来替代学科分类。

### CS2023 缩写 → 本图谱

| CS2023 | 本图谱 | 说明 |
|--------|--------|------|
| MSF | 01 | 数学与统计基础 |
| AL | 02 | 算法与复杂度 |
| SF、AR、OS、NC | 03 | **合并判断**：CS2023 与 Teach Yourself CS 都把网络单独成科；本图谱并入「计算机系统」，依据是 CSAPP 把组成、操作系统和网络放在同一条程序员系统观里，以及 CS2023 Systems 能力方向把 SF、AR、OS、NC、PDC 放在一起 |
| FPL | 04 | 编程语言基础 |
| SDF 与 SE | 05 | SDF 里的基础编程会跨到 02 和 04；主归属放 05 只覆盖「如何把程序做成软件」 |
| DM | 06 | 数据管理 |
| SPD（Web、移动等平台） | 07 | HCI、图形学在 CS2023 是独立知识域，本图谱不升为顶层，后挂到 07 |
| PDC | 08 | 并由 roadmap.sh 的 DevOps / Cloud 补上 Linux、容器、云和可观测性 |
| SEC | 09 | 安全 |
| AI | 10 | CS2023 由 AAAI 共同背书，人工智能与算法、系统平级 |
| SEP | （不设顶层） | 社会、伦理与职业；必要时写进 `00-map/` |

**06 与 08：** Kleppmann《Designing Data-Intensive Applications》同时被当作数据库和分布式系统的读物，两域必须互链，不能切死。

### 与其他文献的对应（摘要）

| 来源 | 如何支撑本图谱 |
|------|----------------|
| SWEBOK V4 | 05 的骨架；Architecture / Operations / Security 分别映射到 05、08、09；Foundations 支撑 01 |
| 国标计算机类 | 组成/OS/网络 → 03；数据结构/算法 → 02；信息管理 → 06；并行分布 → 08；智能技术 → 10 |
| Teach Yourself CS | 自学顺序写入 `00-map/learning-paths.md`；九门科目折叠进 01–08 |
| roadmap.sh | 角色路径支撑 07（前后端）、08（DevOps/Cloud）、09（Cyber Security）、10（AI） |

## 跨域归属规则

1. **一个概念只写一处正文**，其他域用「参见」链接，不复制提纲。
2. **主归属**：去掉它哪条域会缺机制，就归哪条。例如协议栈归 03，浏览器与 Web 应用归 07。
3. **两域都讲得通**：按读者先遇到的域落正文；资料主档仍只一页。
4. **例子/产品工具不新建域**，挂在最近主题的资料或参见里。
5. **性能、面试、职业等不升顶层**，挂最近主题或 `00-map/`。
6. **暂不定居**：记入 [00-map/inbox.md](00-map/inbox.md)。

主题页固定字段须含：主归属、参见、不包含什么（详见 [_templates/topic.md](_templates/topic.md)）。

## 各域划界书（本阶段仅点名）

| 域 | 划界书 / 材料 |
|----|----------------|
| 01 | Sipser 或 MIT 6.042 数学 |
| 02 | Skiena《The Algorithm Design Manual》 |
| 03 | Bryant / O'Hallaron《Computer Systems: A Programmer's Perspective》 |
| 04 | Nystrom《Crafting Interpreters》 |
| 05 | SWEBOK V4 |
| 06 | Hellerstein 等《Readings in Database Systems》 |
| 07 | Kurose《Computer Networking: A Top-Down Approach》的应用语义部分 + MDN |
| 08 | Kleppmann DDIA 与 MIT 6.824 |
| 09 | Anderson《Security Engineering》 |
| 10 | Russell / Norvig《Artificial Intelligence: A Modern Approach》 |

本阶段不写书评；资料主档占位见 [resources/](resources/)。

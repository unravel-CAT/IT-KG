# IT 技术栈知识图谱

纯 Markdown 资料库：用目录与链接表达知识结构，不引入站点生成器或数据库。

**知识在前，资料在后。** 主题先写清定义与骨架，再挂书籍、网站、博客；资料有独立主档，主题页只引用。

**树是分类，路径是视图。** 正文按知识域存放；学习顺序见 [00-map/learning-paths.md](00-map/learning-paths.md)。

## 怎么读

1. [taxonomy.md](taxonomy.md) — 顶层分类、主归属与交叉引用规则  
2. [00-map/panorama.md](00-map/panorama.md) — 域与域之间的依赖  
3. [00-map/how-to-read.md](00-map/how-to-read.md) — 深度层级、条目字段、何时新建主题  
4. [00-map/learning-paths.md](00-map/learning-paths.md) — 系统向 / Web 全栈 / 数据 / 安全等路径  
5. [00-map/inbox.md](00-map/inbox.md) — 暂不定归属的待分类笔记  

目录用英文短横线；标题和正文用中文；术语保留英文（如 HTTP、CAP）。编号前缀固定阅读顺序，不表示难度。

## 十条知识域

| # | 域 | 一句话 |
|---|----|--------|
| 01 | [计算基础](01-computing-foundations/) | 数学与信息表示，服务后面所有域 |
| 02 | [算法与数据结构](02-algorithms/) | 复杂度、结构、设计范式 |
| 03 | [计算机系统](03-computer-systems/) | 程序如何在机器和网络上跑起来 |
| 04 | [编程语言](04-programming-languages/) | 语言本身，不是某个框架 |
| 05 | [软件工程](05-software-engineering/) | 把程序做成可维护的软件 |
| 06 | [数据系统](06-data-systems/) | 建模、存放、查询与流动 |
| 07 | [互联网与应用](07-internet-applications/) | 用户可感知的网络软件 |
| 08 | [基础设施与分布式](08-infrastructure/) | 部署、扩展与排障 |
| 09 | [安全](09-security/) | 攻防与工程化安全 |
| 10 | [人工智能](10-artificial-intelligence/) | 从经典机器学习到工程实践 |

依赖大致自上而下：上面的域是下面的先修，同层可以平行学。安全与人工智能横跨多域，仍各自独立成域。

## 深度约定

- **L0** 全景（本页与 `00-map/`）  
- **L1** 域地图（各域 `README.md`）  
- **L2** 子域清单（写在域地图里）  
- **L3** 主题页（`topics/`，本阶段不写正文）  

资料主档在 [resources/](resources/)；模板在 [_templates/](_templates/)。

## 本仓库现阶段

只落地骨架：分类总纲、十条域地图、统一模板、资料目录占位。不写 L3 主题正文，也不写完整资料书评。

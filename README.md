# The Kai Project
```text
"Answer to the Ultimate Question of Life, the Universe, and Everything"
```

本项目旨在提供一个开源的、便捷的、分享与讨论修考试题答案的地方，破除信息之壁。

项目地址 [https://runjp.com/](https://runjp.com/)

<figure style="text-align:center;">
  <img src="https://raw.githubusercontent.com/Myyura/the_kai_project_assets/main/sample.png" width="700" alt=""/>
</figure>

## LICENSE
本项目使用 GNU Affero General Public License v3.0, 所有解答版权由本项目与作者所有, 试题版权归出题方（校方）所有。

感谢每一位项目的贡献者。

## How to contribute
我们期待你的Input, 倘若你熟悉Git, 可以通过直接为本项目提交PR的方式添砖加瓦, 倘若你不熟悉, 亦可将想要分享的试题/答案通过邮件的方式发送给我们, 我们第一时间将其提交到本项目之上。

* email: 376672994@qq.com

我们并不追求解答的完整性, 但如果你发现了现有解答中的错误, 请积极指出. 亦可以加入项目群与大家交流题解.

* QQ群: 925154731

如有侵权, 请随时联系.

### 内容格式说明

#### 文件结构

```markdown
docs/
├── <university>/
│   ├── <department>/
│   │   ├── <specialization>/
│   │   │   ├── <year>/
│   │   │   │   └── <exam_file>.md
blog/
├── <category>/
│   └── <blog_post>.md
```
docs下每个文档文件都包含有元数据的前置信息，如`sidebar_label`和`tags`，以便于正确组织和查找。

#### 文档前言

文档前言是用来为你的 Markdown 文档页面提供额外的元数据的。本项目的前言有两个，

`sidebar_label`为文档在侧边栏的标题，

`tags`为文档的标签，一般为**学校**（提交时必须标注）和**考点**（非必须）。

以`東京大学 工学系研究科 物理工学専攻 2020年度 物理学 第3問`为例：
```markdown
---
sidebar_label: '物理学 第3問'
tags:
  - Tokyo-University
  - xxx考点
---
```

前言添加完毕后，将你想提交的 Markdown 文件放在 docs 目录下对应的`docs/<university>/<department>/<specialization>/<year>/`目录里，

以`東京大学 工学系研究科 物理工学専攻 2020年度 物理学 第3問`为例

即`docs/tokyo-university/engineering/ap/2020/ap_2020_phys_3.md`。

#### 经验贴前言

每个作者都应该至少有 `name` 属性。

Single author:

```markdown
---
title: Post title
authors:
  name: example author
tags: [Tag1, Tag2]
---
```

Multiple authors:

```markdown
---
title: Post title
authors:
  - name: Joel Marcey
  - name: Sébastien Lorber
tags: [Tag1, Tag2]
---
```

<details>

<summary>构建网站部分（非必须）</summary>

### 网页构建
本网站使用现代静态网站生成器 [Docusaurus](https://docusaurus.io/)构建。

Docusaurus 本质上是一组npm包。

#### 要求
Node.js 版本 18.0 或以上 (可以通过运行 `node -v` 来查看)。
 你可以用 nvm 来管理同一机器上的多个 Node 版本。
安装 Node.js 时，建议勾选所有和依赖相关的选项。

#### 安装

clone本项目 

```bash
git clone https://github.com/Myyura/the_kai_project.git
```
进入项目文件夹

```bash
cd the_kai_project
```
安装docusaurus

```bash
npm install docusaurus
```

#### 本地测试构建

在部署到生产环境前，事先进行本地测试尤为重要。

```bash
npm run serve
```
站点默认会部署在 `http://localhost:3000/`

</details>

### 提交

检查无误后提交 Pull Request，审核无冲突后维护者会合并分支。

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Myyura/the_kai_project&type=Date)](https://www.star-history.com/#Myyura/the_kai_project&Date)

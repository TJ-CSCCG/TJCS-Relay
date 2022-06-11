# :rocket: Task-1

## 1. Background

### i. Markdown

`Markdown` 是一种标记语言，`GitHub` 支持 `Markdown` 渲染，你可以在 [这里](https://github.com/younghz/Markdown) 学习它的使用。

### 2. git

`git` 是一种分布式版本控制系统，可以在 [这里](https://www.liaoxuefeng.com/wiki/896043488029600/) 简单学习这个工具的使用。以下是我认为作为初学者需要掌握的内容：

* 利用 `git` 提交修改；
* 利用 `git` 与他人协作；
* 与远端仓库建立连接；
* 处理代码合入冲突。

进一步，可以在 [这里](https://git-scm.com/book/en/v2) 了解更详细的内容。如果你认为这不具有挑战性，可以通过 [这里](https://github.com/b1f6c1c4/learn-git-the-super-hard-way) 学习如何使用。

### 3. GitHub

`GitHub` 是目前世界上最大的软件项目托管平台。可以通过自建练习仓库，测试 `git` 指令和 `GitHub` 功能以理解下述问题：

* `GitHub` 上与他人协作的工作流程；
* `GitHub` 中的仓库可以做什么。

## 2. Tasks

* **Markdown** | [TJ-CSCCG/TJCS-Course](https://github.com/TJ-CSCCG/TJCS-Course)：

  针对 **1 门 专业必修课 或 专业选修课**，使用 `Markdown` 写一篇课程简述。

  * 简述内容包括但不限于 “选用教材”、“作业情况”、“课堂规则”、“考试方向”、“教师评价” 等方面；（注： **保护隐私**，不可透露 **姓名** 等信息）
  * 该 `*.md` 文件的命名格式参考 [这里](https://github.com/TJ-CSCCG/TJCS-Course/blob/master/CONTRIBUTING.md)；
  * 具体示例：[100583_信息安全数学基础](https://github.com/TJ-CSCCG/TJCS-Course/tree/master/100583_信息安全数学基础)。

* **git / GitHub** | 合作流程：
  1. `fork` 你的目标仓库 A 到你所 “掌控” 的用户或组织下，暂称该 `fork` 仓库为 B；
  2. `clone` 你的仓库 B 到本地，暂称该本地仓库为 C；
  3. 在本地仓库 C 中新建一个分支 a，此后你的所有 `commit` 都在分支 a 上操作；
  4. 将新增的 `*.md` 文件放在同一路径下 / 修改对应的 `*.md` 文件；
  5. 在本地 `commit`，并将分支 a `push` 到你的仓库 B；
  6. 在你的仓库 B 页面点击 `Pull Request`，以仓库 B 中的 a 分支到仓库 A 中的目标分支，向上游仓库 A 发起 `PR`。

（在完成 “体验合作流程” 的第 6 步骤后，新增 / 修改可能不会第一时间合入上游仓库。）

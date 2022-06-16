# :rocket: Task-2

## 1. Background

### i. TeX

TeX 是一种排版语言，只支持英文和数字，通过将 TeX 转换为 PostScript 打印已排版文档。

广为人知的 pdfTeX / XeTeX / LuaTeX 都是重写 TeX 引擎以支持新功能。如 pdfTeX 支持直接输出 pdf 格式文件；XeTeX 支持多种语言；LuaTeX 提供了扩展 TeX 的手段。

LaTeX 摒除了 TeX 底层指令的复杂性，是一个庞大的宏指令集合。可以通过刘海洋的 《LaTeX 入门》 学习 LaTeX 基本使用。所谓的 pdfLaTeX / XeLaTeX / LuaLaTeX 就是在分别使用上述 pdfTeX / XeTeX / LuaTeX 引擎的前提下使用 LaTeX 宏指令集合。

可以通过 [这里](https://www.overleaf.com/learn/latex/Writing_your_own_class) 了解 LaTeX 文档类的写法。

下列是需要了解的工具或工作环境：

* [TexStudio](https://www.texstudio.org/)：一款历史较为悠久的 LaTeX 继承写作环境，现在仍被广泛使用。
* [Overleaf](https://www.overleaf.com/)：一款线上 LaTeX 编辑器，不需人工配环境，十分容易上手。你可以通过 [这里](https://www.overleaf.com/latex/templates/tongji-undergrad-thesis/dfdvqsmpfcgk) 在 Overleaf 上写课程报告。
* VSCode LaTeX-Workshop：一款 VSCode 插件，提供了在 VSCode 上定制化编译 LaTeX 文档的能力。
* latexmk：一个 perl 工具，提供了构建 LaTeX 项目的简单方法。可以通过 [这里](https://mg.readthedocs.io/latexmk.html) 简单了解。

### ii. make

Makefile 用于告知 make 以何种规则运行。可通过下列链接简单了解 Makefile：

* [定义规则](https://www.gnu.org/software/make/manual/make.html#Rule-Syntax)
* [使用通配符](https://www.gnu.org/software/make/manual/make.html#Wildcards)
* [Phony 目标 (.PHONY)](https://www.gnu.org/software/make/manual/make.html#Phony-Targets)
* [使用简单变量](https://www.gnu.org/software/make/manual/make.html#Reference)
* [Automatic 变量 ($@ $< $^)](https://www.gnu.org/software/make/manual/make.html#Automatic-Variables)

## 2. Tasks

* **TeX** | [tongji-undergrad-thesis](https://github.com/TJ-CSCCG/tongji-undergrad-thesis)：

  * 根据剩余 [issues](https://github.com/TJ-CSCCG/tongji-undergrad-thesis/issues) 以及 1 系统上毕业设计论文模板要求修改现有模板。

* **Makefile** | [tongji-undergrad-thesis](https://github.com/TJ-CSCCG/tongji-undergrad-thesis)：

  * 在 ed55a5 下，确认 Linux 系统上使用 GNU Make 编译中断的原因（[Makefile](https://github.com/TJ-CSCCG/tongji-undergrad-thesis/blob/master/Makefile)）。

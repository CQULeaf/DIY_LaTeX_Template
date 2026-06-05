# DIY LaTeX Template

这是一个面向学习、写作、汇报与个人展示的 LaTeX 模板集合。仓库按使用场景拆分为四个可独立编译、独立复制、独立维护的模板工程：知识笔记、论文报告、日常汇报和个人简历。

## 模板速览

| 模板 | 场景 | 入口 | 推荐编译 |
| --- | --- | --- | --- |
| [`knowledge-note`](templates/knowledge-note/) | 日常学习、知识积累、数理与算法笔记 | `main.tex` | `latexmk -xelatex main.tex` |
| [`thesis-report`](templates/thesis-report/) | 课程论文、课程报告、毕设论文、正式提交材料 | `main.tex` | `latexmk -xelatex main.tex` |
| [`daily-presentation`](templates/daily-presentation/) | 组会汇报、小组 pre、项目周报、阶段性展示 | `main.tex` | `latexmk -xelatex main.tex` |
| [`resume`](templates/resume/) | 个人简历、实习申请、升学申请、项目申请 | `main.tex` | `latexmk -xelatex main.tex` |

## 如何选择

- 想长期沉淀课程知识、公式、算法、代码和概念框架：使用 `knowledge-note`。
- 想写课程论文、课程报告、毕业论文或结构正式的提交材料：使用 `thesis-report`。
- 想做组会、课程展示、阶段性进展汇报：使用 `daily-presentation`。
- 想快速产出一页式个人简历：使用 `resume`。

## 使用方式

进入目标模板目录后编译即可：

```bash
cd templates/<template-name>
latexmk -xelatex main.tex
```

每个模板目录下都有独立 `README.md`，其中包含目录结构、使用方式、模板能力、截图展示和定制说明。

## 核心特点

- **场景独立**：四类模板互不依赖，复制任意一个目录即可单独使用。
- **入口统一**：每个模板都以 `main.tex` 作为主入口，降低切换成本。
- **结构清晰**：复杂模板使用 `config/` 与 `content/` 分离格式和内容。
- **可复用可拓展**：模板部分以“重庆大学 / 叶旭航”为示例内容，同时保留集中替换区，便于迁移到其他学校或个人。

## 展示入口

- 知识笔记：见 [`templates/knowledge-note/README.md`](templates/knowledge-note/README.md) 中的字体、三线表、伪代码、代码块和彩色信息框展示。
- 论文报告：见 [`templates/thesis-report/README.md`](templates/thesis-report/README.md) 中的封面、图表公式与算法展示。
- 日常汇报：见 [`templates/daily-presentation/README.md`](templates/daily-presentation/README.md) 中的重庆大学 Beamer 主题展示。
- 个人简历：见 [`templates/resume/README.md`](templates/resume/README.md) 中的一页式简历展示。

## 维护原则

- 根目录只保留集合说明和导航，不放具体模板实现细节。
- 子模板 README 负责说明目录结构、能力、展示和定制方式。
- 编译中间文件默认忽略。
- 引入外部模板时保留来源、许可证和可替换边界。

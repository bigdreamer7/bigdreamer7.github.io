# Markdown
`Markdown`是一种轻量级标记语言，设计用于简单而易读的文本格式编写，最初由约翰·格鲁伯（John Gruber）和亚伦·斯沃茨（Aaron Swartz）共同开发。它使用易于阅读和书写的纯文本格式，并可转换为有效的HTML。Markdown的主要目标是使写作变得更加简单和直观，同时保持文本的可读性。它通过使用简单的标记符号来标记文本的结构和格式，如标题、列表、链接等。
## 语法指南
* [Markdown官方教程](https://markdown.com.cn)
* [在GitHub上写入](https://guides.github.com/features/mastering-markdown/)

## 画图工具
### [Mermaid](https://mermaid.js.org)
`Mermaid`是一个基于JavaScript的图表和可视化工具，它受Markdown的启发将文本渲染成图表，从而动态创建和修改图表。
```
graph TD;
    A-->B;
    A-->C;
    B-->D;
```
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
### Mermaid插件：
* `vscode` : [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)
* `mdbook` : [mdbook-mermaid](https://github.com/badboy/mdbook-mermaid)
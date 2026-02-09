# 中文文案排版指北（个人重制版）

本文章以中国大陆简体中文语境为主，繁体中文，例如港澳台和东南亚地区的中文习惯用法，可能与本文不同，建议按照地区规范进行调整。

## 空格

关于中文和英文之间添加空格，在排版界始终是有争议的，例如维基百科和某些出版社，他们要求中文和英文、数字之间不添加空格，他们依赖于，或者说推崇使用排版软件（例如 Microsoft Word）的自动处理，或者 [`test-spacing`](https://www.w3.org/TR/css-text-4/#text-spacing-property) 和 [-ms-text-autospace](https://learn.microsoft.com/en-us/previous-versions/ms531164(v=vs.85)) 来实现。一般来说，尤其是在 Markdown 和开发环境中，我建议在大多数场景下遵循下面的规范。

- 中英文之间需要增加空格。

- 中文与数字之间需要增加空格。

- 数字和单位之间无须增加空格。

- 度（°）和百分比与数字之间不需要增加空格。

- 全角标点和其他字符之间不增加空格。

- 分割多个并列关系且含义相对的中文字符时 ，使用半角符号 `/`，并在 `/` 前后增加空格（前后已经添加了空格的专有名词、全角标点除外）。

有一些工具可以实现自动在中文和英文、数字之间添加空格，例如：

| 仓库 | 系列 | 语言 |
| :-: | :-: | :-: |
| [pangu.js](https://github.com/vinta/pangu.js) | pangu | JavaScript |
| [pangu-go](https://github.com/vinta/pangu) | pangu | Go |
| [pangu.java](https://github.com/vinta/pangu.java) | pangu | Java |
| [pangu.py](https://github.com/vinta/pangu.py) | pangu | Python |
| [pangu.rb](https://github.com/dlackty/pangu.rb) | pangu | Ruby |
| [pangu.php](https://github.com/cchlorine/pangu.php) | pangu | PHP |
| [pangu.vim](https://github.com/hotoo/pangu.vim) | pangu | Vim |
| [vue-pangu](https://github.com/serkodev/vue-pangu) | pangu | Vue.js (Web Converter) |
| [intellij-pangu](https://plugins.jetbrains.com/plugin/19665-pangu) | pangu | Intellij Platform Plugin |
| [autocorrect](https://github.com/huacnlee/autocorrect) | autocorrect | Rust, WASM, CLI tool |
| [autocorrect-node](https://github.com/huacnlee/autocorrect/tree/main/autocorrect-node) | autocorrect | Node.js |
| [autocorrect-py](https://github.com/huacnlee/autocorrect/tree/main/autocorrect-py) | autocorrect | Python |
| [autocorrect-rb](https://github.com/huacnlee/autocorrect/tree/main/autocorrect-rb) | autocorrect | Ruby |
| [autocorrect-java](https://github.com/huacnlee/autocorrect/tree/main/autocorrect-java) | autocorrect | Java |
| [autocorrect-go](https://github.com/longbridgeapp/autocorrect) | autocorrect | Go |
| [autocorrect-php](https://github.com/NauxLiu/auto-correct) | autocorrect | PHP |
| [autocorrect-vscode](https://marketplace.visualstudio.com/items?itemName=huacnlee.autocorrect) | autocorrect | VS Code Extension |
| [autocorrect-idea-plugin](https://plugins.jetbrains.com/plugin/20244-autocorrect) | autocorrect | Intellij Platform Plugin |
| [jxlwqq/chinese-typesetting](https://github.com/jxlwqq/chinese-typesetting) | other | PHP |
| [sparanoid/space-lover](https://github.com/sparanoid/space-lover) | other | PHP (WordPress) |
| [sparanoid/grunt-auto-spacing](https://github.com/sparanoid/grunt-auto-spacing) | other | Node.js (Grunt) |
| [hjiang/scripts/add-space-between-latin-and-cjk](https://github.com/hjiang/scripts/blob/master/add-space-between-latin-and-cjk) | other | Python |
| [hustcc/hint](https://github.com/hustcc/hint) | other | Python |
| [n0vad3v/Tekorrect](https://github.com/n0vad3v/Tekorrect) | other | Python |

但是，我不推荐使用这种工具，最好还是在编写文章的适合，就自觉的遵循上述规则，况且这些工具在某些极端情况下的行为尚不可知。

## 标点符号

下面基本上是一些共识，详细参考[中文出版物夹用英文的编辑规范](https://www.nppa.gov.cn/xxgk/fdzdgknr/hybz/202210/P020221004608768453140.pdf)。

- 不使用过多重复的标点符号。虽然中国大陆的标点符号用法允许重复使用标点符号，但是这么做会破坏句子的美观性，除非特殊用途，不建议堆叠标点符号，尤其是毫无意义的时候。

- 使用全角中文标点，遇到完整的英文整句、特殊名词，其内容使用半角标点。

- 数字使用半角字符。在设计稿、宣传海报中如出现极少量数字的情形时，为方便文字对齐，是可以使用全角数字的。

- 不允许使用 `。。。` 代替 `……`。例外：允许使用三个连续的英语句点 `...` 代替三点省略号，因为大部分情况下显示效果相同甚至更好

下面的规则存在争议，而且在某些情况下被明确禁止，请谨慎参考：

- 对英文书名或句子的引用，用中文标点符号包裹，不要使用中文。

- 当用括号标注进行补充说明的适合，即使内容全部是英文，只要括号是全角括号，那么其中作为分割作用的逗号、顿号、分号全部使用全角，不要使用句号。

- 为了更美观、易读，简体中文可以使用直角引号；大部分情况下，遵循这一条可能较为困难，但是我们强烈建议在中文中不要使用英文引号，同时用全角中文引号 `“”` 以及 `‘’` 和其他中文字符宽度一致的字体。

- 这一条有极大的争议，请不要盲目听信：链接和正文、斜体和正文之间不要添加空格；句末不要使用全角点号代替句号，如果这一行只有数学公式，那么不要加句号，否则请避免在行末以数学公式结尾。

## 名词

我们建议适当使用缩写以追求更简洁的书写，但是这不应当以牺牲美观度和可读性为代价：

- 专有名词使用正确的大小写。标题或者引用等自动全部大写或小写的情况除外。

- 不要使用不地道的、可能引起歧义的缩写，当情境下显然可以理解的适合，允许在明显位置注明的情况下使用。

- 对于给大众看的文章，能用中文就避免使用英文；对于技术性文章，建议第一次同时指出中文和英文，之后使用习惯用法。

代词的用法，不要有性别歧视。

- 区分“的”和“地”，因为“得”的用法大众普遍不习惯，因此我们建议不要使用“得”一字，固定用法或者常用搭配除外。

- 他、她、它（以及他们、她们、它们）要用对，不要用“他”代指女性，对于同时存在多性别的群体，代指时可以使用他们，如果大部分人是女性，建议使用她们。

- 原则上，对女性应当用“妳”而非你，但是在中国大陆这不通用，或者是不是标准用法，因此这一条可以选择性执行。

- 对用户称呼“你”而非“您”，对自己称呼“我”或“我们”。

需要注意的是，应当以一个人的性别认同作为其性别，不要对跨性别者使用其指派性别（如果其明确同意，原则上可以使用，但是如果对方支持最好用他们的认同性别，那么应当遵循）。

## 参考资料

- [维基百科:格式手册](https://zh.wikipedia.org/wiki/Wikipedia:%E6%A0%BC%E5%BC%8F%E6%89%8B%E5%86%8C)

- [Chinese copywriting guidelines for better written communication／中文文案排版指北](https://github.com/sparanoid/chinese-copywriting-guidelines)

- [Chinese Copywriting Guidelines：中文文案排版指北（简体中文版）](https://github.com/mzlogin/chinese-copywriting-guidelines)

- [中文文案风格指南](https://pdfe.github.io/GUIDELINE/#/others/copywriter)

- [豌豆荚文案风格指南](https://docs.google.com/document/d/1R8lMCPf6zCD5KEA8ekZ5knK77iw9J-vJ6vEopPemqZM/edit?usp=sharing)

- [Help:格式 - openSUSE Wiki](https://zh.opensuse.org/index.php?title=Help:%E6%A0%BC%E5%BC%8F)

- [W3C 中文排版需求](https://www.w3.org/TR/clreq/)

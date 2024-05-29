# 格式手册

本页面将列出在 **Starship** 编写过程时推荐使用的格式规范与编辑方针。请您在撰稿或者修正 Wiki 页面以前，仔细阅读以下内容，以帮助您完成更高质量的内容。

## 贡献文档要求

当你打算贡献某部分的内容时，你应该尽量熟悉以下三部分：

- 文档存储的格式
- 文档的合理性
- remark-lint 和LaTeX公式的格式要求

### 文档引用与存储的格式

- 文档文件名可以为中文或英文，但更推荐使用英文命名文档，以获得更短的文档链接。文件名不能出现空格，请用`-`短横线连接。
- 如果你的文档中引用了某些外链图片，请确保你的图片文件已经转存到本库[\_media文件夹](https://github.com/HowCam/howcam.github.io/tree/main/docs/_media)下，以防止图片链接失效导致图片丢失。请自主创建合适的不易混淆的独立的路径。图片文件的命名应有规律，例如：`[文档名]+[图片序号].[图片后缀]`。
- 推荐使用 SVG 格式的图片，以获取较好的清晰度和缩放效果。
- 同时具有源文件和导出图像的图片（例如` JPG 文件与 PSD 文件`或者` SVG 图像与 TikZ TeX 源代码`），建议将源文件以与图片相同的文件名保存于同一目录下。
- 请确保您的文档中的引用链接的稳定性。**不推荐** 引用 **自建** 服务中的资源。
- 站内链接请去掉网站域名，并且使用相对路径链接对应 `.md` 文件。可以通过`?id=`设置id参数来链接到具体的某一节（标题）。

### 文档的合理性

**合理性**，指所编写的 **内容** 必须具有如下的特性：

- 由浅入深，内容的难度应该具有渐进性。
- 逻辑性。

除现有内容质量较低的情况外，建议尽量从 **补充** 的角度来做贡献，而非采取直接覆盖的方式。如果拿不准主意，可以通过[QQ群](/md/contribute?id=加入我们的讨论群)等形式与 **Starship**项目组联系。

### 文档的基本格式要求

#### 标点符号的使用

- 请在每句话的末尾添加 **句号**。
- 请正确使用 **全角** 标点符号与 **半角** 标点符号。汉语请使用全角符号，英语请使用半角符号。中文中夹用英文时，请参考 [中文出版物夹用英文的编辑规范](https://www.nppa.gov.cn/xxgk/fdzdgknr/hybz/202210/t20221004_445147.html)。
- 注意区分 **顿号** 与 **逗号** 的使用。
- 注意 **括号** 的位置。句内括号与句外括号的位置不同。
- 通常使用 **分号** 来表示列表环境中各复句之间的关系。
- 对于有序列表，推荐在每一项的后面添加 **分号**，在列表最后一项的后面添加 **句号**；对于无序列表，推荐在每一项的后面添加 **句号**。
- 注意区分各种不同的连接号，如 hyphen（一般使用 U+002D hyphen-minus（-），即键盘上的「减号」代替），U+2013 en dash（–）和 U+2014 em dash（—）。（英文中连接多个人名时，须用 en dash，但是极常误用为 hyphen。其他误用较为罕见，基本上只需记住这一点即可。）详见 [连接号 - 维基百科](https://zh.wikipedia.org/wiki/连接号)。

#### Markdown 格式与主题扩展格式要求

表示强调时请使用 `**SOMETHING**` 、 `「SOMETHING」`、或 `` ，而非某级标题，因为使用标题会导致文章结构层次混乱和（或）目录出现问题。

建议使用插件扩展的 `[!note]` 格式来描述需要补充介绍的内容。

- 使用方法：在正常的引用语句内，添加`[!note]`、`[!tip]`、`[!WARNING]`、`[!ATTENTION]`来表示文本高亮，效果如下：
- ![example1](https://pic.imgdb.cn/item/66484260d9c307b7e95de87d.png)

#### 文本内容的格式要求

- 在页面的开头应有一段简短的文字（如「本页面将介绍……」），用于概述页面内容。

- 涉及到「前置知识」的页面，请在开头添加一行 **前置知识：……**，放在页面概述前。格式如下：

  `前置知识：[站内页面1](url1)、[站内页面2](url2)和[站内页面3](url3)`

- 请注意文档结构。文档结构应当十分条理，层次清晰。请不要让诸如「五级标题」这种事情再次发生了，一篇正常的文章是用不到如此复杂的结构层次的。

- 请注意内容的表述。作为一个百科网站，**Starship** 使用的语言应该是书面的，客观的。诸如「抖机灵」性质的，对读者理解帮助不大的内容，不应该出现在 **Starship** 当中。

- 请尽量为链接提供完整的标题、或者可被识别的提示，避免使用裸地址和「这」、「此」之类的模糊不清的描述。每一个超链接都应尽量对其加以清楚明确的描述，方便读者明白该超链接将指向何处。

- 建议使用源文章或者标签页的标题。

- 所有用作序号的数字建议使用中文。示例：
  - 数列的第一项。
  - 输入文件的第一行。

#### LaTeX 公式的格式要求

-   您使用的符号不应与 [数学符号表](symbol.md) 规定的符号冲突。

-   使用 Roman 体表示数字、常量、算子和函数。使用 Italic 体表示变量、下标。LaTeX 已经预先定义好了一些常见的常量、函数、运算符等，我们可以直接调用，包括但不限于：

    ```latex
    \log, \ln, \lg, \sin, \cos, \tan, \sec, \csc, \cot, \gcd, \min, \max, \exp, \inf, \mod, \bmod, \pmod
    ```

    所以在输入常量、函数名、运算符等时，请先检查一下是否应该使用 Roman 体或其它字体。LaTeX 符号的书写可参考 [KaTeX 的 Supported Functions 页面](https://katex.org/docs/supported.html)（不是全部），也可以搜索求解。

    由于 LaTeX 书写 Roman 体小写希腊字母较为困难，故小写希腊字母常量、算子和函数可以使用 Italic 体，如 $\pi$ 以及 $\delta x$ 中的 $\delta$.

    如果遇到没有预先定义好的需要使用 Roman 体的 **函数名**，我们可以使用 `$\operatorname{something}$` 来产生，如我们可以使用 `$\operatorname{lcm}$` 产生正体的最小公倍数（函数）符号。同理，产生 Roman 体的 **常量** 应用 `$\mathrm{}$`；产生 Roman 体粗体符号应用 `$\mathbf{}$`；产生 Italic 体粗体符号应用 `$\boldsymbol{}$`（如向量 $\boldsymbol{a}$）。对于多字母的变量，应当使用 `$\textit{}$`。其他非数学内容，包括英文、特殊符号等，一律使用 `$\text{}$`。中文我们则建议不放在 LaTeX 公式中。

-   如果表达式须折行（常见于较长的行间公式中），则应遵循如下换行规则：

    -   将换行符放在 $=$，$+$，$-$，$\pm$，$\mp$ 之前，如果有必要，也可放在 $\times$，$\cdot$，$/$ 之前，如：

        $$
        \begin{aligned}
            \mathrm{e}^x &= \sum\limits_{n=0}^{\infty} \frac{x^n}{n!} \\
            &= \phantom{+} 1 + x + \frac{x^2}{2} \\
            & \phantom{=} + \frac{x^3}{6} + \frac{x^4}{24} + \dots \\
        \end{aligned}
        $$

    -   同一运算符不应在换行符前后同时出现，

    -   换行符尽量不要出现在括号内的表达式中。

-   在行内使用分数的时候，请使用 `$\dfrac{}{}$`。比如 `$\dfrac{1}{2}$`，效果 $\dfrac{1}{2}$，而不是 `$\frac{1}{2}$`，效果 $\frac{1}{2}$。

-   组合数请使用 `\dbinom{n}{m}`，效果 $\dbinom{n}{m}$，而不是 `{n \choose m}`（在 LaTeX 中这种写法已不推荐）；与上一条关于分数的约定相似，请不要使用 `\binom{n}{m}`，效果 $\binom{n}{m}$。

-   尽可能避免在行内使用巨运算符（如 $\sum$，$\prod$，$\int$ 等）。

-   在不会引起歧义的情况下，请用 `$\times$` 代替星号，叉乘请使用 `$\times$`，点乘请使用 `$\cdot$`。如 $a\times b$，$a\cdot b$，而不是 $a\ast b$。

- 请用 `$\cdots$`（居于排版基线与顶线中间），`$\ldots$`（居于排版基线的位置），`$\vdots$`（竖着的省略号）代替 `$...$`。如 $a_1,a_2,\cdots a_n$，而不是 $a_1,a_2,... a_n$。

- 公式中不要使用中括号连缀（即 C++ 高维数组的表示方式）而多使用下标。即 $a_{i,j,k}$ 而不是 $a[i][j][k]$。在公式中下标较复杂的情况下建议改用多元函数（$f(i,j,k)$）或内联代码格式。对于一元简单函数使用 `$f_i$`、`$f(i)$` 或 `$f[i]$` 均可。

-   在表示等价关系时，请使用 `$\iff$`，效果 $\iff$，而不是 `$\Leftrightarrow$`，效果 $\Leftrightarrow$。

-   分段函数环境 `cases`  **只能有两列**（即一个 `&` 分隔符）。

-   请不要滥用 LaTeX 公式。这不仅会造成页面加载缓慢（因为 MathJax 的效率低是出了名的），同时也会导致页面的排版混乱。我们通常使用 LaTeX 公式字体表示变量名称。我们的建议是，如非必要，尽量减少公式与普通正文字体的 **大量** 混合使用，如非必要，尽量不要使用公式，如：

    ```LaTeX
    我们将要学习 $Network-flow$ 中的 $SPFA$ 最小费用流，需要使用 $Edmonds–Karp$ 算法进行增广。
    ```

    就是一个典型的 **滥用公式字体** 的例子。（在页面中使用斜体请用 `*文本*` 表示。）

-   请正确使用对应的 LaTeX 符号，尤其是公式中的希腊字母等特殊符号。如欧拉函数请使用 `$\varphi$`，圆的直径请使用 `$\Phi$`，黄金分割请使用 `$\phi$`。这些符号虽然同样表示希腊字母 Phi，但是在不同的环境下有不同的含义。切记 **不要使用输入法的插入特殊符号** 来插入这种符号。

    另外，由于 LaTeX 历史原因，空集的符号应为 `$\varnothing$` 而不是 `$\emptyset$`；其他的符号应参照 [数学符号表](symbol.md) 书写。

我们可以使用一个表格来总结一下上述内容。注意本表格没有举出所有符号的用法，只给出常见的错误。类似的情况类比即可。

| 不符合规定的用法                     | 渲染效果           | 符合规定的用法                           | 渲染效果                               |
| ------------------------------------ | ------------------ | ---------------------------------------- | -------------------------------------- |
| `$log, ln, lg$`                      | $log, ln, lg$      | `$\log$, $\ln$, $\lg$`                   | $\log$，$\ln$，$\lg$                   |
| `$sin, cos, tan$`                    | $sin, cos, tan$    | `$\sin$, $\cos$, $\tan$`                 | $\sin$，$\cos$，$\tan$                 |
| `$gcd, lcm$`                         | $gcd, lcm$         | `$\gcd$, $\operatorname{lcm}$`           | $\gcd$，$\operatorname{lcm}$           |
| `$e$, $\text{e}$, e`（自然对数的底） | $e$，$\text{e}$, e | `$\mathrm{e}$`                           | $\mathrm{e}$                           |
| `$i$, $\text{i}$, i`（虚数单位）     | $i$，$\text{i}$, i | `$\mathrm{i}$`                           | $\mathrm{i}$                           |
| `$ 小于 a 的质数 $`                  | $小于 a 的质数$    | `小于 $a$ 的质数`                        | 小于 $a$ 的质数                        |
| `$...$`                              | $...$              | `$\cdots$, $\ldots$, $\vdots$, $\ddots$` | $\cdots$，$\ldots$，$\vdots$，$\ddots$ |
| `$a*b$`（两个数相乘）                | $a*b$              | `$a\times b$, $a\cdot b$`                | $a\times b$，$a\cdot b$                |
| `$SPFA$`（英文名称）                 | $SPFA$             | `SPFA`                                   | SPFA                                   |
| `$a==b$`                             | $a==b$             | `$a=b$`                                  | $a=b$                                  |
| `$f[i][j][k]$`                       | $f[i][j][k]$       | `$f_{i,j,k}$, $f(i,j,k)$`                | $f_{i,j,k}$，$f(i,j,k)$                |
| `$R,N^*$`（集合）                    | $R,N^*$            | `$\mathbf{R}$, $\mathbf{N}^*$`           | $\mathbf{R}$，$\mathbf{N}^*$           |
| `$\emptyset$`                        | $\emptyset$        | `$\varnothing$`                          | $\varnothing$                          |
| `$size$`                             | $size$             | `$\textit{size}$`                        | $\textit{size}$                        |
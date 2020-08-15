## 协作翻译MarkDown格式规范

请大家遵循统一的markdown格式，便于后期集中在一起导出PDF格式文件。

1. 关于标题
    * 文章标题为一级标题 
    * 希腊数字标号的为二级标题
    * 阿拉伯数字编号的章节为三级标题
    * 带小数点的阿拉伯数字编号的章节为四级标题
    * 以此类推，完成标题分级
    * 标题的markdown格式为：一级标题前面有一个#， 二级为##， 三级为###，以此类推，注意#后需要有一个空格

2. 关于正文
    * 正文直接编辑即可
    * 使用一个空白行即可完成分段

3. 关于文中的list
    * 文中的list都是代码或者命令
    * 请大家使用代码区块格式进编写
    * 代码区块的标记方式为用三个\`\`\`前后包裹整个代码，格式如下：\`\`\`我是代码\`\`\`
    * 显示效果如下：
```
cd $FOAM_INST_DIR
cd OpenFOAM -2.1. x
git pull
wclean all
./ Allwmake
```

4. 关于图片
    * 文中的图片我都已经导出并保存到主仓库中
    * 文中图片的编号和文章中的不一致，这是由于有一些图像中采用了多个图片引起的，请大家注意
    * 翻译过程中用到的图片，请使用链接进行显示，链接采用相对路径
    * 具体形式为 \!\[图像说明\]\(图像地址\)，示例：\!\[图像1\]\(images/82.PNG\)
    * 显示效果如下：

![图像1](images/82.PNG)
    * 请一定注意后缀名为大写的PNG，如写为小写将导致无法正常显示（血泪）

5. 关于公式
    * 需要插入数学公式时，使用两个美元符 $$ 包裹 TeX 或 LaTeX 格式的数学公式来实现
    * 示例如下
```
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$
```

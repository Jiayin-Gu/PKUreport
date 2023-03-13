# PKUreport

PKUreport 是一个针对北京大学博士后研究工作报告的 LaTeX，其制作符合 [北京大学博士后出站报告提交说明](https://www.lib.pku.edu.cn/portal/cn/zy/dzzy/chuzhanbaogao/tijiaoyaoqiu) 。


## 作者
顾加银，男，1990年出生，江苏盐城人，于2021年6月至2023年3月期间在北京大学从事博士后研究，方向为非平衡统计物理。联系方式：gujiayin1234@163.com。


## 特性
1 该模板是在 book 文类的基础上加入了 ctex 宏包，支持英文和中文。关于中文的说明，可以参见 [CTeX宏集手册](https://ctan.org/pkg/ctex?lang=en)。

2 该模板遵循简单性原则，没有做过多的封装，尽量将一些格式设置放在主文件的导言区。过多的封装会隐藏模板设计细节，从而影响用户对模板的理解。这里鼓励用户根据自己的需求对模板进行修改。

3 该模板的结构和研究报告的结构保持一致，从而可以使用户能快速且直观地理解模板的结构。




## 使用

使用 [TeX Live](http://tug.org/texlive/) 套装，该套装适用 Unix-like/Microsoft Windows/macOS 操作系统。

使用 xelatex 编译方式。

使用 biber 作为参考文献宏包 biblatex 的后台处理程序。




## 编译步骤
1 xelatex Report.tex

2 biber Report

3 xelatex Report.tex

4 xelatex Report.tex






## 一些具体说明

1 模板的主文件是 Report.tex，在其中可以添加章。每一章的所有相关文件放入一个子文件夹中。每一个子文件夹的路径通过 \path 定义。

2 摘要、致谢、文章发表分别写在相应的 tex 文件中。 

3 封面信息写在 Cover.tex 中。

4 原创性声明和使用授权说明是通过导入 Declaration.pdf 文件的形式，插入到最终的 Report.pdf 中的。可以单独打印 Declaration.pdf 文件，签字完扫描为新的文件，再导入。

5 参考文件信息写在 Bibliography.bib 文件中。这里其实可以导入用户自己的文献库，通过主文件中的添加 s\addbibresource{xxx.bib} 设置完成。

6 源文件中有时出现 spacing 环境，其目的是通过调整行间距，使得文字尽量充满一页，以达到美观的效果。







## 许可证
[GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/)








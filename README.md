# latex-chinese-fonts
```shell
#克隆远程库到本地
git clone git@github.com:vemd/NOTEBOOK.git
git add . 通过这个命令将创建好的测试项目保存到暂缓区
git commit -m "常见中文字体收集"
#  git remote add origin git@github.com:vemd/chinese-fonts.git
#  git push -u origin master
git push 将本地的仓库信息推送到远程仓库
```
收集常用的中文字体

- 使用参考

```latex
\documentclass[fontset=none]{ctexart}
\setCJKmainfont[BoldFont={FZHei-B01},ItalicFont={FZKai-Z03}]{FZShuSong-Z01}
\setCJKsansfont{FZHei-B01}
\setCJKfamilyfont{zhsong}{FZShuSong-Z01}
\setCJKfamilyfont{zhhei}{FZHei-B01}
\setCJKfamilyfont{zhkai}{FZKai-Z03}
\setCJKfamilyfont{zhfs}{FZFangSong-Z02}
\setCJKfamilyfont{zhli}{FZLiShu-S01}

\newcommand*{\songti}{\CJKfamily{zhsong}} % 宋体
\newcommand*{\heiti}{\CJKfamily{zhhei}} % 黑体
\newcommand*{\kaiti}{\CJKfamily{zhkai}} % 楷体
\newcommand*{\fangsong}{\CJKfamily{zhfs}} % 仿宋
\newcommand*{\lishu}{\CJKfamily{zhli}} % 隶书

\begin{document}

\Large

\centering

\begin{quote}
本站购买了北大方正的字库授权，大家可以按照如上代码设置中文显示即可。
\end{quote}

\begin{tabular}{ll}
 \verb|\songti|&\songti
书宋体，CJK 等价命令 \verb|\CJKfamily{zhsong}|。\\
 \verb|\heiti|&\heiti
方正黑体，CJK 等价命令 \verb|\CJKfamily{zhhei}|。\\
 \verb|\fangsong|&\fangsong
方正仿宋，CJK 等价命令 \verb|\CJKfamily{zhfs}|。\\
 \verb|\kaiti|&\kaiti
方正楷体，CJK 等价命令 \verb|\CJKfamily{zhkai}|。\\
\multicolumn{2}{l}{在 founder 字库中，额外定义了隶书}\\
 \verb|\lishu|& \lishu
方正隶书，CJK 等价命令 \verb|\CJKfamily{zhli}|。\\
\end{tabular}
\end{document} 
```
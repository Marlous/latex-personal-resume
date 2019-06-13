# LaTeX Personal Resume
## Introduction - 介绍
### Summary - 概要  
- 一个简约的个人简历模板，通过 LaTeX 生成 PDF，灵活的增减需要的内容模块。  
- 基于 [CV 项目](https://github.com/leouieda/cv) 制作。

### Features - 特性
1. 概况：
- 由一个主文件和若干个模块组成。
- 主文件为 resume.tex。
- 剩下的 tex 格式文件为组成的模块文件。
- 根据自己的情况修改主文件和需要的模块文件，然后在 resume.tex 文件中添加或删除需要或不需要的模块文件代码。

2. 模块文件：
- 基本情况 basic.tex
- 教育信息 education.tex
- 技能 skill.tex
- 项目 project.tex
- 经历 experience.tex
- 荣誉与奖项 reward.tex
- 其它（兴趣、正在学习、规划等） addition.tex

## Usage - 用法
1. 添加或删除照片：
- 默认为有照片。
- 无照片使用方法：将简历头部文本信息代码替换为无照片的简历头部文本信息即可。
```
% 简历头部文本信息
\begin{minipage}[b]{0.8\linewidth}
    \begin{center}
        {\fontsize{36pt}{0}\selectfont \MyName}
        \\[0.5cm]
        {\fontsize{16pt}{0}\selectfont \MyRole}
        \\[0.3cm]
        {\fontsize{10pt}{0}\selectfont
            \Affiliation
            \\[0.2cm]
            \Address
            \\[0.08cm]
            Email: \href{mailto:\Email}{\texttt{\Email}}
            \, | \,
            Tel： \url{\Phone}
            \, | \,
            Website: \url{\Website}
        }
    \end{center}
\end{minipage}
\hfill
\begin{minipage}[b]{0.2\linewidth}
\includegraphics[height=8\baselineskip]{figure.png}
\end{minipage}


% 无照片的简历头部文本信息
\begin{center}
    {\fontsize{36pt}{0}\selectfont \MyName}
    \\[0.5cm]
    {\fontsize{16pt}{0}\selectfont \MyRole}
    \\[0.3cm]
    {\fontsize{10pt}{0}\selectfont
        \Affiliation
        \\[0.2cm]
        \Address
        \\[0.08cm]
        Email: \href{mailto:\Email}{\texttt{\Email}}
        \, | \,
        Tel： \url{\Phone}
        \, | \,
        Website: \url{\Website}
    }
\end{center}
```

## Support - 支持
### Contact - 联系
- By Marlous
- E-mail：Goonecat@foxmail.com

## License - 版权信息
LaTeX Personal Resume is released under the CC BY 4.0 license. See [LICENSE](https://creativecommons.org/licenses/by/4.0/) for additional details.
## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/Lan911/Lan911.github.io/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### vnpy
vnpy是一套基于Python的量化交易程序开发框架。[[GitHub]](https://github.com/Lan911/vnpy/tree/v2.1.7/)
[[中文文档]](https://www.vnpy.com/docs/cn/index.html/)

本文档基于vnpy==2.1.7，python==3.7，Anaconda3，Pycharm2021.1。


#### vnpy环境搭建
1.从github上下载zip文件到本地，下载路径为：[[GitHub]](https://github.com/Lan911/vnpy/tree/v2.1.7/)

2.创建conda环境，可以尝试使用如下指令：
```markdown
conda create -n vnpy_37 python==3.7
conda activate vnpy_37
cd D:\vnpy\vnpy-2.1.7
.\install.bat
```
其中：

vnpy_37 是我自己的conda env的名字

D:\vnpy\vnpy-2.1.7 是我本地vnpy解压下来的文件位置

#### 测试运行
运行 vnpy-2.1.7\examples\vn_trader\run.py 文件。如果出现如下界面，则表示环境搭建成功。
![image](https://user-images.githubusercontent.com/84230708/135444077-ce379f1f-6195-454e-ab08-1508d84594a2.png)

#### 遇到的问题
出现AttributeError: 'backports.zoneinfo.ZoneInfo' object has no attribute 'zone'

#### 解决办法
因为tzlocal这个库更新到3.0以后，原来的get_local_zone更改了，需要使用tzlocal 2.1 版本。可以尝试如下指令：
```markdown
pip install tzlocal==2.1
```

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Lan911/Lan911.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

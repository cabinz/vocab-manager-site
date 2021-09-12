---
title: 使用手册
keywords: 
last_updated: 2021-9-8
summary: Vocab Manager 1.x 的特性和使用帮助。
topnav: topnav_zh
sidebar: v1_zh_sidebar
permalink: v1_zh_manual.html
folder: v1_zh
---

## 1. 初始界面

{% include image.html file="v1_manual/app-home.png" alt="" caption="" %}


安装后，桌面会出现软件的快捷方式，双击打开软件，进入初始界面。

初始界面有两个按钮，点击上方“Notebook"按钮进入笔记本界面进行生词编辑，点击下方“Quiz”按钮进入测试界面进行生词遗忘测试。



## 2. 笔记本界面

笔记本界面分为两页，分别是生词页、标签页，通过页面上方的便签栏进行切换。



### 2.1 生词页

生词编辑页分为左右两栏。左侧是生词浏览框、右侧是生词细节区。



#### 2.1.1 生词列表

生词浏览框，包括上方的生词搜索框 、下方的生词列表。

初始状态下，所有可用的单词都会显示在生词列表中。可以使用生词搜索框对生词进行检索，检索结果会实时显示在下方的生词列表内。生词列表上方会实时显示当前列表中（被筛选出来的）生词数目。

如果希望移除某个单词，在单词列表中选中该单词，并点击下方的”Remove“即可执行移除。

{% include image.html file="v1_manual/word-list-filter.png" alt="" caption="" %}


#### 2.1.2 生词细节

Vocab Manager希望提供的是高度定制化的生词管理工具，以提供给不同领域的使用者。因此，所有的生词细节：包括生词的拼写、定义/翻译（Definition）、生词的语境/例句（Context）、笔记（Notes）都需要由用户进行输入。如果用户在标签页预定义了标签，也可以给生词打上不同的标签。

* 生词拼写、生词定义、生词例句、生词笔记进行人工添加，只有生词拼写不能为空；
* 如果在标签页预定义了标签，可以在添加标签栏下方的下拉框中找到这些标签。在下拉框中选中想要添加的标签后，单击“Tagging”即添加一个标签；
* 如果希望移除标签，则需要在标签栏上方的列表中选中相应的标签，并按下键盘上的”Delete“按键，进行标签移除；
* 双击标签列表中相应的标签，会转跳到相应的标签页面；

**所有在生词细节区中的输入，都需要通过下方的“Create”和“Update”按钮来进行提交**：“Create”是指创建新的一个词条，“Update”是指更新当前选中的词条。“Create”的快捷键是 “Ctrl+Shift+Enter”，“Update”的快捷键是“Ctrl+S”。

最底部中间的 “Clear”按钮，将会清空生词细节区的所有用户输入，以便进行一个新词条的创建。

{% include image.html file="v1_manual/word-detail-editor.png" alt="" caption="" %}



### 2.2 标签页

标签页同样分为左右两栏。左侧是标签浏览框、右侧是标签细节区。

标签页的行为与生词页几乎相同，所有的用户数据也需要通过按钮或快捷键进行提交后才能够保存。

额外的栏目是右下角会展示带有该标签的所有单词。双击其中的单词，会自动转跳到相应的生词页面。

{% include image.html file="v1_manual/tag-viewer.png" alt="" caption="" %}



### 2.3 工具栏

左上角的工具栏，目前仅支持两个功能。

* “File”下的”export as markdown“功能：将所有的生词导出为一份markdown文档，用户可以将其转换为任意格式、打印，便于在其它终端进行复习和回顾。
* “Recycle Bin” 回收站：所有被 “Remove” 移除的单词会进入回收站进行缓冲，用户随时可以进入回收站对移除的单词进行恢复或彻底删除。

{% include image.html file="v1_manual/top-menu.png" alt="" caption="" %}



导出的markdown文件：

{% include image.html file="v1_manual/output-markdown.png" alt="" caption="" %}



## 3. 生词测试界面

生词测试界面是Vocab Manager为用户提供的生词自测功能。通过不断展示生词的拼写，用户判断自己是否记忆该单词选择”Remember“（记得）或”Forget“（遗忘），来进行生词自测。

所有生词自测的结果都会被记录，生词出现的先后顺序，按照历史遗忘率从高到低进行排序。

{% include image.html file="v1_manual/quiz-form.png" alt="" caption="" %}



### 3.1 生词导入

目前支持将所有生词进行导入、按照标签类别进行导入两种选项。

{% include image.html file="v1_manual/load-quiz.png" alt="" caption="" %}

导入生词后，下方按钮变为可操作状态，点击任意按钮开始自测。

{% include image.html file="v1_manual/start-quiz.png" alt="" caption="" %}



### 3.2 遗忘测试

对于正上方中央显示的生词，如果用户对单词的相关信息回忆良好，则单击”Remember“，进行下一个单词的测试。

{% include image.html file="v1_manual/remember.png" alt="" caption="" %}



如果用户忘记了当前单词的有关信息，可以单击”Forget“：

{% include image.html file="v1_manual/forget.png" alt="" caption="" %}

此时，界面会弹出相关信息，供用户查阅。查阅完成后，单击Next继续。

{% include image.html file="v1_manual/detail-hint.png" alt="" caption="" %}



### 3.3 自测报告

当所有导入的生词都测试完毕时，会显示”No more records"。此时，可以点击“File”中的“generate report”生成此次自测的错误报告，其中包含所有此次字词中遗忘的单词已经这些单词的细节，和“export”一样以markdown文件的形式呈现。

事实上，用户在自测过程中可以随时点击生成自测报告，生成包含截至当前的错误生词的报告文件。

{% include image.html file="v1_manual/export-report.png" alt="" caption="" %}
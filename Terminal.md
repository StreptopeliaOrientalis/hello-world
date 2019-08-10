# 终端

https://sspai.com/post/45534

**操作系统分为两个部分，一部分称作内核，另一部分成为用户交互界面**。内核部分负责系统的全部逻辑操作，由海量命令组成，这一部分是系统运行的命脉，不与用户接触；交互界面则是开机之后所有我们所看到的东西，比如窗口，软件，应用程序等等。

**终端就是连接内核与交互界面的这座桥**，它允许用户在交互界面上打开一个叫做「Terminal 终端」的应用程序，在其中输入命令，系统会直接给出反馈。

## 1 路径

显示当前工作路径`pwd`：

```terminal
(base) appledeMacBook-Air-3:~ apple$ pwd
/Users/apple
```

表示/Users/apple/.documents

可以使用相对路径 /.Documents

```
(base) appledeMacBook-Air-3:~ apple$ cd ./Documents
```

也可以直接拖进来

`cd`就是设置工作路径的意思

```
(base) appledeMacBook-Air-3:Documents apple$ cd /Users/apple/Desktop/C 
(base) appledeMacBook-Air-3:C apple$ pwd
/Users/apple/Desktop/C
```

看看里面有啥 `ls`：

```
(base) appledeMacBook-Air-3:C apple$ ls
2019 AO3精华
2019-08-08 Books
ACADEMY
ANKI FLASHCARDS_MD
AO3
AQF
BOOKS
ENGLISH
MATHS
Machine Learning A-Z Chinese Template Folder
Teaching Graduate Students How to Write Clearly.md
屏幕快照 2019-07-12 下午3.03.44.png
屏幕快照 2019-07-29 下午7.43.44.png
```

把文件夹给打开了 `ls -R` (东西有点多)

```
(base) appledeMacBook-Air-3:C apple$ ls -R
2019 AO3精华
2019-08-08 Books
ACADEMY
ANKI FLASHCARDS_MD
AO3
AQF
BOOKS
ENGLISH
MATHS
Machine Learning A-Z Chinese Template Folder
Teaching Graduate Students How to Write Clearly.md
屏幕快照 2019-07-12 下午3.03.44.png
屏幕快照 2019-07-29 下午7.43.44.png

./2019 AO3精华:
[Cherik] Bifurcation.epub
[Cherik] The stars incline us they do not bind us.epub
[Cherik]The Long Pause.epub
[Hannigram] The Very Secret Diary of Will Graham.epub
[Hannigram]The Shape of Me Will Always Be You.epub

./2019-08-08 Books:
Beautiful Code.pdf
Make Something Up - Chuck Palahniuk - azw3 epub
The Best American Essays 2011_ The Best  - Danticat_ Edwidge.mobi
The Best American Travel Writing 20111.mobi
[Bright_Susie]_The_Best_American_Erotica_2002(z-lib.org).fb2
[Chuck_Palahniuk]_Choke(z-lib.org).epub
[Clifford A. Pickover] The Math Book From Pythago(z-lib.org).pdf
[Kensington_Ladies'_Erotica_Society]_Ladies'_Own_E(z-lib.org).pdf
代码之美 浪潮之巅 数学之美.pdf
编程人生-Coders+at+Work.pdf
机器学习.pdf
统计学习方法.pdf

./2019-08-08 Books/Make Something Up - Chuck Palahniuk - azw3 epub:
Make Something Up - Chuck Palahniuk.azw3
Make Something Up - Chuck Palahniuk.epub
cover.jpg
metadata.opf

./ACADEMY:
Financial News
Get Some Headspace.epub
Introductory Econometrics A Modern Approach 6th.pdf
Logic - A Very Short Introduction.pdf
Note-Taking for Consecutive Interpreters.pdf
Shreve－Stochastic Calculus for Finance I & amp;II(2004).pdf
Thomas Calculus 13th with Solutions
Verbal.Advantage.pdf
[1]方法论 宏微观.pdf
[2]微观.pdf
[3]宏观.pdf
[JEFFREY_M._WOOLDRIDGE]_Introductory_Econometrics.(BookFi.org).pdf
[啊哈！算法].啊哈磊.扫描版.pdf
中文 introduction to econometrics.pdf
曹乾-曼昆-微观经济学原理-中文六版.pdf
宏观经济学.pdf
金融随机分析 Shreve 中文版 1、2卷全.pdf
计量经济学导论-现代观点（第5版）[美]伍德里奇_部分1.pdf
计量经济学导论-现代观点（第5版）[美]伍德里奇_部分2.pdf
李子奈计量经济学.pdf
大学生数学竞赛教程 [蒲和平编著].pdf
深南电的期权对赌困局-金融创新案例范本.pdf
【俄罗斯数学教材选译】24.概率（第1卷）【施利.pdf
【俄罗斯数学教材选译】25.概率（第2卷）【施利.pdf
习题解答：金融随机分析（Stochastic Calculus for Finance）.pdf
从荣格的分析心理学看海明威的_硬汉_情结_郭伟平.pdf
中国历史上央行加息降息时间一览表.docx
计量经济学导论伍德里奇第五版答案Wooldridge5thOdd.pdf
范里安微观经济学现代观点第八版中文版.pdf

./ACADEMY/Financial News:
DAY 01 外汇风险准备金率下调 9月新闻
DAY 02 2017年10月存款准备金率、利率
DAY 03 2018年11月人民币近半年贬值原因简析
DAY 04 2018.11.11_10月初 央妈宣布全面降准
DAY 05 2018.11.13_2019中国宏观经济走势展望_中美贸易摩擦影响
DAY 06 2018.11.15_2019中国宏观经济走势展望_中美贸易摩擦影响_2
DAY 07 2018.11.17_2019中国宏观经济走势展望_中美贸易摩擦影响_完整版
DAY 08 2018.11.19_民主党夺回众议院之后
DAY 09 2018.11.21_中美国债收益率倒挂_全球央行动态简析_01
DAY 10 2018.11.23_中美国债收益率倒挂_全球央行动态简析_完整版
DAY 11 2018.11.25_台湾地区“九合一”选举结果揭晓
DAY 12 2018.11.27_大宗商品价格下跌_01
DAY 13 2018.11.29_大宗商品价格下跌_美国退出伊朗核协议_完整版
DAY 14 2018.12.01_大湾区对中国跨越中等收入陷阱将发挥重要作用
DAY 15 2018.12.03_G20吃一顿饭的功夫,中美贸易战就结束了吗_01
DAY 16 2018.12.05_G20吃一顿饭的功夫,中美贸易战就结束了吗_完整版
DAY 17 2018.12.07_卡塔尔宣布退群！全球油价掌舵者闹分裂
DAY 18 2018.12.09_证监会孙念瑞：强平对二级市场影响很小（简易版）
DAY 19 2018.12.11_证监会孙念瑞：强平对二级市场影响很小_详细学习笔记
DAY 20 2018.12.13_神仙打架之高通VS苹果and我们真的买不到iphone了吗_简略版
DAY 21 2018.12.15_神仙打架之高通VS苹果and我们真的买不到iphone了吗_详细版
DAY 22 2018.12.17_央妈连续近40个交易日未实施逆回购是什么情况
DAY 23 2018.12.19 _央行重启逆回购
DAY 24 2018.12.21 _2018年RMBS一骑绝尘增长超2倍
DAY 25 2018.12.23 _2018年RMBS一骑绝尘增长超2倍 完整版
DAY 26 2018.12.25 _一文读懂年终奖在个税新规下如何计税
DAY 27 2018.12.27 _基金业新格局 part1
DAY 28 2018.12.27 _基金业新格局_货基规模缩水_债基亮眼_完整版
DAY 29 2018.12.31 _港交所全年IPO上市数量和募资额双冠全球

./ACADEMY/Financial News/DAY 01 外汇风险准备金率下调 9月新闻:
DAY01 外汇风险储备金下调.doc
DAY01 外汇风险储备金下调PDF .pdf

./ACADEMY/Financial News/DAY 02 2017年10月存款准备金率、利率:
DAY02 未来存款准备金率应发挥宏观审慎工具作用.doc
DAY02 未来存款准备金率应发挥宏观审慎工具作用.pdf

./ACADEMY/Financial News/DAY 03 2018年11月人民币近半年贬值原因简析:
DAY 03 2018年11月人民币近半年贬值原因简析.doc
DAY 03 2018年11月人民币近半年贬值原因简析.pdf

./ACADEMY/Financial News/DAY 04 2018.11.11_10月初 央妈宣布全面降准:
DAY 04 2018.11.11_10月初 央妈宣布全面降准.doc
DAY 04 2018.11.11_10月初 央妈宣布全面降准.pdf

./ACADEMY/Financial News/DAY 05 2018.11.13_2019中国宏观经济走势展望_中美贸易摩擦影响:
DAY 05 2018.11.13_2019中国宏观经济走势展望_中美贸易摩擦影响.doc
DAY 05 2018.11.13_2019中国宏观经济走势展望_中美贸易摩擦影响.pdf

./ACADEMY/Financial News/DAY 06 2018.11.15_2019中国宏观经济走势展望_中美贸易摩擦影响_2:
DAY 06 2018.11.15_2019中国宏观经济走势展望_中美贸易摩擦影响_2.doc
DAY 06 2018.11.15_2019中国宏观经济走势展望_中美贸易摩擦影响_2.pdf

./ACADEMY/Financial News/DAY 07 2018.11.17_2019中国宏观经济走势展望_中美贸易摩擦影响_完整版:
DAY 07 2018.11.17_2019中国宏观经济走势展望_中美贸易摩擦影响_完整版.doc
DAY 07 2018.11.17_2019中国宏观经济走势展望_中美贸易摩擦影响_完整版.pdf

./ACADEMY/Financial News/DAY 08 2018.11.19_民主党夺回众议院之后:
DAY 08 2018.11.19_民主党夺回众议院之后.doc
DAY 08 2018.11.19_民主党夺回众议院之后.pdf

./ACADEMY/Financial News/DAY 09 2018.11.21_中美国债收益率倒挂_全球央行动态简析_01:
DAY 09 2018.11.21_中美国债收益率倒挂_全球央行动态简析.doc
DAY 09 2018.11.21_中美国债收益率倒挂_全球央行动态简析.pdf

./ACADEMY/Financial News/DAY 10 2018.11.23_中美国债收益率倒挂_全球央行动态简析_完整版:
DAY 10 2018.11.23_中美国债收益率倒挂_全球央行动态简析_完整版.doc
DAY 10 2018.11.23_中美国债收益率倒挂_全球央行动态简析_完整版.pdf

./ACADEMY/Financial News/DAY 11 2018.11.25_台湾地区“九合一”选举结果揭晓:
DAY 11 2018.11.25_台湾地区“九合一”选举结果揭晓.doc
DAY 11 2018.11.25_台湾地区“九合一”选举结果揭晓.pdf

./ACADEMY/Financial News/DAY 12 2018.11.27_大宗商品价格下跌_01:
DAY 12 2018.11.27_大宗商品价格下跌.doc

./ACADEMY/Financial News/DAY 13 2018.11.29_大宗商品价格下跌_美国退出伊朗核协议_完整版:
DAY 13 2018.11.29_大宗商品价格下跌_美国退出伊朗核协议_完整版.doc

./ACADEMY/Financial News/DAY 14 2018.12.01_大湾区对中国跨越中等收入陷阱将发挥重要作用:
DAY 14 2018.12.01_大湾区对中国跨越中等收入陷阱将发挥重要作用.doc
DAY 14 2018.12.01_大湾区对中国跨越中等收入陷阱将发挥重要作用.pdf

./ACADEMY/Financial News/DAY 15 2018.12.03_G20吃一顿饭的功夫,中美贸易战就结束了吗_01:
DAY 15 2018.12.03_G20吃一顿饭的功夫,中美贸易战就结束了吗_01.doc
DAY 15 2018.12.03_G20吃一顿饭的功夫,中美贸易战就结束了吗_01.pdf

./ACADEMY/Financial News/DAY 16 2018.12.05_G20吃一顿饭的功夫,中美贸易战就结束了吗_完整版:
DAY 16 2018.12.05_G20吃一顿饭的功夫,中美贸易战就结束了吗_完整版.doc
DAY 16 2018.12.05_G20吃一顿饭的功夫,中美贸易战就结束了吗_完整版.pdf

./ACADEMY/Financial News/DAY 17 2018.12.07_卡塔尔宣布退群！全球油价掌舵者闹分裂:
DAY 17 2018.12.07_卡塔尔宣布退群！全球油价掌舵者闹分裂.doc
DAY 17 2018.12.07_卡塔尔宣布退群！全球油价掌舵者闹分裂.pdf

./ACADEMY/Financial News/DAY 18 2018.12.09_证监会孙念瑞：强平对二级市场影响很小（简易版）:
DAY 18 证监会孙念瑞_强平对二级市场影响很小.docx

./ACADEMY/Financial News/DAY 19 2018.12.11_证监会孙念瑞：强平对二级市场影响很小_详细学习笔记:
DAY 19 2018.12.11_证监会孙念瑞：强平对二级市场影响很小_详细学习笔记.pdf

./ACADEMY/Financial News/DAY 20 2018.12.13_神仙打架之高通VS苹果and我们真的买不到iphone了吗_简略版:
DAY 20 2018.12.13_神仙打架之高通VS苹果and我们真的买不到iphone了吗_简略版.doc
DAY 20 2018.12.13_神仙打架之高通VS苹果and我们真的买不到iphone了吗_简略版.pdf

./ACADEMY/Financial News/DAY 21 2018.12.15_神仙打架之高通VS苹果and我们真的买不到iphone了吗_详细版:
DAY 21 2018.12.15_神仙打架之高通VS苹果and我们真的买不到iphone了吗_详细版.doc
DAY 21 2018.12.15_神仙打架之高通VS苹果and我们真的买不到iphone了吗_详细版.pdf

./ACADEMY/Financial News/DAY 22 2018.12.17_央妈连续近40个交易日未实施逆回购是什么情况:
DAY 22 2018.12.17_央妈连续近40个交易日未实施逆回购是什么情况.doc
DAY 22 2018.12.17_央妈连续近40个交易日未实施逆回购是什么情况.pdf

./ACADEMY/Financial News/DAY 23 2018.12.19 _央行重启逆回购:
DAY 23 2018.12.19 _央行重启逆回购.doc
DAY 23 2018.12.19 _央行重启逆回购.pdf

./ACADEMY/Financial News/DAY 24 2018.12.21 _2018年RMBS一骑绝尘增长超2倍:
DAY 24 2018.12.21 _2018年RMBS一骑绝尘增长超2倍.doc
DAY 24 2018.12.21 _2018年RMBS一骑绝尘增长超2倍.pdf

./ACADEMY/Financial News/DAY 25 2018.12.23 _2018年RMBS一骑绝尘增长超2倍 完整版:
DAY 25 2018.12.23 _2018年RMBS一骑绝尘增长超2倍 完整版.doc
DAY 25 2018.12.23 _2018年RMBS一骑绝尘增长超2倍 完整版.pdf

./ACADEMY/Financial News/DAY 26 2018.12.25 _一文读懂年终奖在个税新规下如何计税:
DAY 26 2018.12.25 _一文读懂年终奖在个税新规下如何计税.doc
DAY 26 2018.12.25 _一文读懂年终奖在个税新规下如何计税.pdf

./ACADEMY/Financial News/DAY 27 2018.12.27 _基金业新格局 part1:
DAY 27 2018.12.27 _基金业新格局 part1.doc
DAY 27 2018.12.27 _基金业新格局 part1.pdf

./ACADEMY/Financial News/DAY 28 2018.12.27 _基金业新格局_货基规模缩水_债基亮眼_完整版:
DAY 28 2018.12.27 _基金业新格局_货基规模缩水_债基亮眼_完整版.doc
DAY 28 2018.12.27 _基金业新格局_货基规模缩水_债基亮眼_完整版.pdf

./ACADEMY/Financial News/DAY 29 2018.12.31 _港交所全年IPO上市数量和募资额双冠全球:
DAY 29 2018.12.31 _港交所全年IPO上市数量和募资额双冠全球.doc
DAY 29 2018.12.31 _港交所全年IPO上市数量和募资额双冠全球.pdf

./ACADEMY/Thomas Calculus 13th with Solutions:
Thomas Calculus 13th [Solutions].pdf
Thomas Calculus 13th with Solutions.torrent
Thomas' Calculus 13th.pdf

./ANKI FLASHCARDS_MD:
2019秋季学期.md			Paper
ANKI FLASHCARDS_MD-README.md	Pronunciation
Adriene.md			Tips
Coding				Topics
FRM				Words

./ANKI FLASHCARDS_MD/Coding:
Algo Notes			ML
GitHub上面什么都有.md		深入浅出程序设计

./ANKI FLASHCARDS_MD/Coding/Algo Notes:
[AN] 0200 preface.md
[AN] 0201 数据类型(1:2)- 变量定义_类型_强制类型转换.md
[AN] 0201 数据类型(2:2)- 运算符.md
[AN] 0202 顺序结构1:3- 赋值表达式.md
[AN] 0202 顺序结构2:3- 使用scanf和printf输入输出.md
[AN] 0202 顺序结构3:3- 使用getchar和putchar输入:输出字符_typedef_math函数.md
[AN] 0203 选择结构 if_switch.md

./ANKI FLASHCARDS_MD/Coding/ML:
 机器学习分支.md
P02S05 MLR_Caveat.md
Part 0 - Welcome   .md
Part 1 - Data Preprocessing.md
Part 1 -[P]Data Preprocessing Template.md
Part 1 -[R] Data Preprocessing Template.md

./ANKI FLASHCARDS_MD/Coding/深入浅出程序设计:
[Notes]深入浅出程序设计.md

./ANKI FLASHCARDS_MD/FRM:
量化投资本土门派与国际门派的技术对比   .md

./ANKI FLASHCARDS_MD/Paper:
[1]文献检索和管理.md

./ANKI FLASHCARDS_MD/Pronunciation:
三分钟贵族式英语1_发音.md

./ANKI FLASHCARDS_MD/Tips:
Learning.png			天鹅臂动作要点.md
MAC 快捷键指南.md

./ANKI FLASHCARDS_MD/Topics:
On Creation.md				口译原则及练习.md
On Michael Fassbender.md		标题大小写问题.md
On my body.md				口译笔记法与口译注意.md
同声传译.md

./ANKI FLASHCARDS_MD/Words:
Dictation	Digest

./ANKI FLASHCARDS_MD/Words/Dictation:
2019-06-11.md	2019-06-17.md	2019-06-24.md	2019-07-08.md	2019-07-14.md
2019-06-12.md	2019-06-18.md	2019-06-25.md	2019-07-09.md	2019-07-15.md
2019-06-13.md	2019-06-19.md	2019-06-26.md	2019-07-10.md	2019-07-16.md
2019-06-14.md	2019-06-20.md	2019-06-27.md	2019-07-11.md	2019-07-17.md
2019-06-15.md	2019-06-22.md	2019-07-04.md	2019-07-12.md	2019-07-18.md
2019-06-16.md	2019-06-23.md	2019-07-07.md	2019-07-13.md	2019-07-19.md

./ANKI FLASHCARDS_MD/Words/Digest:
-2019-07-15.md			Continuing Education_terms.md

./AO3:
Advice for the young at.epub		Rick and Morty Get Real.pdf
Best Behaviour we wonder.epub		Shark Tank.epub
Cant control my reaction.epub		Skybird.txt
Coax me out my love low.epub		Wage Your War.epub
Consenting to Dream.epub		What a lovely way to.epub
De Profundis.epub			eb466112ly1fuofiezpjdj20u087o4qp.jpg
Enough.pdf				eb466112ly1fuofift1qbj20u087zb0x.jpg
Grave Diggers Wife.epub			eb466112ly1fuofigpr73j20u087xqgh.jpg
Grave Diggers Wife.pdf			eb466112ly1fuofihl1mfj20u08841fg.jpg
Lay your head down in my.epub		eb466112ly1fuofiigtk3j20u087v17n.jpg
Prey.pdf				eb466112ly1fuofij3eqtj20u077tk31.jpg
Reminiscence.pdf			notes.png
Rick and Morty Get Real.epub		写文的小notes.md

./AQF:
01 量化投资前导及课程介绍		03 Python语言环境搭建
02 量化投资基础				04 Python编程基础

./AQF/01 量化投资前导及课程介绍:
1.AQF核心课程知识体系介绍.mkv
2.量化策略的python实现和回测.mkv
3. 结合代码的编程整体介绍.mkv
AQF第01章.pdf

./AQF/02 量化投资基础:
01.量化投资背景及决策流程.mkv
02.量化择时.mkv
03.量化择时& 动量及反转策略.mkv
04.结构型基金套利.mkv
05.行业轮动与相对价值.mkv
06.市场中性和多因子.mkv
07.事件驱动.mkv
08.CTA_1.mkv
09.CTA_2（TD模型）.mkv
10.CTA_3.mkv
11.CTA_4.mkv
12.统计套利_低风险套利.mkv
13.大数据和舆情分析.mkv
14.机器学习.mkv
15.高频交易和期权交易.mkv
16.其他策略和策略注意点.mkv
讲义

./AQF/02 量化投资基础/讲义:
AQF第02章.pdf

./AQF/03 Python语言环境搭建:
1.Python语言环境搭建.mkv	讲义

./AQF/03 Python语言环境搭建/讲义:
AQF第03章.pdf
Anaconda + Pycharm 快速安装及基本使用说明_金程教育（更新完整版V）_Password_Removed.pdf

./AQF/04 Python编程基础:
01.python数字运算 and jupyter介绍.mkv
02.字符串.mkv
03.Python运算符.mkv
04.Tuple和List.mkv
05.字典.mkv
06.字符串格式化.mkv
07.控制结构_1.For循环.mkv
08.控制结构_2.If条件判断.mkv
09.控制结构_4.While循环.mkv
10.控制结构_3.Break&Continue.mkv
11.控制结构_5.异常处理.mkv
12.函数_1.质数函数.mkv
13.函数_2.参数设置.mkv
14.函数_3.不定长参数Lambda.mkv
15.全局变量和局部变量.mkv
16.模块.mkv
17.Python当中的重要函数.mkv
讲义

./AQF/04 Python编程基础/讲义:
1.1 Python语法的编程基础-数据基础.ipynb
1.2 Python语法的编程基础-控制结构和异常处理.ipynb
1.3 Python语法的编程基础-函数.ipynb
1.4 Python语法的编程基础-模块.ipynb
1.5 Python里面几个重要函数的用法.ipynb
AQF第04章.pdf
support.py

./BOOKS:
001(Bill Bryson) A short history of nearly everything.mobi
Clean Code-代码整洁之道.pdf
Crime and Punishment - Fyodor Dostoevsky.pdf
David goggins - Can’t hurt me.mobi
Economical Writing.pdf
Harry Potter
How to win friends and influence people.pdf
Jordan B. Peterson-12 Rules for Life_ An Antidote to Chaos-Random House Canada (2018).epub
Kristen Sosulski-Data Visualization Made Simple-Insights Into Becoming Visual Routledge.pdf
Malcolm Gladwell-Outliers_ The Story of Success-Little, Brown Young Readers (2008).epub
RenZhengfei-master
Verbal.Advantage.pdf
[John_C._Bogle,_William_T._Allen,_Paul_A._Volcker](b-ok.org).pdf
[John_Sandford]_Bad_Blood(b-ok.org).mobi
[Martin_George_R_R]_Fevre_Dream(z-lib.org).txt
[Stephen R. C. Hicks] Explaining Postmodernism Sk(z-lib.org).epub
[瑞典] 英格玛·伯格曼－《魔灯》.epub
[万物简史].A.Short.History.of.Nearly.Everything.pdf
thinkpython.pdf
金阁寺[日]三岛由纪夫+陈德文译.epub
我的天才女友.epub
新名字的故事.mobi
离开的，留下的.epub
美国人使用的一本GRE单词书（GRE Vocabulary ）.pdf
荣格论心理治疗与宗教_陈彪.pdf
香港怎麼了：佔中十七問.md
怦然心动的人生整理魔法（中文简体横版）.pdf

./BOOKS/Harry Potter:
Harry Potter and the Chamber of Secrets.epub
Harry Potter and the Deathly Hallows.epub
Harry Potter and the Goblet of Fire.epub
Harry Potter and the Half-Blood Prince.epub
Harry Potter and the Order of the Phoenix.epub
Harry Potter and the Prisoner of Azkaban.epub
Harry Potter and the Sorcerer’s Stone.epub

./BOOKS/RenZhengfei-master:
1994		2000		2006		2012		2018
1995		2001		2007		2013		R&D.md
1996		2002		2008		2014		README.md
1997		2003		2009		2015		SUMMARY.md
1998		2004		2010		2016
1999		2005		2011		2017

./BOOKS/RenZhengfei-master/1994:
19940118_赴美考察散记.md
19940126_团结奋斗_再创华为佳绩.md
19940605_胜利祝酒辞.md
19940621_对中国农话网与交换机产业的一点看法.md
19941225_致新员工书.md
19941225_从二则空难事故看员工培训的重要性.md

./BOOKS/RenZhengfei-master/1995:
19950109_坚定不移地坚持发展的方向.md
19950110_不前进就免职.md
19950110_英雄好汉站出来.md
19950110_励精图治，再创辉煌.md
19950618_上海电话信息技术和业务管理研讨会致谢词.md
199507_要建立一个均衡的平台.md
19951116_在第四届国际电子通信展华为庆祝酒会的发言.md
19951118_解放思想，迎接96年市场大战.md
19951226_目前我们的形势和任务.md

./BOOKS/RenZhengfei-master/1996:
19960128_当干部是一种责任.md
19960402_我们要向市场、开发、创造性工作倾斜.md
19960406_反骄破满，在思想上艰苦奋斗.md
19960502_加强合作走向世界.md
19960608_要树立服务意识、品牌意识、群体意识.md
19960630_再论反骄破满，在思想上艰苦奋斗.md
19960725_我们是要向前迈进一小步，而不是一次大飞跃.md
19960811_胜负无定数，敢搏成七分.md
19960828_赴俄参展杂记.md
19960828_秘书体系是信息桥.md
19961113_做好基础工作，逐步实现全面质量管理.md
19961115_实行低重心管理，层层级级都要在做实上下功夫.md
19961121_培训——通向华为明天的重要阶梯.md
19961202_管理改革，任重道远.md
19961213_坚持顾客导向同步世界潮流.md
19961228_团结起来接受挑战，克服自我溶入大我.md
1996_不要叶公好龙.md

./BOOKS/RenZhengfei-master/1997:
19970123_不要忘记英雄.md
19970207_资源是会枯竭的，唯有文化才能生生不息.md
19970217_加强用户服务中心建设，不断提高用户服务水平.md
19970222_秘书如何定位.md
19970226_坚定不移地推行ISO9000.md
19970226_胜则举杯相庆败则拼死相救.md
19970330_悼念杨琳.md
19970410_自强不息，荣辱与共，促进管理的进步.md
19970428_谈学习.md
19970428_走过亚欧分界线.md
199705_加强夏收管理促进增产增收.md
19970626_呼唤英雄.md
19970715_为提高电信网营运水平而努力.md
19970912_提升自我，找到切入点，迎接人生新挑战.md
19970916_当代青年怎样爱国.md
1997_我们需要什么样的干部.md
1997_苦练基本功，争做维护专家.md
1997_在《委员会管理法》评审上的重要讲话.md
1997_建立一个适应企业生存发展的组织和机制.md

./BOOKS/RenZhengfei-master/1998:
19980116_狭路相逢勇者生.md
1998012_不做昙花一现的英雄.md
19980220_我们向美国人民学习什么.md
19980328_要从必然王国，走向自由王国.md
199803_华为基本法.md
199803_在自我批判中进步.md
199805_希望寄托在你们身上.md
19980620_华为的红旗到底能打多久.md
19980716_小改进、大奖励.md
199809_全心全意对产品负责全心全意为客户服务.md
19981209_印度随笔.md
1998_把生命注入到产品中去.md

./BOOKS/RenZhengfei-master/1999:
19990208_创业创新必须以提升企业核心竞争力为中心.md
19990417_在IPD动员大会上的讲话.md
199904_在实践中培养和选拔干部.md
19990520_能工巧匠是我们企业的宝贵财富.md
19990520_“中国人今天说不”图片新闻感想.md
19990720_任正非答新员工问.md

./BOOKS/RenZhengfei-master/2000:
20000114_与身处逆境员工的对话录.md
20000128_凤凰展翅再创辉煌.md
20000320_一个职业管理者的责任和使命.md
20000408_活下去，是企业的硬道理.md
20000717_沟通从心灵开始.md
20000720_创新是华为发展的不竭动力.md
20000901_为什么要自我批判.md
2000_任正非在秘书资格颁证大会上的讲话.md

./BOOKS/RenZhengfei-master/2001:
20010118_雄赳赳气昂昂跨过太平洋.md
20010201_华为的冬天.md
20010208_我的父亲母亲.md
20010424_北国之春.md

./BOOKS/RenZhengfei-master/2002:
2002_迎接挑战，苦练内功，迎接春天的到来.md

./BOOKS/RenZhengfei-master/2003:
20030525_在理性与平实中存活.md
20030526_产品发展的路标是客户需求导向企业管理的目标是流程化的组织建设.md
2003_发挥核心团队作用，不断提高人均效益.md
2003_在自我批判指导委员会座谈会上的讲话.md

./BOOKS/RenZhengfei-master/2004:
20040115_持续提高人均效益建设高绩效企业文化.md
20040428_华为公司的核心价值观.md

./BOOKS/RenZhengfei-master/2005:
20050726_华为与对手做朋友海外不打价格战.md

./BOOKS/RenZhengfei-master/2006:
20060430_全流程降低成本和费用提高盈利能力.md
20060510_在华为收购港湾时的谈话纪要.md
20060719_我的青春岁月.md
20060721_天道酬勤.md
200608_冰岛游记.md
20060904_上甘岭是不会自然产生将军的但将军都曾经是英雄.md
20061120_华为大学要成为将军的摇篮.md
20061214_在BT系统部、英国代表处汇报会上的讲话.md
20061218_实事求是的科研方向与二十年的艰苦努力.md

./BOOKS/RenZhengfei-master/2007:
20070108_对区域监控工作的讲话纪要.md
20070108_财经的变革是华为公司的变革，不是财务系统的变革.md
200702_要快乐的度过充满困难的一生.md
20070315_在行政采购及信息安全问题座谈会上的讲话.md
20070409_听取艰苦地区生活专项问题汇报会上的讲话.md
20070612_以生动活泼的方式传递奋斗者为主体的文化.md
20070703_上甘岭在你心中，无论何时何地都可以产生英雄.md
20070713_敢于胜利，才能善于胜利.md
20070721_完善和提高对艰苦地区员工的保障措施.md
20070803_关于员工培训工作的谈话.md
20070808_变革最重要的问题是一定要落地.md
20070824_内控体系建设就是要穿美国鞋，不打补丁.md
20070914_将军如果不知道自己错在哪里，就永远不会成为将军.md

./BOOKS/RenZhengfei-master/2008:
20070728_珍惜生命，要从自己关爱自己做起.md
20080131_在EMT例会“08年公司业务计划与预算”汇报上的讲话.md
20080215_看莫斯科保卫战有感.md
20080410_人生是美好的，但过程确实是痛苦的.md
20080531_让青春的火花，点燃无愧无悔的人生.md
20080613_让青春的生命放射光芒.md
20080616_大家都是共和国的英雄.md
20080705_任正非在PSST体系干部大会上的讲话.md
20080715_逐步加深理解“以客户为中心，以奋斗者为本”的企业文化.md
20080721_在地区部向EMT进行2008年年中述职会议上的讲话.md
200807_理解国家，做好自己.md
20080902_从泥坑里爬起来的人就是圣人.md
20080922_从汶川特大地震一片瓦砾中，一座百年前建的教堂不倒所想到的.md
20081229_围绕客户PO打通，支撑“回款、收入、项目预核算”.md
2008_2008年新年祝词.md

./BOOKS/RenZhengfei-master/2009:
20090115_开放、妥协与灰度.md
20090116_让听得见炮声的人来决策.md
20090116_谁来呼唤炮火，如何及时提供炮火支援.md
20090206_任正非与IFS项目组及财经体系员工座谈纪要.md
20090312_在驻外行政人员培训交流沟通会上的座谈纪要.md
20090324_市场经济是最好的竞争方式，经济全球化是不可阻挡的潮流.md
20090327_任正非与PMS高端项目经理的座谈纪要.md
20090424_深淘滩，低作堰.md
20090827_具有“长期持续艰苦奋斗的牺牲精神，永恒不变的艰苦奋斗的工作作风”是成为一个将军最基本条件.md
20091026_CFO要走向流程化和职业化，支撑公司及时、准确、优质、低成本交付.md
20091127_加快CFO队伍建设，支撑IFS推行落地.md

./BOOKS/RenZhengfei-master/2010:
2000_以客户为中心，加大平台投入，开放合作，实现共赢.md
20091231_春风送暖入屠苏.md
20100120_以客户为中心，以奋斗者为本，长期坚持艰苦奋斗是我们胜利之本.md
20100304_在全球行政人员年度表彰暨经验交流大会座谈纪要.md
20100430_拉通项目四算，支撑项目层面经营管理.md
20100715_干部要担负起公司价值观的传承.md
20100910_开放、合作、自我批判，做容千万家的天下英雄.md
20101031_世博结束了，我们胜利了.md
20101125z_改善和媒体的关系.md
20101203_做事要霸气，做人要谦卑，要按消费品的规律，敢于追求最大的增长和胜利.md
20101206_五彩云霞飞遍天涯.md
20110104_以“选拔制”建设干部队伍，按流程梳理和精简组织，推进组织公开性和均衡性建设.md

./BOOKS/RenZhengfei-master/2011:
20110117_成功不是未来前进的可靠向导.md
20110223_关于珍爱生命与职业责任的讲话.md
20110414_华为关于如何与奋斗者分享利益的座谈会纪要.md
20110614_任总与罗马尼亚账务共享中心座谈会纪要.md
20110727_与华为大学第10期干部高级管理研讨班学员座谈纪要.md
20111019_任正非与财经体系员工座谈讲话.md
20111026_与同等学历认证班学员座谈纪要.md
20111031_力出一孔，要集中优势资源投入在主航道上，敢于去争取更大的机会与差距.md
20111225_一江春水向东流.md

./BOOKS/RenZhengfei-master/2012:
20120119_不要盲目扩张，不要自以为已经强大.md
20120319_绝对考核的目的是团结多数人.md
20120412_紧紧围绕客户，在战略层面宣传公司.md
20120423_董事会领导下的CEO轮值制度辨.md
20120712_中国没有创新土壤不开放就是死亡.md
201209_面向未来，以客户痛点为切入点，全球化展示.md
20121115_东南非多国管理部向任总汇报工作纪要.md
20121120_与毛里求斯员工座谈会议纪要.md
20121219_与华为大学教育学院座谈会纪要.md

./BOOKS/RenZhengfei-master/2013:
20121231_力出一孔，利出一孔.md
20130114_在小国表彰会上的讲话.md
20130219_任总和广州代表处座谈纪要.md
20130330_家人永远不接班.md
20130517_要敢于超越美国公司，最多就是输.md
20130527_在海外行政后勤服务管理思路汇报会上的讲话.md
20130627_财经流程建设向任总汇报纪要.md
20130719_要培养一支能打仗、打胜仗的队伍.md
20130723_在重装旅集训营座谈会上的讲话.md
20130904_在GTS客户培训服务座谈会上的讲话.md
20130905_最好的防御就是进攻.md
20130911_团结一切可以团结的力量.md
20130911_提倡节俭办晚会，节约会议成本.md
20130929_财经向任正非汇报纪要.md
20131019_用乌龟精神，追上龙飞船.md
20131031_与CEC成员座谈会的讲话.md
20131105_在GTS网规网优业务座谈会上的讲话.md
20131106_在华为大学教育学院工作汇报会上的讲话.md
20131111_在IP交付保障团队座谈会上的讲话.md
20131125_我一贯不是一个低调的人.md
20131129_在EMT办公例会上的讲话.md
20131204_在公司内控与风险管理“三层防线”优化方案汇报的讲话.md
20131219_关于“严格、有序、简化的认真管理是实现超越的关键”的座谈纪要.md
20131222_聚焦商业成功，英雄不问出处.md
20131228在运营商网络BG战略务虚会上的讲话及主要讨论发言.md
20131230_任正非在大规模消灭腐败进展汇报会上的讲话.md
2013_CFO标准与培养机制向任总汇报纪要.md

./BOOKS/RenZhengfei-master/2014:
20140105_风物长宜放眼量.md
20140113_做谦虚的领导者.md
20140122_在董事赋能研讨会上与候选专职董事交流讲话.md
20140129_握紧拳头才有力量.md
20140219_自我批判，不断超越.md
20140225_在外派伙食补助汇报会上的讲话.md
20140307_在关于重装旅组织汇报会议上的讲话.md
20140311_在大机会时代，千万不要机会主义.md
20140314三年，从士兵到将军.md
20140327_在华大建设思路汇报会上的讲话.md
20140331_在日本研究所工作汇报会上的讲话.md
20140409_与巴西代表处及巴供中心座谈纪要.md
20140410_在巴西代表处的讲话.md
20140411_在秘鲁代表处座谈会上的讲话.md
20140413_在拉美北地区部、哥伦比亚代表处工作汇报会上的讲话.md
20140416_在华为上研所专家座谈会上的讲话.md
20140424_在后备干部项目管理与经营短训项目座谈会上的讲话.md
20140502_英国媒体会谈纪要.md
20140509_喜马拉雅山的水为什么不能流入亚马逊河.md
20140509_简化管理，选拔使用有全局观的干部，数据及信息透明.md
20140510_在巡视松山湖制造现场的讲话纪要.md
20140513_推动行政服务业务变革，试点流程责任制.md
20140527_在海外子公司董事会推行工作汇报会上的讲话.md
20140603_在丹麦代表处员工座谈会上的讲话.md
20140604_在西欧地区部工作汇报会上的讲话.md
20140605_在德国LTC教导队训战班座谈会上的讲话.md
20140606_在保加利亚代表处工作汇报会上的讲话.md
20140616_为什么我们今天还要向“蓝血十杰”学习.md
20140619_洞庭湖装不下太平洋的水.md
20140624_在人力资源工作汇报会上的讲话.md
20140624_在“关于内部网络安全工作方向“的决议.md
20140707_第一次就把事情做对.md
20140723_在变革项目激励政策汇报会上的讲话.md
20140723_在小国综合管理变革汇报会上的讲话.md
20140723_在项目管理资源池第一期学员座谈会上的讲话.md
20140725_在2014年7月25日EMT办公会议上的讲话.md
20140826_在销售项目经理资源池第一期学员座谈会上的讲话.md
20140923_在公司近期激励导向和激励原则汇报会上的讲话.md
20140923_在“班长的战争”对华为的启示和挑战汇报会上的讲话.md
201409_在多个汇困国家调研中的讲话.md
20141104_与CEC就非物质激励工作优化的座谈纪要.md
20141104_在行政流程责任制试点进展汇报会上的讲话.md
20141106_遍地英雄下夕烟，六亿神州尽舜尧.md
20141114_坚持为世界创造价值，为价值而创新.md
20141205_在“从中心仓到站点打通”工作汇报会上的讲话.md
20141218_依托欧美先进软件包构建高质量的IT系统.md
20141218在艰苦地区及岗位管理部工作汇报会上的讲话.md

./BOOKS/RenZhengfei-master/2015:
20150108_在与法务部、董秘及无线员工座谈会上的讲话.md
20150109_打造运营商BG“三朵云”，将一线武装到牙齿.md
20150116_变革的目的就是要多产粮食和增加土地肥力.md
20150125_最大的敌人是我们自己.md
20150127_改善艰苦地区条件，加快循环赋能，为公司筑起第二道防线.md
20150310_非主航道组织要率先实现流程责任制，通过流程责任来选拔管理者，淘汰不作为员工，为公司管理进步摸索经验.md
20150318_在2015年全球行政工作年会上的讲话.md
20150331_在变革战略预备队进展汇报上的讲话.md
20150408_埃森哲董事长Pierre拜访任正非的会谈纪要.md
20150504_在变革战略预备队及进展汇报座谈上的讲话.md
20150506_与BCG顾问交流会谈纪要.md
20150508_在变革战略预备队誓师及颁奖典礼上的座谈纪要.md
20150515_在监管重装旅座谈会上的讲话.md
20150520_在公司质量工作汇报会上的讲话.md
20150702_在固网产业趋势及进展汇报会上的讲话.md
20150713_在合同场景师建设思路汇报上的讲话.md
20150713_在子公司监督型董事会管理层监督方案及试点情况汇报上的讲话.md
20150714_与英国研究所、北京研究所、伦敦财经风险管控中心座谈的纪要.md
20150730_在战略预备队业务汇报上的讲话.md
20150731_在变革战略预备队第三期誓师典礼上的讲话.md
20150812_构建先进装备，沉淀核心能力，在更高维度打赢下一场战争.md
20150827_脚踏实地，做挑战自我的长跑者.md
20150828_在2015年8月28日EMT办公会议上的讲话.md
20150902_在波士顿咨询汇报行政服务变革（国家驻点成果及未来变革方向）的讲话.md
20150906_任正非接受福布斯中文网采访.md
20150907_在战略预备队誓师典礼暨优秀队员表彰大会上的讲话.md
20150923_在公共及政府事务部2015年工作汇报会的讲话.md
20150924_在2015年9月24日EMT办公会议上的讲话.md
20150928_在GTS站点信息库、地理信息库、网络动态运行信息库和集成交付平台建设汇报会上的讲话.md
201509致新员工书.md
20151010_最终的竞争是质量的竞争.md
20151023_将军是打出来的.md
20151023_在调查工作授权及流程优化汇报上的讲话.md
20151027_小国要率先实现精兵战略，让听得见炮声的人呼唤炮火.md
20151031_聚焦主航道，在战略机会点上抢占机会.md
20151218_彭剑锋专访任正非纪要.md

./BOOKS/RenZhengfei-master/2016:
20160113_决胜取决于坚如磐石的信念，信念来自专注.md
20160118_变革的目的就是更简单、更及时、更准确.md
20160125_在2016年1月25日EMT办公会议上的讲话.md
20160214_做“成吉思汗的马掌”，支撑我们服务世界的雄心.md
20160223_巴塞罗那通信展小型恳谈会纪要.md
20160227_多路径多梯次跨越“上甘岭”攻进无人区.md
20160305_28年只对准一个城墙口冲锋.md
20160307_关于改善艰苦国家的作战环境.md
20160331_在巴展总结会议上的讲话.md
20160405_与日本代表处、日本研究所员工座谈纪要.md
20160428_在专业服务业务策略汇报上的讲话.md
20160505_任正非与Fellow座谈会上的讲话.md
20160523_在中亚地区部员工座谈会上的讲话.md
20160528_为祖国百年科技振兴而努力奋斗.md
20160530_以创新为核心竞争力，为祖国百年科技振兴而奋斗.md
20160712_前进的路上不会铺满了鲜花.md
20160804_在签证业务变革进展汇报上的讲话.md
20160805_聚焦战略平台，加强血液流动，夺取未来胜利.md
20160810_在诺亚方舟实验室座谈会上的讲话.md
20160813_IPD的本质是从机会到商业变现.md
20160815_公司必须持续不断的、永恒的促进组织血液流动，增强优秀干部、专家的循环赋能.md
20160819_美丽的爱尔兰是软件的大摇篮.md
20161021_关于行政与慧通工作讲话的纪要.md
20161025_建立对作业类员工的科学管理方法与评价体系，导向多产粮食.md
20161026_在质量与流程IT管理部员工座谈会上的讲话.md
20161026_在运营商三朵云2.0阶段进展汇报会上的讲话.md
20161028_春江水暖鸭先知，不破楼兰誓不还.md
20161031_聚焦主航道，眼望星空，朋友越多天下越大.md
201610_在中亚（塔吉克斯坦、土耳其、白俄）代表处汇报会议上的讲话.md
20161115_聚焦平台，加强血液流动，敢于破格，抢占世界高地.md
20161121_与合同场景师座谈会上的讲话.md
20161130_人力资源政策要朝着熵减的方向发展.md
20161201_内外合规多打粮，保驾护航赢未来.md
20161217_在法国美学研究所的讲话.md
20161217_在法国研究所座谈交流纪要.md
20161222_在存货账实相符项目汇报会上的讲话.md

./BOOKS/RenZhengfei-master/2017:
20170107_在人工智能应用GTS研讨会上的讲话.md
20170111_在2017年市场工作大会上的讲话.md
20170117_在消费者BG年度大会上的讲话.md
20170120_在健康指导中心业务变革项目阶段汇报会上的讲话.md
201701_在北部非洲（尼日尔、布基纳法索）汇报会议的讲话.md
20170203_在厄瓜多尔代表处的讲话.md
20170205_在玻利维亚代表处的讲话.md
20170206_在巴拉圭的讲话.md
20170215_在泰国与地区部负责人、在尼泊尔与员工座谈的讲话.md
20170220_在泛网络区域组织变革优化总结与规划汇报的讲话.md
20170224_在高研班和战略预备队汇报会上的讲话.md
20170314_我们的目的是实现高质量.md
20170316_客户需求导向，提升公司E2E系统竞争力.md
20170327_在公司监督与管控体系延伸建设思考汇报会上的讲话.md
20170328_在支付系统员工座谈会上的讲话.md
20170406_与广州代表处部分员工晚餐会的讲话.md
20170410_与网络能源产品线部分员工晚餐会的讲话.md
20170418_在战略预备队座谈会上的讲话.md
20170424_在道德遵从委员会第二次代表大会的讲话.md
20170427_在职员类定位与差异化管理汇报会上的讲话.md
201704_在哈佛商学院全球高管论坛上的演讲.md
20170527_在继任计划工作汇报会上的讲话.md
20170527_在健康指导与应急保障业务整合及签证变革进展汇报会上的讲话.md
20170601_什么叫精神文明，什么叫物质文明.md
20170602_方向要大致正确，组织要充满活力.md
20170621_与任总在曼谷座谈纪要.md
20170622_与德国代表处交流纪要.md
20170623_与波兰代表处交流纪要.md
20170624_在俄罗斯代表处讲话纪要.md
20170705_在华为平安园区项目汇报会上的讲话.md
20170711_在战略预备队述职会上的讲话.md
20170712_在三季度区域总裁会议上的讲话.md
20170712_在新员工入职培训座谈会上的讲话.md
20170718_与韩国办事处交流纪要.md
20170723_任正非与徐直军在消费者BG2017年中市场大会上的讲话.md
20170807_在人力资源管理纲要2.0沟通会上的讲话.md
20170807_在行政服务解决“小鬼难缠”工作进展汇报上的讲话.md
20170807_科学的量化、简化管理，关注技能与经验的积累，培育工匠文化.md
20170809_在子公司监督型董事会年中工作会议上的讲话.md
20170816_在冰岛与四位弟兄咖啡细语.md
20170821_在规范职能组织权力工作组座谈会上的讲话.md
20170824_与采购干部座谈会上的讲话.md
20170826_开放创新，吸纳全球人才，构建“为我所知、为我所用、为我所有”的全球能力布局.md
20170828_在诺亚方舟实验室使能工程部成立会上的讲话.md
20170829_任总在GTS人工智能实践进展汇报会上的讲话.md
20170829_在“合同在代表处审结”工作汇报会上的讲话.md
20170906_在英国代表处的讲话.md
20170913_任总在伦敦FRCC听取贸易合规和金融合规汇报的讲话.md
20170914_任总与接入网团队座谈会上的讲话.md
20170917_在捷克代表处讲话.md
20171003_在加拿大代表处的讲话.md
20171006_一杯咖啡吸收宇宙能量，一桶浆糊粘接世界智慧.md
20171018_在会议标准化及服务提升项目汇报会上的讲话.md
20171019_在2017年第四季度地区部总裁会议上的讲话.md
20171024_在消费者BG业务汇报及骨干座谈会上的讲话.md
20171113_关于人力资源管理纲要2.0修订与研讨的讲话纪要.md
20171120_在公司愿景与使命研讨会上的讲话.md
20171211_什么是“一杯咖啡吸收宇宙能量'.md
20171213_什么是确定性工作.md
20171215_确定性工作精细化、自动化.md
20171218_在落实日落法及清理机关说NO.md
20171219_熵减的过程是痛苦的，前途是光明的.md
20171225_在听取展厅工作汇报时，关于咨询师的讲话.md

./BOOKS/RenZhengfei-master/2018:
20180116_在财务部分员工座谈会上的讲话.md
20180117_从泥坑中爬起来的是圣人.md
20180118_与财务、基建、行政座谈会上的讲话.md
20180205_与“落实日落法及清理机关说NO”秘书处座谈会上的讲话.md
20180209_在员工关系变革工作进展汇报上的讲话.md
20180223_在斯里兰卡代表处的讲话.md
20180224_从系统工程角度出发规划华为大生产体系架构，建设世界一流的先进生产系统.md
20180302_在蒙古办事处汇报会议上的讲话.md
20180314_任正非在2018年全球行政年会上的座谈纪要.md
20180321_研发要做智能世界的“发动机”.md
20180411_在黎巴嫩代表处的讲话.md
20180420_关于人力资源组织运作优化的讲话.md
20180426_任正非在战略预备队述职会上的讲话.md
20180515_励精图治，十年振兴.md
20180605_在剑桥和伊普斯维奇研究所座谈纪要.md
20180622_BG机关要缩短经线，畅通纬线，强化作战组织的能力考核与选拔，精减非作战组织的规模及运作.md
20180623_在2018年IRB战略务虚研讨会的讲话.md
20180627_与平台协调委员会座谈纪要.md
20180701在卢旺达饭店与员工聊天记录.md
20180713_在攀登珠峰的路上沿途下蛋.md
20180718在GTS人工智能实践进展汇报会上的讲话.md
20180929_从人类文明的结晶中，找到解决世界问题的钥匙.md
20181017_坚持多路径、多梯次、多场景化的研发路线，攻上“上甘岭”，实现5G战略领先.md
20181019_鼓足干劲，力争上游，不畏一切艰苦困苦.md
20181107_寂寞的英雄是伟大的英雄，我们要鼓励新旧循环.md
20181119_加强与国内大学合作，吸纳全球优秀人才，共同推动中国基础研究.md
20181121_任正非在日本研究所业务汇报.md

./ENGLISH:
006JSwchgy1fk06q9a0hqj30hs0p3q4d.jpg
006fQkcJly1flfcudng4rj30go0yzqbz.jpg
006fQkcJly1flfcuekmzsj30go15447q.jpg
006fQkcJly1flfcuel18zj30go0yu46v.jpg
006fQkcJly1flfcuel30rj30go18ldqf.jpg
006fQkcJly1flfcuew47sj30go10p10y.jpg
006fQkcJly1flfcufjkyvj30go0y3jzn.jpg
006fQkcJly1flfcufjzmoj30go0ztwml.jpg
006fQkcJly1flfcufl99tj30go0xwqbb.jpg
006fQkcJly1flfcufv525j30go0znjz9.jpg
006iOs7dly1g0couj0byqj30bu0lgq3m.jpg
006iOs7dly1g0couj625qj30c80mggmo.jpg
006iOs7dly1g0coujbq2kj30bi0m8750.jpg
006iOs7dly1g0coujfxmaj30bu0ioaan.jpg
006iOs7dly1g0coujk57vj30c20jujs1.jpg
006iOs7dly1g0coujoshwj30bs0m8wf3.jpg
006iOs7dly1g0couju6hlj30c40m6wfb.jpg
006iOs7dly1g0coujym2hj30bm0m8aau.jpg
006iOs7dly1g0couk3e5oj30ag0k6q3i.jpg
6bd5ced9gy1fz3z0hli9fj20vw184b29.jpg
7e4923ddly1fyudmjnombj22ao328kjm.jpg
7e4923ddly1fyudmo5vdzj22ao328x6q.jpg
7e4923ddly1fyudmsqe31j22ao328hdu.jpg
7e4923ddly1fyudmw4vm6j22ao328e82.jpg
7e4923ddly1fyudmzej9cj22ao328npe.jpg
7e4923ddly1fyudn2mmixj22ao328npe.jpg
Cambridge English Grammar in Use [Advanced].pdf
English Vocabulary in Use.pdf
[新概念英语]pdf全四册
d7534598gy1fydmbddf0aj20ku0k8tdh.jpg
d7551e98gy1ftn6ujryxqj20ku0vaadn.jpg
小3000电子版.xlsx
【Cambridge】English Vocabulary in Use-Upper-intermediate.pdf
口语.jpg
口语2.jpg
口语3.jpg
丘吉尔
杨鹏《GRE&GMAT阅读难句教程》.pdf
发音练习
屏幕快照 2019-07-29 下午7.43.51.png
屏幕快照 2019-07-29 下午8.15.38.png
屏幕快照 2019-07-29 下午8.15.54.png
屏幕快照 2019-07-29 下午8.16.09.png
屏幕快照 2019-07-29 下午8.16.25.png
屏幕快照 2019-07-29 下午8.18.14.png
屏幕快照 2019-07-29 下午8.18.42.png
屏幕快照 2019-07-29 下午8.22.03.png
屏幕快照 2019-07-29 下午8.22.36.png
屏幕快照 2019-07-29 下午8.22.51.png
屏幕快照 2019-07-29 下午8.23.35.png
屏幕快照 2019-07-29 下午8.24.17.png
屏幕快照 2019-07-29 下午8.24.31.png
屏幕快照 2019-07-29 下午8.25.26.png
屏幕快照 2019-07-29 下午8.26.29.png
屏幕快照 2019-07-29 下午8.26.50.png
屏幕快照 2019-07-29 下午8.27.09.png
屏幕快照 2019-07-29 下午8.27.26.png
屏幕快照 2019-07-29 下午8.28.02.png
屏幕快照 2019-07-29 下午8.28.13.png
屏幕快照 2019-07-29 下午8.28.25.png
屏幕快照 2019-07-29 下午8.28.59.png
屏幕快照 2019-07-29 下午8.29.23.png
屏幕快照 2019-07-29 下午8.29.47.png
英汉视译.pdf
阅读方法论.md
考研英语词汇 — 熟词僻义.pdf
猴哥托福词汇excel背诵版4.0.xls
考研英语形近词.pdf
背单词，记住这200个词根词缀就够了.pdf
英语高分手写笔记
考研写作核心词汇分类总结.pdf
林超伦实战口译笔记实例详解.doc
史上最详尽解释的考研英语熟词僻义词 .pdf

./ENGLISH/[新概念英语]pdf全四册:
新概念1.pdf	新概念2.pdf	新概念3.pdf	新概念4.pdf

./ENGLISH/丘吉尔:
Germany invades Russia.docx		speech to the allied delegates.docx
Germany invades Russia.mp3		speech to the allied delegates.mp3
Germany's unconditional surrender.docx	their finest hour.docx
Germany's unconditional surrender.mp3	their finest hour.mp3
blood, toil, tears and sweat.docx	war with Japan.docx
blood, toil, tears and sweat.mp3	war with Japan.mp3
meeting with Roosevelt.docx		we shall fight on the beaches.docx
meeting with Roosevelt.mp3		we shall fight on the beaches.mp3

./ENGLISH/发音练习:
Comma Gets A Cure.mp3	英音 男.mp3		口语练习.pdf

./ENGLISH/英语高分手写笔记:
15页大小作文冲刺QQ2516605455.pdf	7页完型填空QQ2516605455.pdf
20页大小作文笔记QQ2516605455.pdf	考研英语词汇笔记.pdf
6页翻译+新题型QQ2516605455.pdf		英语考研高分手写笔记.pdf

./MATHS:
006JSwchgy1fl99kbf27fj30r80qon31.jpg
006JSwchgy1fmgpqiothej30kp0xd46p.jpg
006JSwchgy1fmiey6z0zfj30yi0cqmz5.jpg
006JSwchgy1fmjz6m5iooj30r90qoafx.jpg
006JSwchgy1fmkm2if71nj30ck0a4q3k.jpg
006JSwchgy1fmn6uan2tnj30gm08cta0.jpg
006JSwchgy1fssgr0yzd2j30ol0g2k2e.jpg
006JSwchgy1fssgr1juzij30nk0h7k19.jpg
006JSwchgy1fssgr9o7n4j30fe05iglj.jpg
006JSwchgy1fwseid84glj30u01hc4ea.jpg
006JSwchgy1fwseidh693j30yi1ba78q.jpg
2019张宇高等数学18讲.pdf
2019考研数学接力题典1800 数学三 解答册 汤家凤.pdf
2019考研数学接力题典1800 数学三 题目册 汤家凤.pdf
2019考研数学高等数学基础讲义.pdf
214-1P53015235U62.png
67f6d06fjw1eb4gesulqoj20nxc9pe82.jpg
6a63f6246b600c337915a9c3134c510fd9f9a149.jpg.png
7ab38b28gy1fsz602yi2rj22c03407wh.jpg
7ab38b28gy1fsz605y4h7j22c0340e81.jpg
7ab38b28gy1fsz608sl7jj22c0340e81.jpg
7ab38b28gy1ft86i1ke92j22c03401kx.jpg
7ab38b28gy1fun4287vv9j21w02iou0x.jpg
7ab38b28gy1fun42cda6dj21f01w0x6r.jpg
7ab38b28gy1fun42gkiv6j21f01w0qv8.jpg
7ab38b28gy1fwhe5f5k9mj22c03404qp.jpg
7ab38b28gy1fwhe5hpt3ij22c0340hbf.jpg
7ab38b28gy1fwhe5keafhj22c03404qp.jpg
7ab38b28gy1fwhe5n0i16j22c03407wh.jpg
7ab38b28gy1fwhe5ozryjj22c03407wh.jpg
7ab38b28gy1fwhe5so222j22c03404qp.jpg
7ab38b28gy1fwhe5vnfnjj22c03407wh.jpg
7ab38b28gy1fwhe5y20guj22c0340tzi.jpg
7ab38b28gy1fwhe607m2jj22c03407wh.jpg
7ab38b28gy1fwtwo7uzupj21r00r4kjl.jpg
7ab38b28gy1fwuoqoe5muj22c0340tx4.jpg
7ab38b28gy1fwuore5fytj22c0340qqk.jpg
7ab38b28gy1fwuqyv7j8xj22c01r04qt.jpg
7ab38b28gy1fwuqyxy4eij22c01r01l1.jpg
7ab38b28gy1fy9wqxt8c5j20qo0zkag7.jpg
7ab38b28gy1fy9wqycqqdj20qo0zkjy1.jpg
7ab38b28gy1fy9wqyqcykj20qo0zkq93.jpg
7ab38b28gy1fy9wqzf4lxj20qo0zkgrf.jpg
7ab38b28ly1ftr371a587j22c03407wh.jpg
7ab38b28ly1ftrnxr45j1j22c0340b29.jpg
7ab38b28ly1ftwzlo0wm1j22c03404qp.jpg
8afbb187ly1frh16hcledj23402c0hdt.jpg
Mean of Sample Variance 样本方差的证明.jpg
timg (1).jpeg
屏幕快照 2018-03-03 下午9.22.17.png
屏幕快照 2018-07-28 下午3.28.45.png
总链接文档 19.3- .docx
希腊字母读音.jpg
高等数学证明题500例.pdf
考研数学公式大全.pdf
张宇带你学线性代数同济六版.pdf
张宇带你学概率论与数理同济浙大四版.pdf
张宇带你学高等数学同济七版（上册）.pdf
张宇带你学高等数学同济七版（下册）.pdf

./Machine Learning A-Z Chinese Template Folder:
Part 0 - Welcome to Machine Learning A-Z
Part 1 - Data Preprocessing
Part 10 - Model Selection & Boosting
Part 2 - Regression
Part 3 - Classification
Part 4 - Clustering
Part 5 - Association Rule Learning
Part 6 - Reinforcement Learning
Part 7 - Natural Language Processing
Part 8 - Deep Learning
Part 9 - Dimensionality Reduction

./Machine Learning A-Z Chinese Template Folder/Part 0 - Welcome to Machine Learning A-Z:
Section 1 - Welcome to Machine Learning A-Z !

./Machine Learning A-Z Chinese Template Folder/Part 0 - Welcome to Machine Learning A-Z/Section 1 - Welcome to Machine Learning A-Z !:

./Machine Learning A-Z Chinese Template Folder/Part 1 - Data Preprocessing:
Section 2 -------------------- Part 1 - Data Preprocessing --------------------

./Machine Learning A-Z Chinese Template Folder/Part 1 - Data Preprocessing/Section 2 -------------------- Part 1 - Data Preprocessing --------------------:
Data_Preprocessing

./Machine Learning A-Z Chinese Template Folder/Part 1 - Data Preprocessing/Section 2 -------------------- Part 1 - Data Preprocessing --------------------/Data_Preprocessing:
Data.csv				data_preprocessing_template.R
My Data Preprocessing Template.R	data_preprocessing_template.py
My Data Preprocessing Template.py	missing_data.R
categorical_data.R			missing_data.py
categorical_data.py

./Machine Learning A-Z Chinese Template Folder/Part 10 - Model Selection & Boosting:
Section 39 -------------------- Part 10 - Model Selection --------------------
Section 40 - Model Selection
Section 41 - XGBoost
Section 42 - Part Recap

./Machine Learning A-Z Chinese Template Folder/Part 10 - Model Selection & Boosting/Section 39 -------------------- Part 10 - Model Selection --------------------:

./Machine Learning A-Z Chinese Template Folder/Part 10 - Model Selection & Boosting/Section 40 - Model Selection:

./Machine Learning A-Z Chinese Template Folder/Part 10 - Model Selection & Boosting/Section 41 - XGBoost:

./Machine Learning A-Z Chinese Template Folder/Part 10 - Model Selection & Boosting/Section 42 - Part Recap:

./Machine Learning A-Z Chinese Template Folder/Part 2 - Regression:
Section 3 -------------------- Part 2 - Regression --------------------
Section 4 - Simple Linear Regression
Section 5 - Multiple Linear Regression
Section 6 - Polynomial Regression
Section 7 - Evaluating Regression Models Performance
Section 8 - Part Recap

./Machine Learning A-Z Chinese Template Folder/Part 2 - Regression/Section 3 -------------------- Part 2 - Regression --------------------:

./Machine Learning A-Z Chinese Template Folder/Part 2 - Regression/Section 4 - Simple Linear Regression:
[0] Salary_Data.csv
[1] simple_linear_regression.py
[2] My SLR.py
[3] SLR_2.py
[4] Salary VS Experience (trainning set).png
[5] Salary VS Experience (test set).png
[6]simple_linear_regression.R

./Machine Learning A-Z Chinese Template Folder/Part 2 - Regression/Section 5 - Multiple Linear Regression:
50_Startups.csv
Homework_Solutions
P46-Step-by-Step-Blueprints-For-Building-Models.pdf
multiple_linear_regression.R
multiple_linear_regression.py

./Machine Learning A-Z Chinese Template Folder/Part 2 - Regression/Section 5 - Multiple Linear Regression/Homework_Solutions:
50_Startups.csv			multiple_linear_regression.R
data_preprocessing_template.R	multiple_linear_regression.py
data_preprocessing_template.py

./Machine Learning A-Z Chinese Template Folder/Part 2 - Regression/Section 6 - Polynomial Regression:
Position_Salaries.csv		polynomial_regression.py
polynomial_regression.R

./Machine Learning A-Z Chinese Template Folder/Part 2 - Regression/Section 7 - Evaluating Regression Models Performance:

./Machine Learning A-Z Chinese Template Folder/Part 2 - Regression/Section 8 - Part Recap:

./Machine Learning A-Z Chinese Template Folder/Part 3 - Classification:
Section 10 - Logistic Regression
Section 11 - Support Vector Machine (SVM)
Section 12 - Kernel SVM
Section 13 - Naive Bayes
Section 14 - Decision Tree Classification
Section 15 - Random Forest Classification
Section 16 - Evaluating Classification Models Performance
Section 17 - Part Recap
Section 9 -------------------- Part 3 - Classification --------------------

./Machine Learning A-Z Chinese Template Folder/Part 3 - Classification/Section 10 - Logistic Regression:

./Machine Learning A-Z Chinese Template Folder/Part 3 - Classification/Section 11 - Support Vector Machine (SVM):

./Machine Learning A-Z Chinese Template Folder/Part 3 - Classification/Section 12 - Kernel SVM:

./Machine Learning A-Z Chinese Template Folder/Part 3 - Classification/Section 13 - Naive Bayes:

./Machine Learning A-Z Chinese Template Folder/Part 3 - Classification/Section 14 - Decision Tree Classification:

./Machine Learning A-Z Chinese Template Folder/Part 3 - Classification/Section 15 - Random Forest Classification:

./Machine Learning A-Z Chinese Template Folder/Part 3 - Classification/Section 16 - Evaluating Classification Models Performance:

./Machine Learning A-Z Chinese Template Folder/Part 3 - Classification/Section 17 - Part Recap:

./Machine Learning A-Z Chinese Template Folder/Part 3 - Classification/Section 9 -------------------- Part 3 - Classification --------------------:

./Machine Learning A-Z Chinese Template Folder/Part 4 - Clustering:
Section 18 -------------------- Part 4 - Clustering --------------------
Section 19 - K-Means Clustering
Section 20 - Part Recap

./Machine Learning A-Z Chinese Template Folder/Part 4 - Clustering/Section 18 -------------------- Part 4 - Clustering --------------------:

./Machine Learning A-Z Chinese Template Folder/Part 4 - Clustering/Section 19 - K-Means Clustering:

./Machine Learning A-Z Chinese Template Folder/Part 4 - Clustering/Section 20 - Part Recap:

./Machine Learning A-Z Chinese Template Folder/Part 5 - Association Rule Learning:
Section 21 -------------------- Part 5 - Association Rule Learning --------------------
Section 22 - Apriori
Section 23 - Part Recap

./Machine Learning A-Z Chinese Template Folder/Part 5 - Association Rule Learning/Section 21 -------------------- Part 5 - Association Rule Learning --------------------:

./Machine Learning A-Z Chinese Template Folder/Part 5 - Association Rule Learning/Section 22 - Apriori:

./Machine Learning A-Z Chinese Template Folder/Part 5 - Association Rule Learning/Section 23 - Part Recap:

./Machine Learning A-Z Chinese Template Folder/Part 6 - Reinforcement Learning:
Section 24 -------------------- Part 6 - Reinforcement Learning --------------------
Section 25 - Upper Confidence Bound (UCB)
Section 26 - Thompson Sampling
Section 27 - Part Recap

./Machine Learning A-Z Chinese Template Folder/Part 6 - Reinforcement Learning/Section 24 -------------------- Part 6 - Reinforcement Learning --------------------:

./Machine Learning A-Z Chinese Template Folder/Part 6 - Reinforcement Learning/Section 25 - Upper Confidence Bound (UCB):

./Machine Learning A-Z Chinese Template Folder/Part 6 - Reinforcement Learning/Section 26 - Thompson Sampling:

./Machine Learning A-Z Chinese Template Folder/Part 6 - Reinforcement Learning/Section 27 - Part Recap:

./Machine Learning A-Z Chinese Template Folder/Part 7 - Natural Language Processing:
Section 28 -------------------- Part 7 - Natural Language Processing --------------------
Section 29 - Natural Language Processing
Section 30 - Part Recap

./Machine Learning A-Z Chinese Template Folder/Part 7 - Natural Language Processing/Section 28 -------------------- Part 7 - Natural Language Processing --------------------:

./Machine Learning A-Z Chinese Template Folder/Part 7 - Natural Language Processing/Section 29 - Natural Language Processing:

./Machine Learning A-Z Chinese Template Folder/Part 7 - Natural Language Processing/Section 30 - Part Recap:

./Machine Learning A-Z Chinese Template Folder/Part 8 - Deep Learning:
Section 31 -------------------- Part 8 - Deep Learning --------------------
Section 32 - Artificial Neural Networks (ANN)
Section 33 - Convolutional Neural Networks (CNN)
Section 34 - Part Recap

./Machine Learning A-Z Chinese Template Folder/Part 8 - Deep Learning/Section 31 -------------------- Part 8 - Deep Learning --------------------:

./Machine Learning A-Z Chinese Template Folder/Part 8 - Deep Learning/Section 32 - Artificial Neural Networks (ANN):

./Machine Learning A-Z Chinese Template Folder/Part 8 - Deep Learning/Section 33 - Convolutional Neural Networks (CNN):

./Machine Learning A-Z Chinese Template Folder/Part 8 - Deep Learning/Section 34 - Part Recap:

./Machine Learning A-Z Chinese Template Folder/Part 9 - Dimensionality Reduction:
Section 35 -------------------- Part 9 - Dimensionality Reduction --------------------
Section 36 - Principal Component Analysis (PCA)
Section 37 - Kernel PCA
Section 38 - Part Recap

./Machine Learning A-Z Chinese Template Folder/Part 9 - Dimensionality Reduction/Section 35 -------------------- Part 9 - Dimensionality Reduction --------------------:

./Machine Learning A-Z Chinese Template Folder/Part 9 - Dimensionality Reduction/Section 36 - Principal Component Analysis (PCA):

./Machine Learning A-Z Chinese Template Folder/Part 9 - Dimensionality Reduction/Section 37 - Kernel PCA:

./Machine Learning A-Z Chinese Template Folder/Part 9 - Dimensionality Reduction/Section 38 - Part Recap:
(base) appledeMacBook-Air-3:C apple$ 

```

可以使用 `clear`指令来**清屏**。

## 其他功能

- **不要进入休眠状态：**当你临时不希望电脑进入休眠状态时，可以使用 `caffeinate` 命令让电脑时刻清醒。当你需要其恢复正常时，按下 `⌃Control - C` 即可停止该命令。


- **程序假死需要强退：**有时候程序假死了，强行退出也没用，这时可以使用 `killall` 命令。以微信为例，若想强退它，只需输入 `killall WeChat` 即可。


- **截图保存为 JPEG：**Mac 的默认截图格式为 PNG，若你想让默认的截图保存类型为 JPEG，可以输入如下指令 `defaults write com.apple.screencapture type jpg`，结果如下图所示，以后的截图都会变成 JPEG 格式。如果你希望撤销这条指令，输入 `defaults write com.apple.screencapture type png` 即可。
- **整理程序栏：**你也许会发现，底部的程序栏越用越乱，有时候内容多的半天找不到所需程序。这时你可以考虑为其加入几个隐藏的分界符将其归为几个区域，输入：`defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'; killall Dock`即可添加一个空白分界符，需要几个重复运行几遍命令即可。当你不需要这个白分界符了，将它从程序栏拖走即可删除。


- **显示隐藏文件夹：**在你跟着网络上的教程进行一些操作时，难免会遇到让你寻找隐藏文件夹的情况，这时你可以使用：`defaults write com.apple.finder AppleShowAllFiles -bool true; killall Finder`来显示所有隐藏文件夹，当你不需要再显示时，输入：`defaults write com.apple.finder AppleShowAllFiles -bool false; killall Finder`即可恢复隐藏。查看下图，你会发现所有隐藏文件夹全部显示出来了。


- **关闭截图自动阴影：** 若你使用 Mac 自带的截图，会发现每次的窗口截图均会自动添加阴影，当你需要后期处理这些图片时，这些阴影可能会对你造成困扰。你可以使用下面这串命令来关闭截图阴影：`defaults write com.apple.screencapture disable-shadow -bool true; killall SystemUIServer`当你希望重新启动阴影时，可以输入：`defaults write com.apple.screencapture disable-shadow -bool false; killall SystemUIServer`查看下方的截图，你就会发现它和本文的其他截图不同，没有阴影。
- **打印机械感十足的文字：**当你想要打出机械感十足的文字时，可以玩玩`banner -w 80 legolas.me`这句命令，只需要将代码结尾处的文字替换为你想打印的字即可。
- **修改文件日期：** 有时你可能需要修改文件创建或修改日期，这时可以使用 `touch -t 199505090000 拖入文件`命令。这句命令中的数字表示 1995 年 5 月 9 日 00:00 分，你可以根据实际需要修改。


- ### 文件格式转换 textutil

  textutil 是一个系统自带的，用于**处理文稿**的命令，其中我最常用的功能是其下属功能 convert，这句指令允许你将任何文件，在以下文件格式中互相转换 txt, html, rtf, rtfd, doc, docx, wordml, odt, webarchive, md。

  若你手头有一篇 DOCX 文件需要被转换成 TXT，则可以输入 `textutil -convert txt 文件路径`，这句代码中的 txt 处，可以替换为任何你需要转换到的文件格式，文件路径则可以采用拖拽文件到终端的方法自动填充。
---
title: 不正经与正经的《R语言统计学基础》说明
published: true
comments: true
layout: post
---

这里提供本人在清华大学出版社出版的《R语言统计学基础》的相关说明，分不正经版和正经版两种，读者可各取所好、随意阅读。本文随时保持更新，如果您发现之前阅读的内容不翼而飞，请不要感到惊讶。选择GitHub平台发布此文，即表明我对文中内容不垄断编辑专有权。因此，如果您对此中观点感到愤怒，不妨注册GitHub在此文中与我直接PK。如果您知道如何科学上网，也可在文末直接评论，评论需要注册[Disqus](https://disqus.com/)账号。我虽“贵”为文科出身，但中英文语法都不好，高考语文可能前10道选择题错了7道，只凭感觉来写作；所以如果文中出现各种稀奇古怪的文字与句法错误，大约是因为我用了某狗的五笔输入法所致。

全书的勘误请见[这里](https://xkdog.github.io/2017-03-23-Errata/)，如想提交勘误，请点击[这里](https://github.com/xkdog/xkdog.github.io/blob/master/_posts/2017-03-23-Errata.md)。勘误过程会使用简单的LaTeX语法，在此先行谢过。如不熟悉GitHub和LaTeX操作，也可直接发信至xkdog@126.com说明。

![cover](https://images-cn.ssl-images-amazon.com/images/I/61wcEf4ElmL.jpg)


# 不正经的简介（An Unorthodox Introduction）


## 缘起

[本书](https://www.amazon.cn/%E6%95%B0%E9%87%8F%E7%BB%8F%E6%B5%8E%E5%AD%A6%E7%B3%BB%E5%88%97%E4%B8%9B%E4%B9%A6-R%E8%AF%AD%E8%A8%80%E7%BB%9F%E8%AE%A1%E5%AD%A6%E5%9F%BA%E7%A1%80-%E5%90%95%E5%B0%8F%E5%BA%B7/dp/B06XGR6LJZ/ref=sr_1_1?ie=UTF8&qid=1490843285&sr=8-1&keywords=%E5%90%95%E5%B0%8F%E5%BA%B7)是[我](http://zfxy.nankai.edu.cn/xk)在编写基础本科统计教材方面的一个新尝试，主要面向研究型大学的社会科学和行为科学类学生编著。说它“新”，主要是因为从基本教学理念和统计工具方面与以往的教材相比，存在诸多的不同之处；说它是“尝试”，主要是因为很难说这种处理就是最完善的，而是一种试验性的探索过程。作为个人，出于所谓的敝帚自珍心态也罢，出于社会心理学里常讲的[“基本归因谬误”](https://en.wikipedia.org/wiki/Fundamental_attribution_error)也罢，当然坚信目前这种方式“代表”着未来的潮流，希望能够得到更多的呼应与支持，也欢迎真挚的批评与建议。这里将此中心路历程做一简单介绍，读者或可从中感悟一二。


约10来年前，由于阴差阳错的机会，我参与到美国大学先修课程（[Advanced Placement](http://apcentral.collegeboard.com/home)）、尤其是其中的[Calculus AB & BC和Statistics](http://apcentral.collegeboard.com/apc/public/courses/teachers_corner/index.html)两门课程在中国大陆的推广与培训过程。在历次[AP Annual Conference](https://apac.collegeboard.org/)的研讨会中，我频繁接触美国大学入门数学类、统计类课程的教学理念、课堂组织、教材体系和评分标准等问题，感觉深有启发。与此同时，在面向中国拟留美攻读本科学位的大陆高中生、以及我在南开大学周恩来政府管理学院的本职统计类教学科目的教学实践中，在自己于社会学、心理学领域的实证社会科学研究的经验体悟中，我开始深度反思如何为中国的研究型大学的本科生撰写一本能够具有时代特征的统计教材。

期间的2013年，还顺带在中国人民大学出版社出版了中英双语版的[《AP微积分基础教程》](https://www.amazon.cn/%E5%9B%BE%E4%B9%A6/dp/B00B1ZUG4I/ref=sr_1_3?ie=UTF8&qid=1490852616&sr=8-3&keywords=%E5%90%95%E5%B0%8F%E5%BA%B7)和[《AP统计学基础教程》](https://www.amazon.cn/%E5%9B%BE%E4%B9%A6/dp/B00BZLMJ98/ref=sr_1_2?ie=UTF8&qid=1490852616&sr=8-2&keywords=%E5%90%95%E5%B0%8F%E5%BA%B7)，算是投石问路之作，此时面向的对象仅是拟出国留学的高中生。当时不知天高地厚，有种“王侯将相、宁有种乎”的心迹，颇有匹马称雄之意。当然现在看来，很多都是心气过高而力气不够时的狂语。书中多处错讹，如今看来皆是笑话。然书稿撰写过程中深受Word中反复使用Mathtype插入数学公式之苦，遂发愤（确定是此“愤”而非彼“奋”）自学了一阵LaTeX，显然不求甚解，勉强基本入门，算是一个最大的意外收获。

同时，在2011年前后，不知何处听得一个名字很“二”的统计软件，名之为`R`，性格中的不安分因子就开始在冥冥之中四处悸动。于是在本该用于享受生活的各种茶余饭后美好时光中，我在各种概率、统计、`R`、`Rstudio`、`LaTeX`等符号与数字的教材森林里“叫嚣乎东西、隳突乎南北”，穿梭于各种正规不正规的论坛求助；中间多少无人求解的苦处，也只化为一意孤行地强装笑颜，以此砥砺前行。为逼自己入定`R`坑，我又逼迫自己开设相关的硕士和本科课程，以半桶水之内存、晃叮当响之信号，拽人入坑，名为“教学相长”，实为拉人垫背、强行洗脑。中间又发表几篇相关的低水平“学术论文”——当然还有被毙掉的更多，这使我更清醒地认识到自己的种种不足，足以彻底放弃所谓的智商优越感。但不论同行评议如何糟糕，勉强在心中为自己划定了个名分：此生或可投身于社会科学类的统计教育与普及工作。世上有人生为开天辟地者，创造新观念、新工具、新物种，此种人雄才大略、可望不可即；也有一些人只是传播者，受某种事物之感召，自愿追随其后、为其之流行贡献绵薄之力。这可能就是我的定位。此中过程虽无实质建树，但可乐此不疲。我不是意义驱动的人，不过意义裹胁的人生；然而这并不意味着人生就此失去目的和方向。此中真义，欲辩忘言。

再后来，由于系里的张阔副教授出国进修，需要有人代上心理统计课程。我就承接了这一教学任务。之前在院里开设`R`语言统计课程时，重点均在软件学习与使用，使用的都是他人的教材。接手心理统计课程时，觉得已有教材能跟`R`匹配的实在太少，教材内容上也存在诸多不理想之处。于是就想：何不造个让自己觉得称手的“工具”出来？譬如孙猴子，没有一根如意金箍棒，恐怕就不能随意捣蛋。一来二去，讲义就变成了书稿，遂想干脆集结出版。心意既动，只能催着自己拼命赶路。中间也曾后悔多次，不该事先跟学生夸下海口“要写一本全面超越既有教材的教材”、导致自己骑虎难下。到后来只能不时动用意志力逼迫自己完成书稿。以心理学术语而言，这中间确有诸多的自我损耗（[ego depletion](https://en.wikipedia.org/wiki/Ego_depletion)）；“强”（此为勉强之强、而非强劲之强）弩之末，姿态本已分外妖娆，何况期间亦总有世事纷扰，一点随机扰动就可能成为压倒骆驼的最后一颗稻草。原来的序言中有一句，后因篇幅原因删去了，这里抄录如下：

    从意气风发地开篇到再三踌躇地结稿，此间诸多波折，竟令我等庸人之资，不时悟得John von Neumann的神人心迹：	

    If people do not believe that mathematics is simple, it is only because they do not realize how complicated life is.

    也不知该喜该悲。

凡此各种，遂有此书。当然，更多心路，还可参见“言不尽意”一节及正式“序言”一节。

## 资源链接

本书所有的相关PDF课件、数据、附录等内容可通过以下[网盘链接](https://pan.baidu.com/s/1Sx0ZHQDlt9dHBiZssiEF5A)(提取码：4cal)公开分享。有时你可能会看到存在不同的分享链接，可能是因为我建立了多个分享目录所致，内容应无实质区别；又或者可能发现原书序言中的链接已经失效，可能是我误删或其他不明原因所致。此时可致信xkdog@126.com直接向我询问相关资料信息。本书的其他相关资料，将陆续存放于本人的[GitHub目录](https://github.com/xkdog/StatsUsingR)，敬请光临浏览。

本书的PDF课件由南开大学社会心理学系2013级本科生张光耀、柳婷基于Texlive平台下的Beamer模板制作完成，在此表示由衷的感谢。如有任何错误，请直接联系本人。PDF格式比较简陋，希望各位注重领会“精神”而非“外在”。

本人另外撰写了约130页的教材中所有相关习题的详细解答，为保证教学有效性以及选用本教材进行课堂教学的教师进行作业管理的需要，此件暂不主动公开。如您还是学生，在未完成相关章节的练习之前，请不要向我发邮件索取。如果您是老师，如您说明相关身份（最好能够显示您的电子邮件地址的所在学院官方网页链接），我可发送相关附件，以便进行习题布置，并请批评指正；如果您想在我提供的课件基础上制作内容更为丰富的课件，也可给我邮件，我可提供所有课件的Tex文档与源图片，以便您使用LaTeX编辑器生成新的PDF课件。


## 致歉 & 致谢


由于本人的学识与细致有限，本书仍存在不少原本可以避免的失误。全书的勘误请见[这里](https://xkdog.github.io/2017-03-23-Errata/)，想要提交勘误意见烦请移步[这里](https://github.com/xkdog/StatsUsingR/blob/master/Errata.md)。这些都通过[GitHub](https://github.com/)平台和各种免费网络存储平台发布。我诚恳地建议各统计学的新手与老鸟、旁观者与爱好者，都能充分地感受和学习[R](https://www.r-project.org/)、[Rstudio](https://www.rstudio.com/)和[GitHub](https://github.com/)等计算化、网络化工具带来的便利，尽管这些工具的学习过程可能充满各种猥琐心结。

感谢本书责任编辑、清华大学出版社编辑部张伟老师的慧眼与精心。本书初稿既定，我斟酌再三，向“素未谋面”的清华大学出版社发出邮件，征询出版意向。几日后即收到张老师的回邮，很快便签订了出版合同并进入校对流程。有时张老师半夜仍与我微信联系、讨论书中存在的问题，如此无视作息基本法的行为让我再一次感慨清华人的辛勤风范。“业精于勤荒于嬉，行成于思毁于随”，我以为这是至理名言，不论对天才或常人。本书从提交书稿到最终出版，不过半年时间（若非遇上16年底的雾霾，还可更加提前）。清华大学出版社的专业与高效，给我留下深刻的印象。但愿我的书稿，不会辜负这其中的种种宽容与错爱。

今后如有精力和人手，会进一步完善相关教材资料，例如：

* 制作`.RMD`格式的课件，包含所有`R`代码，方便进行网页化展示。
* 制作更多更有新意的统计练习题并提供答案。
* 编写`.RMD`格式的、更简洁的关于数据导入、清洗与操纵的R语言使用说明并提供相关练习。
* 利用`Rstudio`与`shiny`制作动态呈现概率论与统计学知识的网页App。
* ……（反正吹牛不上税，不凡多列几个点）


## 言不尽意

出于各种可以理解和未必可以理解的原因，短短篇幅不能说尽我对当下统计教学的种种意见与牢骚。更多不负责任的八卦与胡说，欢迎私下场合当面与我交流对质、互通有无。当是时也，或有二三子，可以赞、可以弹、可以讽、可以狂，意欣欣然、飘飘然、熏熏然，而皆不足为外人道也。统计工具的妙处，或正在可暂束个人情感好恶于高阁，转而求诸一定之方。用时下流行的[Kahneman](http://www.princeton.edu/~kahneman/)等诸神之[认知双系统理论](https://en.wikipedia.org/wiki/Dual_process_theory)，即在于压制直觉系统（系统1）的启发式、转而寻求分析系统（系统2）的精准推理。有人谓此“方枘圆凿、缘木求鱼”，某只回曰：知我者谓我心忧，不知我者谓我何求。不同道而强相谋，何如相忘于江湖。

最后，作为一名严格意义上的文科生（如果您不介意，可以点击这里[考证](https://github.com/xkdog/xkdog.github.io/blob/master/_posts/2017-04-06-gossips.md)，阅读后果自负），我对祖国文字“御敌于千里、杀人于无形”的力量恐惧尤深。以致若非必要，极力否定在标准化的文体中加入个人色彩；作为推崇科学思维和统计方法（我以为两者并不是一回事）的研究者，我以为其行文的基本原则应是：不要用终极意义之类“绝对正确”的框架来要挟他人、不要诉诸情感的力量来感化他人、不要用文字的魅力来争取他人——凡此种种，皆为报刊体、网文体（如知音体、南周体、知乎体等）中刀笔小吏的奇技淫巧，只可小玲珑，未可雄泰华。学术文章就应当八股化、格式化、规范化，追求“千人一面”，使一千个读者只读出一个标准的哈姆雷特。

然而，事实总证明人有两面性或多面性——这个不正经的介绍本身就高度情绪化和不规范化，既可能间接戳中诸位的阅读痛点，也直接违反自己定下的三观。那下面就提供一个官方版本的简介，给各位列官压压惊，以便诸位虎躯一震，抖擞出山。


# 正经的介绍：出版序言

与正儿八经的介绍相比, 我更想说的是: 这是一本有思想、有技术、说“人话”的新一代概率统计与数据分析入门教材. 我希望读者在阅读此书之后, 能够明白统计方法并不简单的只是一种硬邦邦、冷冰冰的“客观方法”, 而是一种严谨且有弹性的思维方式; 学习统计方法的过程是一种处处充满惊喜的智力探索过程: 通过严格而系统的训练, 逐一打开统计方法的黑箱. 

为此, 本书努力在以下几个方面体现自身特色, 以充分拓展学生的数据想象力与分析力. (1) 贯彻统计思想重于统计计算的基本教学理念. 本教材的主要目的并不是培养专业统计研究人才, 而是培养学生理性而健全的统计思维模式, 以及使用基本统计方法解决本学科领域的实际问题的能力. (2) 以实证数据处理为中心阐述基本统计内容.  教材的主要内容完全针对行为与社会科学中的实际研究情境设计, 例子和习题同时具有可读性和知识性, 注重从一手文献、大型社会调查中提取相关数据作为训练数据. (3) 补充国内同类教材目前尚较为少见的重要内容, 这主要包括抽样分布产生、实验数据的随机化检验、自助分布置信区间、效应值与统计功效等内容. (4) 重视统计数据和统计结果的可视化呈现, 全书利用`R`语言绘制了100多个统计图形, 旨在培养学生的图形思维能力. (5) 强调统计结果的合理表达, 使普通读者能够更好地理解统计公式与计算结果在现实世界中的含义. 

本书的第1章和第2章是传统概率论的内容, 此部分内容需要一元函数微积分学的基础. 第3章开始介绍统计学的内容. 一般而言, 统计学可分为两大块: 描述性统计(Descriptive Statistics)和推论性统计(Inferential Statistics). 描述性统计是有关数据采集、组织和呈现的统计学分支, 主要涉及统计数字记录和归总、统计指标建立、统计图表制作等内容, 其重点在于两个方面: (1) 数据的数字特征的概括, 也就是集中趋势与离散趋势的概括; (2) 统计图表的制作与理解. 本书对各种统计指标背后的构造思想进行深入的剖析, 并结合`R`软件说明其应用. 

推论性统计学主要涉及如何从样本数据推论到总体数据的工作. 通常而言, 我们不可能针对研究对象的全体、即总体做研究, 而只可能根据总体的某个子集、即样本做研究, 并且希望将根据样本得到的信息, 来归纳和推论总体的信息. 本书的所有推论统计观点都基于频率学派的研究, 这涉及第4--7章. 其中, 第4章讨论的抽样分布是推论统计学习的重点和难点, 是社会科学研究中反事实框架的一个具体形式. 第5章和第6章分别介绍参数估计和假设检验的内容. 同时, 本教材还介绍了随机化实验中常用的推论框架: 随机化分布, 并介绍了最近几十年发展迅速的自助法置信区间及`R`语言实现, 以拓展学生的统计视野与软件技能. 第7章主要介绍线性模型的基础内容, 这主要包括线性回归和方差分析两大部分. 限于篇幅与自身学识, 本书并未涉及频率学派统计学之外的贝叶斯统计学的基本观点. 

本书文字写作基于`Texlive 2015`平台, 统计分析和图形绘制基于`Rstudio`平台. 本书并不刻意回避英文. 涉及的概率统计人物均不做翻译, 直接以英语出现. 关键术语均注明英文原文, 以便检索. 例题和练习中的变量名称也多用英文, 这是为了与`R`中的变量命名原则相匹配. 本书所涉及的所有数据可从[网盘链接](https://pan.baidu.com/s/1Sx0ZHQDlt9dHBiZssiEF5A)(提取码：4cal)下载.

本教材多数章节的内容在出版之前, 已作为内部讲义在南开大学周恩来政府管理学院各专业作为内部讲义试用. 由衷感谢各界本科生和研究生同学对本教材内容与表述方式的改进建议. 尤其要感谢(以下排名不分先后)我的助教、博士生张慧娟和王丛, 我的硕士生曹松峰、贾婷, 2015级南开大学应用心理学全体学术硕士, 以及我指导过的本科生付英涛、陈丹忆、李亚静、张光耀、柳婷、荣杨、彭芷晴、付鑫鹏、穆蔚琦、杨旋、刘奕男、孙超然、隋晓阳等同学. 他们协助我校订了讲义中的文字、公式、例题和习题, 同时还帮助我撰写了部分章节的`LaTeX`文档与`R`语言操作说明, 并共同设计了部分练习题. 在此特别要向这些热心好学的学生致以诚挚的谢意! 

感谢南开大学社会心理学系及周恩来政府管理学院诸位师长和同事对我的宽容, 使我能够自由地探索和实践自己的教学思想. 感谢张阔副教授的信任, 使我得以全程尝试用`R`软件进行心理统计课程教学的机会. 还要感谢教材例题与习题中“神出鬼没”、备受调侃的“柴教授”的原型, 我的同门师弟柴民权博士. 他虽已是兰州大学管理学院的教师, 仍不改逗萌本色为本书贡献了“柴教授”的著名绰号, 以其独特方式证明他的持久影响力. 

撰写此书虽已尽全力, 成书在即仍旧诚惶诚恐. 既恐出现纰漏, 贻笑方家; 更恐误人子弟, 罪莫大焉. 相关建议或批评, 可直接发至本人邮箱xkdog@126.com交流探讨. 如需更多国内外教学资料、统计习题、`R`代码和考试试题, 也可直接发信索取, 我可承诺做到知无不言、全面分享. 

最后, 用我很喜欢的一句英文谚语做为结尾吧:

> Throw your hat over the fence! （直译：先把你的帽子扔过墙！）

这样你就有了翻墙而上的勇气. 

吕小康

2016年8月31日, 于南开大学津南校区

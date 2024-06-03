---
layout: post
title: csdiy，计算机学习
categories: 计算机
description: False
keywords: 计算机，网课
mermaid: false
sequence: false
flow: false
mathjax: false
mindmap: false
mindmap2: false
---

![Image title](https://cdn.jsdelivr.net/gh/Halerfermatqing/images_bed@main/typora/202406031531579.png)

# 前言

**最近更新：[Release v1.1.0](https://github.com/PKUFlyingPig/cs-self-learning/releases/tag/v1.1.0) 已发布 🎉**

这是一本计算机的自学指南，也是对自己大学三年自学生涯的一个纪念。

这同时也是一份献给北大信科学弟学妹们的礼物。如果这本书能对你们的信科生涯有哪怕一丝一毫的帮助，都是对我极大的鼓励和慰藉。

本书目前包括了以下部分(如果你有其他好的建议，或者想加入贡献者的行列，欢迎邮件 [zhongyinmin@pku.edu.cn](mailto:zhongyinmin@pku.edu.cn) 或者在 issue 里提问)：

- 本书使用指南：由于书内涵盖资源众多，我根据不同人群的空闲时间和学习目标制定了对应的使用指南。
- 一份供参考的 CS 学习规划：我根据自己的自学经历制定的全面的、系统化的 CS 自学规划。
- 必学工具：一些 CSer 效率工具介绍，例如 IDE, 翻墙, StackOverflow, Git, GitHub, Vim, LaTeX, GNU Make, Docker, 工作流 等等。
- 经典书籍推荐：你是否苦于教材的晦涩难懂不知所云？别从自己身上找原因了，可能只是教材写得太烂。看过 CSAPP 这本书的同学一定会感叹好书的重要，我将列举推荐各个计算机领域的必看好书与资源链接。
- **国内外高质量 CS 课程汇总**：我将把我上过的以及开源社区贡献的**高质量**的国内外 CS 课程分门别类进行汇总，介绍其课程内容特点并给出相应的自学建议，大部分课程都会有一个独立的仓库维护相关的资源以及作业实现供大家学习参考。

## 梦开始的地方 —— CS61A

大一入学时我是一个对计算机一无所知的小白，装了几十个 G 的 Visual Studio 天天和 OJ 你死我活。凭着高中的数学底子我数学课学得还不错，但在专业课上对竞赛大佬只有仰望。提到编程我只会打开那笨重的 IDE，新建一个我也不知道具体是干啥的命令行项目，然后就是 `cin`, `cout`, `for` 循环，然后 CE, RE, WA 循环。当时的我就处在一种拼命想学好但不知道怎么学，课上认真听讲但题还不会做，课后做作业完全是用时间和它硬耗的痛苦状态。我至今电脑里还存着自己大一上学期计算概论大作业的源代码 —— 一个 1200 行的 C++ 文件，没有头文件、没有类、没有封装、没有 unit test、没有 Makefile、没有 Git，唯一的优点是它确实能跑，缺点是“能跑”的补集。我一度怀疑我是不是不适合学计算机，因为童年对于极客的所有想象，已经被我第一个学期的体验彻底粉碎了。

这一切的转机发生在我大一的寒假，我心血来潮想学习 Python。无意间看到知乎有人推荐了 CS61A 这门课，说是 UC Berkeley 的大一入门课程，讲的就是 Python。我永远不会忘记那一天，打开 [CS61A](https://cs61a.org/) 课程网站的那个瞬间，就像哥伦布发现了新大陆一样，我开启了新世界的大门。

我一口气 3 个星期上完了这门课，它让我第一次感觉到原来 CS 可以学得如此充实而有趣，原来这世上竟有如此精华的课程。

为避免有崇洋媚外之嫌，我单纯从一个学生的视角来讲讲自学 CS61A 的体验：

- 独立搭建的课程网站: 一个网站将所有课程资源整合一体，条理分明的课程 schedule、所有 slides, homework, discussion 的文件链接、详细明确的课程给分说明、历年的考试题与答案。这样一个网站抛开美观程度不谈，既方便学生，也让资源公正透明。
- 课程教授亲自编写的教材：CS61A 这门课的开课老师将 MIT 的经典教材 *Structure and Interpretation of Computer Programs* (SICP) 用Python这门语言进行改编（原教材基于 Scheme 语言），保证了课堂内容与教材内容的一致性，同时补充了更多细节，可以说诚意满满。而且[全书开源](https://www.composingprograms.com/)，可以直接线上阅读。
- 丰富到让人眼花缭乱的课程作业：14 个 lab 巩固随堂知识点，10 个 homework，还有 4 个代码量均上千行的 project。与大家熟悉的 OJ 和 Word 文档式的作业不同，所有作业均有完善的代码框架，保姆级的作业说明。每个 Project 都有详尽的 handout 文档、全自动的评分脚本。CS61A 甚至专门开发了一个[自动化的作业提交评分系统](https://okpy.org/)（据说还发了论文）。当然，有人会说“一个 project 几千行代码大部分都是助教帮你写好的，你还能学到啥？”。此言差矣，作为一个刚刚接触计算机，连安装 Python 都磕磕绊绊的小白来说，这样完善的代码框架既可以让你专注于巩固课堂上学习到的核心知识点，又能有“我才学了一个月就能做一个小游戏了！”的成就感，还能有机会阅读学习别人高质量的代码，从而为自己所用。我觉得在低年级，这种代码框架可以说百利而无一害。就是苦了老师和助教，因为开发这样的作业可想而知需要相当大的时间投入和多年的迭代积累。
- 每周 Discussion 讨论课：助教会讲解知识难点和考试例题，习题全部用 LaTeX 撰写，相当规范并且会给出详细的解答，让学生及时查漏补缺巩固知识点。

这样的课程，你完全不需要任何计算机的基础，你只需要努力、认真、花时间就够了。此前那种有劲没处使的感觉，那种付出再多时间却得不到回报的感觉，从此烟消云散。这太适合我了，我从此爱上了自学。

试想如果有人能把艰深的知识点嚼碎嚼烂，用生动直白的方式呈现给你，还有那么多听起来就很 fancy，种类繁多的 project 来巩固你的理论知识，你会觉得他们真的是在倾尽全力想方设法地让你完全掌握这门课，你会觉得不学好它简直是对这些课程建设者的侮辱。

如果你觉得我在夸大其词，那么不妨从 [CS61A](https://cs61a.org/) 开始，因为它是我的梦开始的地方。

## 为什么写这本书

在我2020年秋季学期担任《深入理解计算机系统》（CSAPP）这门课的助教时，我已经自学一年多了。这一年多来我无比享受这种自学模式，为了分享这种快乐，我为自己的研讨班学生做过一个 [CS自学资料整理仓库](https://github.com/PKUFlyingPig/Self-learning-Computer-Science)。当时纯粹是心血来潮，因为我也不敢公然鼓励大家翘课自学。

但随着又一年时间的维护，这个仓库的内容已经相当丰富，基本覆盖了计科、智能系、软工系的绝大多数课程，我也为每个课程都建了各自的 GitHub 仓库，汇总我用到的自学资料以及作业实现。

直到大四开始凑学分毕业的时候，我打开自己的培养方案，我发现它已经是我这个自学仓库的子集了，而这距离我开始自学也才两年半而已。于是，一个大胆的想法在我脑海中浮现：也许，我可以打造一个自学式的培养方案，把我这三年自学经历中遇到的坑、走过的路记录下来，以期能为后来的学弟学妹们贡献自己的一份微薄之力。

如果大家可以在三年不到的时间里就能建立起整座 CS 的基础大厦，能有相对扎实的数学功底和代码能力，经历过数十个千行代码量的 Project 的洗礼，掌握至少 C/C++/Java/JS/Python/Go/Rust 等主流语言，对算法、电路、体系、网络、操统、编译、人工智能、机器学习、计算机视觉、自然语言处理、强化学习、密码学、信息论、博弈论、数值分析、统计学、分布式、数据库、图形学、Web开发、云服务、超算等等方面均有涉猎。我想，你将有足够的底气和自信选择自己感兴趣的方向，无论是就业还是科研，你都将有相当的竞争力。

因为我坚信，既然你能坚持听我 BB 到这里，你一定不缺学好 CS 的能力，你只是没有一个好的老师，给你讲一门好的课程。而我，将力图根据我三年的体验，为你挑选这样的课程。

## 自学的好处

对我来说，自学最大的好处就在于可以完全根据自己的进度来调整学习速度。对于一些疑难知识点，我可以反复回看视频，在网上谷歌相关的内容，上 StackOverflow 提问题，直到完全将它弄明白。而对于自己掌握得相对较快的内容，则可以两倍速甚至三倍速略过。

自学的另一大好处就是博采众长。计算机系的几大核心课程：体系、网络、操统、编译，每一门我基本都上过不同大学的课程，不同的教材、不同的知识点侧重、不同的 project 将会极大丰富你的视野，也会让你理解错误的一些内容得到及时纠正。

自学的第三个好处是时间自由。大学的课余时间本就相对自由，再加上不用去上课的话更是可以放飞自我地安排自学时间和进度。我大二的时候赶上疫情在家窝了大半年，返校之后也基本没有线下去过教室上课，对绩点也毫无影响。

## 自学的坏处

当然，作为 CS 自学主义的忠实拥趸，我不得不承认自学也有它的坏处。

第一就是交流沟通的不便。我其实是一个很热衷于提问的人，对于所有没有弄明白的点，我都喜欢穷追到底。但当你面对着屏幕听到老师讲了一个你没明白的知识点的时候，你无法顺着网线到另一端向老师问个明白。我努力通过独立思考和善用 Google 来缓解这一点，但是，如果能有几个志同道合的伙伴结伴自学，那将是极好的。关于交流群的建立，大家可以参考仓库 `README` 中的教程。

第二就是这些自学的课程基本都是英文的。从视频到课件再到作业全是英文，所以有一定的门槛。我尽量在汇总课程视频资源的时候寻找带中文字幕的搬运视频，但大多数课程还是只有机翻或者生肉，而课件和作业肯定都是英文的。不过我觉得这是个值得努力克服的挑战，因为在当下，虽然我很不情愿，但也不得不承认，在计算机领域，很多优质的文档、论坛、网站都是英文居多。养成英文阅读的习惯，在赤旗插遍世界之前，还是有一定好处的（狗头保命）。

第三，也是我觉得最困难的一点，就是自律。因为没有 DDL 有时候真的是一件可怕的事情。特别是随着学习的深入，国外的很多课程是相当虐的。你得有足够的驱动力强迫自己静下心来，阅读几十页的 Project Handout，理解上千行的代码框架，忍受数个小时的 debug 时光。而这一切，没有学分，没有绩点，没有老师，没有同学，只有一个信念 —— 你在变强。

## 这本书适合谁

正如我在前言里说的，任何有志于自学计算机的朋友都可以参考这本书。如果你已经有了一定的计算机基础，只是对某个特定的领域感兴趣，可以选择性地挑选你感兴趣的内容进行学习。当然，如果你是一个像我当年一样对计算机一无所知的小白，初入大学的校门，我希望这本书能成为你的攻略，让你花最少的时间掌握你所需要的知识和能力。某种程度上，这本书更像是一个根据我的体验来排序的课程搜索引擎，帮助大家足不出户，体验世界顶级名校的计算机优质课程。

当然，作为一个还未毕业的本科生，我深感自己没有能力也没有权利去宣扬一种学习方式，我只是希望这份资料能让那些同样有自学之心和毅力朋友可以少走些弯路，收获更丰富、更多样、更满足的学习体验。

## 特别鸣谢

在这里，我怀着崇敬之心真诚地感谢所有将课程资源无偿开源的各位教授们。这些课程倾注了他们数十年教学生涯的积淀和心血，他们却选择无私地让所有人享受到如此高质量的 CS 教育。没有他们，我的大学生活不会这样充实而快乐。很多教授在我给他们发了感谢邮件之后，甚至会回复上百字的长文，真的让我无比感动。他们也时刻激励着我，做一件事，就得用心做好，无论是学习、科研、还是为人。

## 你也想加入到贡献者的行列

一个人的力量终究是有限的，这本书也是我在繁重的科研之余熬夜抽空写出来的，难免有不够完善之处。另外，由于个人做的是系统方向，很多课程侧重系统领域，对于数学、理论计算机、高级算法相关的内容则相对少些。如果有大佬想在其他领域分享自己的自学经历与资源，可以直接在项目中发起 Pull Request，也欢迎和我邮件联系（[zhongyinmin@pku.edu.cn](mailto:zhongyinmin@pku.edu.cn)）。

## 关于交流群的建立

本书支持页面评论功能，因此如果你想自学某课程，可以自己建立群聊后（QQ 微信皆可）在对应的课程页面下方发表评论，注明你的学习目标以及加入交流群的途径。此外，过去已有不少朋友在 issue 里建立了类似群聊，可以自行选择直接加入。

## 请作者喝杯下午茶

本书的内容是完全开源免费的，如果你觉得该项目对你真的有帮助，可以给仓库点个 star 或者请作者喝一杯下午茶。

![Image title](https://cdn.jsdelivr.net/gh/Halerfermatqing/images_bed@main/typora/202406031533764.png)

May 21, 2024

# 如何使用这本书

随着贡献者的不断增多，本书的内容也不断扩展，想把书中所有的课程全部学完是不切实际也没有必要的，甚至会起到事倍功半的反效果，吃力而不讨好。为了更好地贴合读者，让这本书真正为你所用，我将读者按照需求大致分为了如下三类，大家可以结合切身实际，精准地规划属于自己的自学方案。

## 初入校园

如果你刚刚进入大学校园或者还在低年级，并且就读的是计算机方向或者想要转到计算机方向，那么你很幸运，因为学习是你的本业，你可以有充足的时间和自由来学习自己感兴趣的东西，不会有工作的压力和生活的琐碎，不必过于纠结“学了有没有用”，“能不能找到工作”这类功利的想法。那么该如何安排自己的学业呢？我觉得首要的一点就是要打破在高中形成的“按部就班”式的被动学习。作为一个小镇做题家，我深知国内大部分高中会把大家一天当中的每一分钟都安排得满满当当，你只需要被动地跟着课表按部就班地完成一个个既定的任务。只要足够认真，结果都不会太差。但步入大学的校门，自由度一下子变大了许多。首先所有的课外时间基本都由你自由支配，没有人为你整理知识点，总结提纲，考试也不像高中那般模式化。如果你还抱着高中那种“乖学生”的心态，老老实实按部就班，结果未必如你所愿。因为专业培养方案未必就是合理，老师的教学未必就会负责，认真出席课堂未必就能听懂，甚至考试内容未必就和讲的有关系。说句玩笑话，你或许会觉得全世界都与你为敌，而你只能指望自己。

那么现状就是这么个现状，你想改变，也得先活过去，并且拥有足够的能力去质疑它。而在低年级，打好基础很重要。这里的基础是全方面的，课内的知识固然重要，但计算机很大程度上还是强调实践，因此有很多课本外的能力需要培养，而这恰恰是国内的计算机本科教育很欠缺的一点。我根据个人的体验总结出了下面几点建议，供大家参考。

其一就是了解如何写“优雅”的代码。国内的很多大一编程入门课都会讲成极其无聊的语法课，其效果还不如直接让学生看官方文档。事实上，在刚开始接触编程的时候，让学生试着去了解什么样的代码是优雅的，什么样的代码 "have bad taste" 是大有裨益的。一般来说，编程入门课会先介绍过程式编程（例如 C 语言）。但即便是面向过程编程，**模块化** 和 **封装** 的思想也极其重要。如果你只想着代码能在 OpenJudge 上通过，写的时候图省事，用大段的复制粘贴和臃肿的 main 函数，长此以往，你的代码质量将一直如此。一旦接触稍微大一点的项目，无尽的 debug 和沟通维护成本将把你吞没。因此，写代码时不断问自己，是否有大量重复的代码？当前函数是否过于复杂（Linux 提倡每个函数只需要做好一件事）？这段代码能抽象成一个函数吗？一开始你可能觉得很不习惯，甚至觉得这么简单的题需要如此大费周章吗？但记住好的习惯是无价的，C 语言初中生都能学会，凭什么公司要招你去当程序员呢？

学过面向过程编程后，大一下学期一般会讲面向对象编程（例如 C++ 或 Java）。这里非常推荐大家看 [MIT 6.031: Software Construction](https://csdiy.wiki/软件工程/6031/) 这门课的 Notes，会以 Java 语言（22年改用了 TypeScript 语言）为例非常详细地讲解如何写出“优雅”的代码。例如 Test-Driven 的开发、函数 Specification 的设计、异常的处理等等等等。除此之外，既然接触了面向对象，那么了解一些常见的设计模式也是很有必要的。因为国内的面向对象课程同样很容易变成极其无聊的语法课，让学生纠结于各种继承的语法，甚至出一些无聊的脑筋急转弯一样的题目，殊不知这些东西在地球人的开发中基本不会用到。面向对象的精髓是让学生学会自己将实际的问题抽象成若干类和它们之间的关系，而设计模式则是前人总结出来的一些精髓的抽象方法。这里推荐[大话设计模式](https://book.douban.com/subject/2334288/) 这本书，写得非常浅显易懂。

其二就是尝试学习一些能提高生产力的工具和技能，例如 Git、Shell、Vim。这里强烈推荐学习 [MIT missing semester](https://csdiy.wiki/编程入门/MIT-Missing-Semester/) 这门课，也许一开始接触这些工具用起来会很不习惯，但强迫自己用，熟练之后开发效率会直线提高。此外，还有很多应用也能极大提高的你生产力。一条定律是：一切需要让手离开键盘的操作，都应该想办法去除。例如切换应用、打开文件、浏览网页这些都有相关插件可以实现快捷操作（例如 Mac 上的 [Alfred](https://www.alfredapp.com/)）。如果你发现某个操作每天都会用到，并且用时超过1秒，那就应该想办法把它缩减到0.1秒。毕竟以后数十年你都要和电脑打交道，形成一套顺滑的工作流是事半功倍的。最后，学会盲打！如果你还需要看着键盘打字，那么赶紧上网找个教程学会盲打，这将极大提高你的开发效率。

其三就是平衡好课内和自学。我们质疑现状，但也得遵守规则，毕竟绩点在保研中还是相当重要的。因此在大一，我还是建议大家尽量按照自己的课表学习，但辅以一些优质的课外资源。例如微积分线代可以参考 [MIT 18.01/18.02](https://csdiy.wiki/数学基础/MITmaths/) 和 [MIT 18.06](https://csdiy.wiki/数学基础/MITLA/) 的课程 Notes。假期可以通过 [UCB CS61A](https://csdiy.wiki/编程入门/Python/CS61A/) 来学习 Python。同时做到上面第一、第二点说的，注重好的编程习惯和实践能力的培养。就个人经验，大一的数学课学分占比相当大，而且数学考试的内容方差是很大的，不同学校不同老师风格迥异，自学也许能让你领悟数学的本质，但未必能给你一个好成绩。因此考前最好有针对性地刷往年题，充分应试。

在升入大二之后，计算机方向的专业课将居多，此时大家可以彻底放飞自我，进入自学的殿堂了。具体可以参考 [一份仅供参考的CS学习规划](https://csdiy.wiki/CS学习规划/)，这是我根据自己三年自学经历总结提炼出来的全套指南，每门课的特点以及为什么要上这门课我都做了简单的介绍。对于你课表上的每个课程，这份规划里应该都会有相应的国外课程，而且在质量上我相信基本是全方位的碾压。由于计算机方向的专业知识基本是一样的，而且高质量的课程会让你从原理上理解知识点，对于国内大多照本宣科式的教学来说基本是降维打击。一般来说只要考前将老师“辛苦”念了一学期的 PPT 拿来突击复习两天，取得一个不错的卷面分数并不困难。如果有课程大作业，则可以尽量将国外课程的 Lab 或者 Project 修改一番以应付课内的需要。我当时上操作系统课，发现老师还用着早已被国外学校淘汰的课程实验，便邮件老师换成了自己正在学习的 [MIT 6.S081](https://csdiy.wiki/操作系统/MIT6.S081/) 的 xv6 Project，方便自学的同时还无意间推动了课程改革。总之，灵活变通是第一要义，你的目标是用最方便、效率最高的方式掌握知识，所有与你这一目标违背的所谓规定都可以想方设法地去“糊弄”。凭着这份糊弄劲儿，我大三之后基本没有去过线下课堂（大二疫情在家呆了大半年），对绩点也完全没有影响。

最后，希望大家少点浮躁和功利，多一些耐心和追求。很多人发邮件问我自学需不需要很强的自制力，我觉得得关键得看你自己想要什么。如果你依然抱着会一门编程语言便能月薪过万的幻想，想分一杯互联网的红利，那么我说再多也是废话。其实我最初的自学并没有太多功利的想法，只是单纯的好奇和本能的求知欲。自学的过程也没有所谓的“头悬梁，锥刺股”，该吃吃，该玩玩，不知不觉才发现竟然攒下了这么多资料。现如今中美的对抗已然成为趋势，而我们还在“卑微”地“师夷长技”，感叹国外高质量课程的同时也时常会有一种危机感。这一切靠谁来改变呢？靠的是刚刚入行的你们。所以，加油吧，少年！

## 删繁就简

如果你已经本科毕业开始读研或者走上了工作岗位，亦或是从事着其他领域的工作想要利用业余时间转码，那么你也许并没有充足的业余时间来系统地学完 [一份仅供参考的CS学习规划](https://csdiy.wiki/CS学习规划/) 里的内容，但又想弥补本科时期欠下的基础。考虑到这部分读者通常有一定的编程经验，入门课程没有必要再重复学习。而且从实用角度来说，由于工作的大体方向已经确定，确实没有太大必要对于每个计算机分支都有特别深入的研究，更应该侧重一些通用性的原则和技能。因此我结合自身经历，选取了个人感觉最重要也是质量最高的几门核心专业课，希望能更好地加深读者对计算机的理解。学完这些课程，无论你具体从事的是什么工作，我相信你将不可能沦为一个普通的调包侠，而是对计算机的底层运行逻辑有更深入的了解。

| 课程方向         | 课程名                                                                            |
| :--------------- | :-------------------------------------------------------------------------------- |
| 离散数学和概率论 | [UCB CS70 : discrete Math and probability theory](https://csdiy.wiki/数学进阶/CS70/) |
| 数据结构与算法   | [Coursera: Algorithms I &amp; II](https://csdiy.wiki/数据结构与算法/Algo/)           |
| 软件工程         | [MIT 6.031: Software Construction](https://csdiy.wiki/软件工程/6031/)                |
| 全栈开发         | [MIT web development course](https://csdiy.wiki/Web开发/mitweb/)                     |
| 计算机系统导论   | [CMU CS15213: CSAPP](https://csdiy.wiki/计算机系统基础/CSAPP/)                       |
| 体系结构入门     | [Coursera: Nand2Tetris](https://csdiy.wiki/体系结构/N2T/)                            |
| 体系结构进阶     | [CS61C: Great Ideas in Computer Architecture](https://csdiy.wiki/体系结构/CS61C/)    |
| 数据库原理       | [CMU 15-445: Introduction to Database System](https://csdiy.wiki/数据库系统/15445/)  |
| 计算机网络       | [Computer Networking: A Top-Down Approach](https://csdiy.wiki/计算机网络/topdown/)   |
| 人工智能         | [Harvard CS50: Introduction to AI with Python](https://csdiy.wiki/人工智能/CS50/)    |
| 深度学习         | [Coursera: Deep Learning](https://csdiy.wiki/深度学习/CS230/)                        |

## 心有所属

如果你对于计算机领域的核心专业课都掌握得相当扎实，而且已经确定了自己的工作或研究方向，那么书中还有很多未在 [一份仅供参考的CS学习规划](https://csdiy.wiki/CS学习规划/) 提到的课程供你探索。

随着贡献者的不断增多，左侧的目录中将不断增加新的分支，例如 **机器学习进阶** 和 **机器学习系统**。并且同一个分支下都有若干同类型课程，它们来自不同的学校，有着不同的侧重点和课程实验，例如 **操作系统** 分支下就包含了麻省理工、伯克利、南京大学还有哈工大四所学校的课程。如果你想深耕一个领域，那么学习这些同类的课程会给你不同的视角来看待类似的知识。同时，本书作者还计划联系一些相关领域的科研工作者来分享某个细分领域的科研学习路径，让 CS自学指南 在追求广度的同时，实现深度上的提高。

如果你想贡献这方面的内容，欢迎和作者邮件联系 [zhongyinmin@pku.edu.cn](mailto:zhongyinmin@pku.edu.cn)

May 21, 2024

# 一个仅供参考的 CS 学习规划

计算机领域方向庞杂，知识浩如烟海，每个细分领域如果深究下去都可以说学无止境。因此，一个清晰明确的学习规划是非常重要的。我在多年自学的尝试中也走过不少弯路，最终提炼出了下面的内容，供大家参考。

不过，在开始学习之前，先向小白们强烈推荐一个科普向系列视频 [Crash Course: Computer Science](https://www.bilibili.com/video/BV1EW411u7th)，在短短 8 个小时里非常生动且全面地科普了关于计算机科学的方方面面：计算机的历史、计算机是如何运作的、组成计算机的各个重要模块、计算机科学中的重要思想等等等等。正如它的口号所说的 *Computers are not magic!*，希望看完这个视频之后，大家能对计算机科学有个全貌性地感知，从而怀着兴趣去面对下面浩如烟海的更为细致且深入的学习内容。

## 必学工具

> 俗话说：磨刀不误砍柴工。如果你是一个刚刚接触计算机的24k纯小白，学会一些工具将会让你事半功倍。

学会提问：也许你会惊讶，提问也算计算机必备技能吗，还放在第一条？我觉得在开源社区中，学会提问是一项非常重要的能力，它包含两方面的事情。其一是会变相地培养你自主解决问题的能力，因为从形成问题、描述问题并发布、他人回答、最后再到理解回答这个周期是非常长的，如果遇到什么鸡毛蒜皮的事情都希望别人最好远程桌面手把手帮你完成，那计算机的世界基本与你无缘了。其二，如果真的经过尝试还无法解决，可以借助开源社区的帮助，但这时候如何通过简洁的文字让别人瞬间理解你的处境以及目的，就显得尤为重要。推荐阅读[提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/main/README-zh_CN.md)这篇文章，这不仅能提高你解决问题的概率和效率，也能让开源社区里无偿提供解答的人们拥有一个好心情。

[MIT-Missing-Semester](https://csdiy.wiki/编程入门/MIT-Missing-Semester/) 这门课覆盖了这些工具中绝大部分，而且有相当详细的使用指导，强烈建议小白学习。不过需要注意的一点是，在课程中会不时提到一些与开发流程相关的术语。因此推荐至少在学完计算机导论级别的课程之后进行学习。

[翻墙](https://csdiy.wiki/必学工具/翻墙/)：由于一些众所周知的原因，谷歌、GitHub 等网站在大陆无法访问。然而很多时候，谷歌和 StackOverflow 可以解决你在开发过程中遇到的 99% 的问题。因此，学会翻墙几乎是一个内地 CSer 的必备技能。（考虑到法律问题，这个文档提供的翻墙方式仅对拥有北大邮箱的用户适用）。

命令行：熟练使用命令行是一种常常被忽视，或被认为难以掌握的技能，但实际上，它会极大地提高你作为工程师的灵活性以及生产力。[命令行的艺术](https://github.com/jlevy/the-art-of-command-line/blob/master/README-zh.md)是一份非常经典的教程，它源于 Quora 的一个提问，但在各路大神的贡献努力下已经成为了一个 GitHub 十万 stars 的顶流项目，被翻译成了十几种语言。教程不长，非常建议大家反复通读，在实践中内化吸收。同时，掌握 Shell 脚本编程也是一项不容忽视的技术，可以参考这个[教程](https://www.shellscript.sh/)。

IDE (Integrated Development Environment)：集成开发环境，说白了就是你写代码的地方。作为一个码农，IDE 的重要性不言而喻，但由于很多 IDE 是为大型工程项目设计的，体量较大，功能也过于丰富。其实如今一些轻便的文本编辑器配合丰富的插件生态基本可以满足日常的轻量编程需求。个人常用的编辑器是 VS Code 和 Sublime（前者的插件配置非常简单，后者略显复杂但颜值很高）。当然对于大型项目我还是会采用略重型的 IDE，例如 Pycharm (Python)，IDEA (Java) 等等（免责申明：所有的 IDE 都是世界上最好的 IDE）。

[Vim](https://csdiy.wiki/必学工具/Vim/)：一款命令行编辑工具。这是一个学习曲线有些陡峭的编辑器，不过学会它我觉得是非常有必要的，因为它将极大地提高你的开发效率。现在绝大多数 IDE 也都支持 Vim 插件，让你在享受现代开发环境的同时保留极客的炫酷（yue）。

[Emacs](https://csdiy.wiki/必学工具/Emacs/)：与 Vim 齐名的经典编辑器，同样具有极高的开发效率，同时具有更为强大的扩展性，它既可以配置为一个轻量编辑器，也可以扩展成一个个人定制的 IDE，甚至可以有更多奇技淫巧。

[Git](https://csdiy.wiki/必学工具/Git/)：一款代码版本控制工具。Git的学习曲线可能更为陡峭，但出自 Linux 之父 Linus 之手的 Git 绝对是每个学 CS 的童鞋必须掌握的神器之一。

[GitHub](https://csdiy.wiki/必学工具/GitHub/)：基于 Git 的代码托管平台。全世界最大的代码开源社区，大佬集聚地。

[GNU Make](https://csdiy.wiki/必学工具/GNU_Make/)：一款工程构建工具。善用 GNU Make 会让你养成代码模块化的习惯，同时也能让你熟悉一些大型工程的编译链接流程。

[CMake](https://csdiy.wiki/必学工具/CMake/)：一款功能比 GNU Make 更为强大的构建工具，建议掌握 GNU Make 之后再加以学习。

[LaTex](https://csdiy.wiki/必学工具/LaTeX/)：~~逼格提升~~ 论文排版工具。

[Docker](https://csdiy.wiki/必学工具/Docker/)：一款相较于虚拟机更轻量级的软件打包与环境部署工具。

[实用工具箱](https://csdiy.wiki/必学工具/tools/)：除了上面提到的这些在开发中使用频率极高的工具之外，我还收集了很多实用有趣的免费工具，例如一些下载工具、设计工具、学习网站等等。

[Thesis](https://csdiy.wiki/必学工具/thesis/)：毕业论文 Word 写作教程。

## 好书推荐

> 私以为一本好的教材应当是以人为本的，而不是炫技式的理论堆砌。告诉读者“是什么”固然重要，但更好的应当是教材作者将其在这个领域深耕几十年的经验融汇进书中，向读者娓娓道来“为什么”以及未来应该“怎么做”。

[链接戳这里](https://csdiy.wiki/好书推荐/)

## 环境配置

> 你以为的开发 —— 在 IDE 里疯狂码代码数小时。
>
> 实际上的开发 —— 配环境配几天还没开始写代码。

### PC 端环境配置

如果你是 Mac 用户，那么你很幸运，这份[指南](https://sourabhbajaj.com/mac-setup/) 将会手把手地带你搭建起整套开发环境。如果你是 Windows 用户，在开源社区的努力下，你同样可以获得与其他平台类似的体验：[Scoop](https://csdiy.wiki/必学工具/Scoop/)。

另外大家可以参考一份灵感来自 [6.NULL MIT-Missing-Semester](https://csdiy.wiki/编程入门/MIT-Missing-Semester/) 的 [环境配置指南](https://taylover2016.github.io/新机器上手指南（新手向）/index.html)，重点在于终端的美化配置。此外还包括常用软件源（如 GitHub, Anaconda, PyPI 等）的加速与替换以及一些 IDE 的配置与激活教程。

### 服务器端环境配置

服务器端的运维需要掌握 Linux（或者其他类 Unix 系统）的基本使用以及进程、设备、网络等系统相关的基本概念，小白可以参考中国科学技术大学 Linux 用户协会编写的[《Linux 101》在线讲义](https://101.lug.ustc.edu.cn/)。如果想深入学习系统运维相关的知识，可以参考 [Aspects of System Administration](https://stevens.netmeister.org/615/) 这门课程。

另外，如果需要学习某个具体的概念或工具，推荐一个非常不错的 GitHub 项目 [DevOps-Guide](https://github.com/Tikam02/DevOps-Guide)，其中涵盖了非常多的运维方面的基础知识和教程，例如 Docker, Kubernetes, Linux, CI-CD, GitHub Actions 等等。

## 课程地图

> 正如这章开头提到的，这份课程地图仅仅是一个**仅供参考**的课程规划，我作为一个临近毕业的本科生。深感自己没有权利也没有能力向别人宣扬“应该怎么学”。因此如果你觉得以下的课程分类与选择有不合理之处，我全盘接受，并深感抱歉。你可以在下一节[定制属于你的课程地图](https://csdiy.wiki/CS学习规划/#yourmap)

以下课程类别中除了含有 *基础* 和 *入门* 字眼的以外，并无明确的先后次序，大家只要满足某个课程的先修要求，完全可以根据自己的需要和喜好选择想要学习的课程。

### 数学基础

#### 微积分与线性代数

作为大一新生，学好微积分线代是和写代码至少同等重要的事情，相信已经有无数的前人经验提到过这一点，但我还是要不厌其烦地再强调一遍：学好微积分线代真的很重要！你也许会吐槽这些东西岂不是考完就忘，那我觉得你是并没有把握住它们本质，对它们的理解还没有达到刻骨铭心的程度。如果觉得老师课上讲的内容晦涩难懂，不妨参考 MIT 的 [Calculus Course](https://csdiy.wiki/数学基础/MITmaths/) 和 [18.06: Linear Algebra](https://csdiy.wiki/数学基础/MITLA/) 的课程 notes，至少于我而言，它帮助我深刻理解了微积分和线性代数的许多本质。顺道再安利一个油管数学网红 [**3Blue1Brown**](https://www.youtube.com/c/3blue1brown)，他的频道有很多用生动形象的动画阐释数学本质内核的视频，兼具深度和广度，质量非常高。

#### 信息论入门

作为计算机系的学生，及早了解一些信息论的基础知识，我觉得是大有裨益的。但大多信息论课程都面向高年级本科生甚至研究生，对新手极不友好。而 MIT 的 [6.050J: Information theory and Entropy](https://csdiy.wiki/数学基础/information/) 这门课正是为大一新生量身定制的，几乎没有先修要求，涵盖了编码、压缩、通信、信息熵等等内容，非常有趣。

### 数学进阶

#### 离散数学与概率论

集合论、图论、概率论等等是算法推导与证明的重要工具，也是后续高阶数学课程的基础。但我觉得这类课程的讲授很容易落入理论化与形式化的窠臼，让课堂成为定理结论的堆砌，而无法使学生深刻把握理论的本质，进而造成学了就背，考了就忘的怪圈。如果能在理论教学中穿插算法运用实例，学生在拓展算法知识的同时也能窥见理论的力量和魅力。

[UCB CS70 : discrete Math and probability theory](https://csdiy.wiki/数学进阶/CS70/) 和 [UCB CS126 : Probability theory](https://csdiy.wiki/数学进阶/CS126/) 是 UC Berkeley 的概率论课程，前者覆盖了离散数学和概率论基础，后者则涉及随机过程以及深入的理论内容。两者都非常注重理论和实践的结合，有丰富的算法实际运用实例，后者还有大量的 Python 编程作业来让学生运用概率论的知识解决实际问题。

#### 数值分析

作为计算机系的学生，培养计算思维是很重要的，实际问题的建模、离散化，计算机的模拟、分析，是一项很重要的能力。而这两年开始风靡的，由 MIT 打造的 [Julia](https://julialang.org/) 编程语言以其 C 一样的速度和 Python 一样友好的语法在数值计算领域有一统天下之势，MIT 的许多数学课程也开始用 Julia 作为教学工具，把艰深的数学理论用直观清晰的代码展示出来。

[ComputationalThinking](https://computationalthinking.mit.edu/Spring21/) 是 MIT 开设的一门计算思维入门课，所有课程内容全部开源，可以在课程网站直接访问。这门课利用 Julia 编程语言，在图像处理、社会科学与数据科学、气候学建模三个 topic 下带领学生理解算法、数学建模、数据分析、交互设计、图例展示，让学生体验计算与科学的美妙结合。内容虽然不难，但给我最深刻的感受就是，科学的魅力并不是故弄玄虚的艰深理论，不是诘屈聱牙的术语行话，而是用直观生动的案例，用简练深刻的语言，让每个普通人都能理解。

上完上面的体验课之后，如果意犹未尽的话，不妨试试 MIT 的 [18.330 : Introduction to numerical analysis](https://csdiy.wiki/数学进阶/numerical/)，这门课的编程作业同样会用 Julia 编程语言，不过难度和深度上都上了一个台阶。内容涉及了浮点编码、Root finding、线性系统、微分方程等等方面，整门课的主旨就是让你利用离散化的计算机表示去估计和逼近一个数学上连续的概念。这门课的教授还专门撰写了一本配套的开源教材 [Fundamentals of Numerical Computation](https://fncbook.github.io/fnc/frontmatter.html)，里面附有丰富的 Julia 代码实例和严谨的公式推导。

如果你还意犹未尽的话，还有 MIT 的数值分析研究生课程 [18.335: Introduction to numerical method](https://ocw.mit.edu/courses/mathematics/18-335j-introduction-to-numerical-methods-spring-2019/index.htm) 供你参考。

#### 微分方程

如果世间万物的运动发展都能用方程来刻画和描述，这是一件多么酷的事情呀！虽然几乎任何一所学校的 CS 培养方案中都没有微分方程相关的必修课程，但我还是觉得掌握它会赋予你一个新的视角来审视这个世界。

由于微分方程中往往会用到很多复变函数的知识，所以大家可以参考 [MIT18.04: Complex variables functions](https://ocw.mit.edu/courses/mathematics/18-04-complex-variables-with-applications-spring-2018/) 的课程 notes 来补齐先修知识。

[MIT18.03: differential equations](https://ocw.mit.edu/courses/mathematics/18-03sc-differential-equations-fall-2011/unit-i-first-order-differential-equations/) 主要覆盖了常微分方程的求解，在此基础之上 [MIT18.152: Partial differential equations](https://ocw.mit.edu/courses/mathematics/18-152-introduction-to-partial-differential-equations-fall-2011/index.htm) 则会深入偏微分方程的建模与求解。掌握了微分方程这一有力工具，相信对于你的实际问题的建模能力以及从众多噪声变量中把握本质的直觉都会有很大帮助。

### 数学高阶

作为计算机系的学生，我经常听到数学无用论的论断，对此我不敢苟同但也无权反对，但若凡事都硬要争出个有用和无用的区别来，倒也着实无趣，因此下面这些面向高年级甚至研究生的数学课程，大家按兴趣自取所需。

#### 凸优化

[Standford EE364A: Convex Optimization](https://csdiy.wiki/数学进阶/convex/)

#### 信息论

[MIT6.441: Information Theory](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-441-information-theory-spring-2016/syllabus/)

#### 应用统计学

[MIT18.650: Statistics for Applications](https://ocw.mit.edu/courses/mathematics/18-443-statistics-for-applications-spring-2015/index.htm)

#### 初等数论

[MIT18.781: Theory of Numbers](https://ocw.mit.edu/courses/mathematics/18-781-theory-of-numbers-spring-2012/index.htm)

#### 密码学

[Standford CS255: Cryptography](http://crypto.stanford.edu/~dabo/cs255/)

### 编程入门

> Languages are tools, you choose the right tool to do the right thing. Since there's no universally perfect tool, there's no universally perfect language.

#### General

- [MIT-Missing-Semester](https://csdiy.wiki/编程入门/MIT-Missing-Semester/)
- [Harvard CS50: This is CS50x](https://csdiy.wiki/编程入门/C/CS50/)

#### Java

- [MIT 6.092: Introduction To Programming In Java](https://csdiy.wiki/编程入门/Java/MIT 6.092/)

#### Python

- [CS50P: CS50&#39;s Introduction to Programming with Python](https://csdiy.wiki/编程入门/Python/CS50P/)
- [UCB CS61A: Structure and Interpretation of Computer Programs](https://csdiy.wiki/编程入门/Python/CS61A/)

#### C++

- [Stanford CS106B/X: Programming Abstractions](https://csdiy.wiki/编程入门/cpp/CS106B_CS106X/)
- [Stanford CS106L: Standard C++ Programming](https://csdiy.wiki/编程入门/cpp/CS106L/)

#### Rust

- [Stanford CS110L: Safety in Systems Programming](https://csdiy.wiki/编程入门/Rust/CS110L/)

#### OCaml

- [Cornell CS3110: OCaml Programming Correct + Efficient + Beautiful](https://csdiy.wiki/编程入门/Functional/CS3110/)

### 电子基础

#### 电路基础

作为计算机系的学生，了解一些基础的电路知识，感受从传感器收集数据到数据分析再到算法预测整条流水线，对于后续知识的学习以及计算思维的培养还是很有帮助的。[EE16A&amp;B: Designing Information Devices and Systems I&amp;II](https://csdiy.wiki/电子基础/EE16/) 是伯克利 EE 学生的大一入门课，其中 EE16A 注重通过电路从实际环境中收集和分析数据，而 EE16B 则侧重从这些收集到的数据进行分析并做出预测行为。

#### 信号与系统

信号与系统是一门我觉得非常值得一上的课，最初学它只是为了满足我对傅里叶变换的好奇，但学完之后我才不禁感叹，傅立叶变换给我提供了一个全新的视角去看待这个世界，就如同微分方程一样，让你沉浸在用数学去精确描绘和刻画这个世界的优雅与神奇之中。

[MIT 6.003: signal and systems](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-003-signals-and-systems-fall-2011/lecture-videos/lecture-1-signals-and-systems/) 提供了全部的课程录影、书面作业以及答案。也可以去看这门课的[远古版本](https://csdiy.wiki/电子基础/Signals_and_Systems_AVO/)

而 [UCB EE120: Signal and Systems](https://csdiy.wiki/电子基础/signal/) 关于傅立叶变换的 notes 写得非常好，并且提供了6 个非常有趣的 Python 编程作业，让你实践中运用信号与系统的理论与算法。

### 数据结构与算法

算法是计算机科学的核心，也是几乎一切专业课程的基础。如何将实际问题通过数学抽象转化为算法问题，并选用合适的数据结构在时间和内存大小的限制下将其解决是算法课的永恒主题。如果你受够了老师的照本宣科，那么我强烈推荐伯克利的 [UCB CS61B: Data Structures and Algorithms](https://csdiy.wiki/数据结构与算法/CS61B/) 和普林斯顿的 [Coursera: Algorithms I &amp; II](https://csdiy.wiki/数据结构与算法/Algo/)，这两门课的都讲得深入浅出并且会有丰富且有趣的编程实验将理论与知识结合起来。

以上两门课程都是基于 Java 语言，如果你想学习 C/C++ 描述的版本，可以参考斯坦福的数据结构与基础算法课程 [Stanford CS106B/X: Programming Abstractions](https://csdiy.wiki/编程入门/cpp/CS106B_CS106X/)。偏好 Python 的同学可以学习 MIT 的算法入门课 [MIT 6.006: Introduction to Algorithms](https://csdiy.wiki/数据结构与算法/6.006/)

对一些更高级的算法以及 NP 问题感兴趣的同学可以学习伯克利的算法设计与分析课程 [UCB CS170: Efficient Algorithms and Intractable Problems](https://csdiy.wiki/数据结构与算法/CS170/) 或者 MIT 的高阶算法 [MIT 6.046: Design and Analysis of Algorithms](https://csdiy.wiki/数据结构与算法/6.046/)。

### 软件工程

#### 入门课

一份“能跑”的代码，和一份高质量的工业级代码是有本质区别的。因此我非常推荐低年级的同学学习一下 [MIT 6.031: Software Construction](https://csdiy.wiki/软件工程/6031/) 这门课，它会以 Java 语言为基础，以丰富细致的阅读材料和精心设计的编程练习传授如何编写**不易出 bug、简明易懂、易于维护修改**的高质量代码。大到宏观数据结构设计，小到如何写注释，遵循这些前人总结的细节和经验，对于你此后的编程生涯大有裨益。

#### 专业课

当然，如果你想系统性地上一门软件工程的课程，那我推荐的是伯克利的 [UCB CS169: software engineering](https://csdiy.wiki/软件工程/CS169/)。但需要提醒的是，和大多学校（包括贵校）的软件工程课程不同，这门课不会涉及传统的 **design and document** 模式，即强调各种类图、流程图及文档设计，而是采用近些年流行起来的小团队快速迭代 **Agile Develepment** 开发模式以及利用云平台的 **Software as a service** 服务模式。

### 体系结构

#### 入门课

从小我就一直听说，计算机的世界是由 01 构成的，我不理解但大受震撼。如果你的内心也怀有这份好奇，不妨花一到两个月的时间学习 [Coursera: Nand2Tetris](https://csdiy.wiki/体系结构/N2T/) 这门无门槛的计算机课程。这门麻雀虽小五脏俱全的课程会从 01 开始让你亲手造出一台计算机，并在上面运行俄罗斯方块小游戏。一门课里涵盖了编译、虚拟机、汇编、体系结构、数字电路、逻辑门等等从上至下、从软至硬的各类知识，非常全面。难度上也是通过精心的设计，略去了众多现代计算机复杂的细节，提取出了最核心本质的东西，力图让每个人都能理解。在低年级，如果就能从宏观上建立对整个计算机体系的鸟瞰图，是大有裨益的。

#### 专业课

当然，如果想深入现代计算机体系结构的复杂细节，还得上一门大学本科难度的课程 [UCB CS61C: Great Ideas in Computer Architecture](https://csdiy.wiki/体系结构/CS61C/)。UC Berkeley 作为 RISC-V 架构的发源地，在体系结构领域算得上首屈一指。其课程非常注重实践，你会在 Project 中手写汇编构造神经网络，从零开始搭建一个 CPU，这些实践都会让你对计算机体系结构有更为深入的理解，而不是仅停留于“取指译码执行访存写回”的单调背诵里。

### 系统入门

计算机系统是一个庞杂而深刻的主题，在深入学习某个细分领域之前，对各个领域有一个宏观概念性的理解，对一些通用性的设计原则有所知晓，会让你在之后的深入学习中不断强化一些最为核心乃至哲学的概念，而不会桎梏于复杂的内部细节和各种 trick。因为在我看来，学习系统最关键的还是想让你领悟到这些最核心的东西，从而能够设计和实现出属于自己的系统。

[MIT6.033: System Engineering](http://web.mit.edu/6.033/www/) 是 MIT 的系统入门课，主题涉及了操作系统、网络、分布式和系统安全，除了知识点的传授外，这门课还会讲授一些写作和表达上的技巧，让你学会如何设计并向别人介绍和分析自己的系统。这本书配套的教材 *Principles of Computer System Design: An Introduction* 也写得非常好，推荐大家阅读。

[CMU 15-213: Introduction to Computer System](https://csdiy.wiki/计算机系统基础/CSAPP/) 是 CMU 的系统入门课，内容覆盖了体系结构、操作系统、链接、并行、网络等等，兼具广度和深度，配套的教材 *Computer Systems: A Programmer's Perspective* 也是质量极高，强烈建议阅读。

### 操作系统

> 没有什么能比自己写个内核更能加深对操作系统的理解了。

操作系统作为各类纷繁复杂的底层硬件虚拟化出一套规范优雅的抽象，给所有应用软件提供丰富的功能支持。了解操作系统的设计原则和内部原理对于一个不满足于当调包侠的程序员来说是大有裨益的。出于对操作系统的热爱，我上过国内外很多操作系统课程，它们各有侧重和优劣，大家可以根据兴趣各取所需。

[MIT 6.S081: Operating System Engineering](https://csdiy.wiki/操作系统/MIT6.S081/)，MIT 著名 PDOS 实验室出品，11 个 Project 让你在一个实现非常优雅的类Unix操作系统xv6上增加各类功能模块。这门课也让我深刻认识到，做系统不是靠 PPT 念出来的，是得几万行代码一点点累起来的。

[UCB CS162: Operating System](https://csdiy.wiki/操作系统/CS162/)，伯克利的操作系统课，采用和 Stanford 同样的 Project —— 一个教学用操作系统 Pintos。我作为北京大学2022年和2023年春季学期操作系统实验班的助教，引入并改善了这个 Project，课程资源也会全部开源，具体参见[课程网站](https://pku-os.github.io/)。

[NJU: Operating System Design and Implementation](https://csdiy.wiki/操作系统/NJUOS/)，南京大学的蒋炎岩老师开设的操作系统课程。蒋老师以其独到的系统视角结合丰富的代码示例将众多操作系统的概念讲得深入浅出，此外这门课的全部课程内容都是中文的，非常方便大家学习。

[HIT OS: Operating System](https://csdiy.wiki/操作系统/HITOS/)，哈尔滨工业大学的李治军老师开设的中文操作系统课程。李老师的课程基于 Linux 0.11 源码，十分注重代码实践，并站在学生视角将操作系统的来龙去脉娓娓道来。

### 并行与分布式系统

想必这两年各类 CS 讲座里最常听到的话就是“摩尔定律正在走向终结”，此话不假，当单核能力达到上限时，多核乃至众核架构如日中天。硬件的变化带来的是上层编程逻辑的适应与改变，要想充分利用硬件性能，编写并行程序几乎成了程序员的必备技能。与此同时，深度学习的兴起对计算机算力与存储的要求都达到了前所未有的高度，大规模集群的部署和优化也成为热门技术话题。

#### 并行计算

[CMU 15-418/Stanford CS149: Parallel Computing](https://csdiy.wiki/并行与分布式系统/CS149/)

#### 分布式系统

[MIT 6.824: Distributed System](https://csdiy.wiki/并行与分布式系统/MIT6.824/)

### 系统安全

不知道你当年选择计算机是不是因为怀着一个中二的黑客梦想，但现实却是成为黑客道阻且长。

#### 理论课程

[UCB CS161: Computer Security](https://csdiy.wiki/系统安全/CS161/) 是伯克利的系统安全课程，会涵盖栈攻击、密码学、网站安全、网络安全等等内容。

[ASU CSE365: Introduction to Cybersecurity](https://csdiy.wiki/系统安全/CSE365/) 亚利桑那州立大学的 Web 安全课程，主要涉及注入、汇编与密码学的内容。

[ASU CSE466: Computer Systems Security](https://csdiy.wiki/系统安全/CSE466/) 亚利桑那州立大学的系统安全课程，涉及内容全面。门槛较高，需要对 Linux, C 与 Python 充分熟悉。

[SU SEED Labs](https://csdiy.wiki/系统安全/SEEDLabs/) 雪城大学的网安课程，由 NSF 提供130万美元的资金支持，为网安教育开发了动手实践性的实验练习（称为 SEED Lab）。课程理论教学和动手实践并重，包含详细的开源讲义、视频教程、教科书（被印刷为多种语言）、开箱即用的基于虚拟机和 docker 的攻防环境等。目前全球有1050家研究机构在使用该项目。涵盖计算机和信息安全领域的广泛主题，包括软件安全、网络安全、Web 安全、操作系统安全和移动应用安全。

#### 实践课程

掌握这些理论知识之后，还需要在实践中培养和锻炼这些“黑客素养”。[CTF 夺旗赛](https://ctf-wiki.org/)是一项比较热门的系统安全比赛，赛题中会融会贯通地考察你对计算机各个领域知识的理解和运用。北大今年也成功举办了[第 0 届和第 1 届](https://geekgame.pku.edu.cn/)，鼓励大家后期踊跃参与，在实践中提高自己。下面列举一些我平时学习（摸鱼）用到的资源：

- [CTF-wiki](https://ctf-wiki.org/)
- [CTF-101](https://ctf101.org/)
- [Hacker-101](https://ctf.hacker101.com/)

### 计算机网络

> 没有什么能比自己写个 TCP/IP 协议栈更能加深对计算机网络的理解了。

大名鼎鼎的 [Stanford CS144: Computer Network](https://csdiy.wiki/计算机网络/CS144/)，8 个 Project 带你实现整个 TCP/IP 协议栈。

如果你只是想在理论上对计算机网络有所了解，那么推荐计网著名教材《自顶向下方法》的配套学习资源 [Computer Networking: A Top-Down Approach](https://csdiy.wiki/计算机网络/topdown/)。

### 数据库系统

> 没有什么能比自己写个关系型数据库更能加深对数据库系统的理解了。

CMU 的著名数据库神课 [CMU 15-445: Introduction to Database System](https://csdiy.wiki/数据库系统/15445/) 会通过 4 个 Project 带你为一个用于教学的关系型数据库 [bustub](https://github.com/cmu-db/bustub) 添加各种功能。实验的评测框架也免费开源了，非常适合大家自学。此外课程实验会用到 C++11 的众多新特性，也是一个锻炼 C++ 代码能力的好机会。

Berkeley 作为著名开源数据库 postgres 的发源地也不遑多让，[UCB CS186: Introduction to Database System](https://csdiy.wiki/数据库系统/CS186/) 会让你用 Java 语言实现一个支持 SQL 并发查询、B+ 树索引和故障恢复的关系型数据库。

### 编译原理

> 没有什么能比自己写个编译器更能加深对编译器的理解了。

[Stanford CS143: Compilers](https://csdiy.wiki/编译原理/CS143/) 带你手写编译器。

### Web开发

前后端开发很少在计算机的培养方案里被重视，但其实掌握这项技能还是好处多多的，例如搭建自己的个人主页，抑或是给自己的课程项目做一个精彩的展示网页。

#### 两周速成版

[MIT web development course](https://csdiy.wiki/Web开发/mitweb/)

#### 系统学习版

[Stanford CS142: Web Applications](https://csdiy.wiki/Web开发/CS142/)

### 计算机图形学

- [Stanford CS148](https://csdiy.wiki/计算机图形学/CS148/)
- [Games101](https://csdiy.wiki/计算机图形学/GAMES101/)
- [Games103](https://csdiy.wiki/计算机图形学/GAMES103/)
- [Games202](https://csdiy.wiki/计算机图形学/GAMES202/)

### 数据科学

其实数据科学和机器学习与深度学习有着很紧密的联系，但可能更侧重于实践。Berkeley 的 [UCB Data100: Principles and Techniques of Data Science](https://csdiy.wiki/数据科学/Data100/) 通过丰富的编程练习让你在实践中掌握各类数据分析工具和算法，并带领你体验从海量的数据集中提取出想要的结果，并对未来的数据或用户的行为做出相应的预测。但这只是一门基础课，如果想学习工业级别的数据挖掘与分析技术，可以尝试 Stanford 的大数据挖掘课程 [CS246: Mining Massive Data Sets](https://web.stanford.edu/class/cs246/)。

### 人工智能

近十年人工智能应该算是计算机界最火爆的领域。如果你不满足于整日听各路媒体争相报道人工智能相关的进展，而想真正一探究竟，那么非常推荐学习 Harvard 神课 CS50 系列的人工智能课程 [Harvard CS50: Introduction to AI with Python](https://csdiy.wiki/人工智能/CS50/)。课程短小精悍，覆盖了传统人工智能领域的几大分支，并配有丰富有趣的 Python 编程练习来巩固你对人工智能算法的理解。美中不足的是这门课因为面向在线自学者的缘故内容较为精简，并且不会涉及特别深入的数学理论，如果想要系统深入地学习还需要一门本科生难度的课程，例如 Berkeley 的 [UCB CS188: Introduction to Artificial Intelligence](https://csdiy.wiki/人工智能/CS188/)。这门课的 Project 复刻了经典游戏糖豆人，让你运用人工智能算法玩游戏，非常有趣。

### 机器学习

机器学习领域近些年最重要的进展就是发展出了基于神经网络的深度学习分支，但其实很多基于统计学习的算法依然在数据分析领域有着广泛的应用。如果你之前从未接触过机器学习的相关知识，而且不想一开始就陷入艰深晦涩的数学证明，那么不妨先从 Andrew Ng （吴恩达）的 [Coursera: Machine Learning](https://csdiy.wiki/机器学习/ML/) 学起。这门课在机器学习领域基本无人不晓，吴恩达以其深厚的理论功底和出色的表达能力把很多艰深的算法讲得深入浅出，并且非常实用。其配套的作业也是质量相当上乘，可以帮助你快速入门。

但上过这门课只能让你从宏观上对机器学习这一领域有一定了解，如果想真正理解那些“神奇”算法背后的数学原理甚至从事相关领域的科研工作，那么还需要一门更“数学”的课程，例如 [Stanford CS229: Machine Learning](https://csdiy.wiki/机器学习/CS229/) 或者 [UCB CS189: Introduction to Machine Learning](https://csdiy.wiki/机器学习/CS189/)。

### 深度学习

前几年 AlphaGo 的大热让深度学习进入了大众的视野，不少大学甚至专门成立了相关专业。很多计算机的其他领域也会借助深度学习的技术来做研究，因此基本不管你干啥多少都会接触到一些神经网络、深度学习相关的技术需求。如果想快速入门，同样推荐 Andrew Ng （吴恩达）的 [Coursera: Deep Learning](https://csdiy.wiki/深度学习/CS230/)，质量无需多言，Coursera 上罕见的满分课程。此外如果你觉得英文课程学习起来有难度，推荐李宏毅老师的 [国立台湾大学：机器学习](https://csdiy.wiki/深度学习/LHY/) 课程。这门课打着机器学习的名号，却囊括了深度学习领域的几乎所有方向，非常全面，很适合你从宏观上对这个领域有一个大致的了解。而且老师本人也非常幽默，课堂金句频出。

当然因为深度学习领域发展非常迅速，已经拥有了众多研究分支，如果想要进一步深入，可以按需学习下面罗列的代表课程，

#### 计算机视觉

[UMich EECS 498-007 / 598-005: Deep Learning for Computer Vision](https://csdiy.wiki/深度学习/EECS498-007/)

[Stanford CS231n: CNN for Visual Recognition](https://csdiy.wiki/深度学习/CS231/)

#### 自然语言处理

[Stanford CS224n: Natural Language Processing](https://csdiy.wiki/深度学习/CS224n/)

#### 图神经网络

[Stanford CS224w: Machine Learning with Graphs](https://csdiy.wiki/深度学习/CS224w/)

#### 强化学习

[UCB CS285: Deep Reinforcement Learning](https://csdiy.wiki/深度学习/CS285/)

## 定制属于你的课程地图

> 授人以鱼不如授人以渔。

以上的课程规划难免带有强烈的个人偏好，不一定适合所有人，更多是起到抛砖引玉的作用。如果你想挑选自己感兴趣的方向和内容加以学习，可以参考我在下面列出来的资源。

- [MIT OpenCourseWare](https://ocw.mit.edu/): 麻省理工学院的课程资源开放共享项目，收录了数以千计的各科课程资源，其中计算机类的课号是 6.xxx。
- [MIT CS Course List](http://student.mit.edu/catalog/m6a.html): 麻省理工学院的 CS 课程列表。
- [UC Berkeley EECS Course Map](https://hkn.eecs.berkeley.edu/courseguides): UC Berkeley 的 EECS 培养方案，以课程地图的方式将各门课程的类别和先修关系一目了然地呈现，其中绝大多数课程本书中均有收录。
- [UC Berkeley CS Course List](https://www2.eecs.berkeley.edu/Courses/CS/): UC Berkeley 的 CS 课程列表。
- [Stanford CS Course List](https://blog.csdn.net/qq_41220023/article/details/81976967): 斯坦福的 CS 课程列表。

May 21, 2024

# 必学工具

# Vim

## 为什么学习 Vim

在我看来 Vim 编辑器有如下的好处：

- 让你的整个开发过程手指不需要离开键盘，而且光标的移动不需要方向键使得你的手指一直处在打字的最佳位置。
- 方便的文件切换以及面板控制可以让你同时开发多份文件甚至同一个文件的不同位置。
- Vim 的宏操作可以批量化处理重复操作（例如多行 tab，批量加双引号等等）
- Vim 是很多服务器自带的命令行编辑器，当你通过 `ssh` 连接远程服务器之后，由于没有图形界面，只能在命令行里进行开发（当然现在很多 IDE 如 PyCharm 提供了 `ssh` 插件可以解决这个问题）。
- 异常丰富的插件生态，让你拥有世界上最花里胡哨的命令行编辑器。

## 如何学习 Vim

不幸的是 Vim 的学习曲线确实相当陡峭，我花了好几个星期才慢慢适应了用 Vim 进行开发的过程。最开始你会觉得非常不适应，但一旦熬过了初始阶段，相信我，你会爱上 Vim。

Vim 的学习资料浩如烟海，但掌握它最好的方式还是将它用在日常的开发过程中，而不是一上来就去学各种花里胡哨的高级 Vim 技巧。个人推荐的学习路线如下：

- 先阅读[这篇 tutorial](https://missing.csail.mit.edu/2020/editors/)，掌握基本的 Vim 概念和使用方式，不想看英文的可以阅读[这篇教程](https://github.com/wsdjeg/vim-galore-zh_cn)。
- 用 Vim 自带的 `vimtutor` 进行练习，安装完 Vim 之后直接在命令行里输入 `vimtutor` 即可进入练习程序。
- 最后就是强迫自己使用 Vim 进行开发，IDE 里可以安装 Vim 插件。
- 等你完全适应 Vim 之后新的世界便向你敞开了大门，你可以按需配置自己的 Vim（修改 `.vimrc` 文件），网上有数不胜数的资源可以借鉴。
- 如果你想对配置 Vim 有更加深入的了解，[*Learn Vim Script the Hard Way*](https://learnvimscriptthehardway.stevelosh.com/) 是一个很好的资源。

## 关于键位映射

用 Vim 编辑代码的时候会频繁用到 ESC 和 CTRL 键, 但是这两个键都离 home row 很远, 可以把 CapsLock 键映射到 Esc 或者 Ctrl 键，让手更舒服一些。

Windows 系统可以使用 [Powertoys](https://learn.microsoft.com/en-us/windows/powertoys/) 或者 [AutoHotkey](https://www.autohotkey.com/) 重映射键位。
MacOS 系统提供了重映射键位的[设置](https://vim.fandom.com/wiki/Map_caps_lock_to_escape_in_macOS)，另外也可以使用 [Karabiner-Elements](https://karabiner-elements.pqrs.org/) 重映射。

但更佳的做法是同时将 CapsLock 映射为 Ctrl 和 Esc，点按为 Esc，按住为 Ctrl。这是不同系统下的实现方法：

- [Windows](https://gist.github.com/sedm0784/4443120)
- [MacOS](https://ke-complex-modifications.pqrs.org/#caps_lock_tapped_escape_held_left_control)
- [Linux](https://www.jianshu.com/p/6fdc0e0fb266)

## 推荐参考资料

- Neil, Drew. Practical Vim: Edit Text at the Speed of Thought. N.p., Pragmatic Bookshelf, 2015.
- Neil, Drew. Modern Vim: Craft Your Development Environment with Vim 8 and Neovim. United States, Pragmatic Bookshelf.

May 21, 2024

# Emacs

## 为什么学习 Emacs

Emacs 是一个与 Vim 齐名的强大编辑器，事实上 Emacs 几乎具有 Vim 的所有好处，例如：

- 只需要键盘就可以完成所有操作，大量使用快捷键，具有极高的编辑效率。
- 既可以在终端无图形界面的场景下使用，也可使用有图形界面的版本获得更现代、更美观的体验。

此外，Emacs 与其它大部分编辑器最大的不同就在于其强大的扩展性。Emacs 的内核没有对用户做出任何限制，使用 Emacs Lisp 编程语言可以为 Emacs 编写任意逻辑的插件来扩展 Emacs 的功能。经过几十年的积累，Emacs 的插件生态可谓编辑器中最为丰富和强大的生态之一。有一种说法是，“Emacs 表面上是个编辑器，其实是一个操作系统”。只要稍作学习，你也可以编写属于自己的 Emacs 扩展。

Emacs 对 Vim 用户也十分友好，有一个叫 [evil](https://github.com/emacs-evil/evil) 的插件可以让用户在 Emacs 中使用 Vim 的基本操作，只需要很低的迁移成本即可从 Vim 转到 Emacs。曾经有统计显示有相当一部分用户会从 Vim 转到 Emacs，但几乎没有用户从 Emacs 转到 Vim。事实上，Emacs 相对 Vim 最大的不足是纯文本编辑方面不如 Vim 的多模态编辑效率高，但凭借其强大的扩展性，Emacs 可以扬长避短，把 Vim 吸收进来，结合了二者的长处。

## 如何学习 Emacs

与 Vim 相同，Emacs 的学习曲线也比较陡峭，但一旦理解了 Emacs 的使用逻辑，就会爱不释手。然而，网上的 Emacs 资料大多不细致、不够准确，甚至有哗众取宠的嫌疑。

这里给大家推荐一个较新的中文教程[《专业 Emacs 入门》](https://www.zhihu.com/column/c_1440829147212279808)，这篇教程比较系统和全面，且讲述相对比较耐心细致，在讲解 Emacs 基本逻辑的同时也给出了成套的插件推荐，读完后可以获得一个功能完善的、接近 IDE 的 Emacs，因此值得一读。学完教程只是刚刚开始，学会之后要经常使用，在使用中遇到问题勤于搜索和思考，最终才能得心应手。

## 关于键位映射

Emacs 的唯一缺点便是对 Ctrl 键的使用过多，对小手指不是很友好，强烈建议更改 Ctrl 键的键盘映射。更改映射的方式与 [Vim 教程](https://csdiy.wiki/必学工具/Vim/)中的方法相同，这里不做赘述。

May 21, 2024

# Git

## 为什么使用 Git

Git 是一款分布式的代码版本控制工具，Linux 之父 Linus 嫌弃当时主流的中心式的版本控制工具太难用还要花钱，就自己开发出了 Git 用来维护 Linux 的版本（给大佬跪了）。

Git 的设计非常优雅，但初学者通常因为很难理解其内部逻辑因此会觉得非常难用。对 Git 不熟悉的初学者很容易出现因为误用命令将代码给控制版本控制没了的状况（好吧是我）。

但相信我，和 Vim 一样，Git 是一款你最终掌握之后会感叹“它值得！”的神器。

## 如何学习 Git

和 Vim 不同，我不建议初学者在一知半解的情况下贸然使用 Git，因为它的内部逻辑并不能熟能生巧，而是需要花时间去理解。我推荐的学习路线如下：

1. 阅读这篇 [Git tutorial](https://missing.csail.mit.edu/2020/version-control/)，视频的话可以看这个[尚硅谷Git教程](https://www.bilibili.com/video/BV1vy4y1s7k6)
2. 阅读这本开源书籍 [Pro Git](https://git-scm.com/book/en/v2) 的 Chapter1 - Chapter5，是的没错，学 Git 需要读一本书（捂脸）。
3. 此时你已经掌握了 Git 的原理和绝大部分用法，接下来就可以在实践中反复巩固 Git 的命令了。但用好它同样是一门哲学，我个人觉得这篇[如何写好 Commit Message](https://chris.beams.io/posts/git-commit/) 的博客非常值得一读。
4. 好的此时你已经爱上了 Git，你已经不满足于学会它了，你想自己实现一个 Git！巧了，我当年也有这样的想法，[这篇 tutorial](https://wyag.thb.lt/) 可以满足你！
5. 什么？光实现一个 Git 无法满足你？小伙子/小仙女有前途，巧的是我也喜欢造轮子，这两个 GitHub 项目 [build-your-own-x](https://github.com/danistefanovic/build-your-own-x) 和 [project-based-learning](https://github.com/tuvtran/project-based-learning) 收录了你能想到的各种造轮子教程，比如：自己造个编辑器、自己写个虚拟机、自己写个 docker、自己写个 TCP 等等等等。

May 21, 2024

# GitHub

## GitHub 是什么

从功能上来说，GitHub 是一个在线代码托管平台。你可以将你的本地 Git 仓库托管到 GitHub 上，供多人同时开发浏览。但现如今 GitHub 的意义已远不止如此，它已经演变为一个非常活跃且资源极为丰富的开源交流社区。全世界的软件开发者在 GitHub 上分享各式各样种类繁多的开源软件。大到工业级的深度学习框架 PyTorch, TensorFlow，小到几十行的实用脚本，既有硬核的知识分享，也有保姆级的教程指导，甚至很多技术书籍也在 GitHub上开源（例如诸位正在看的这本——如果我厚着脸皮勉强称之为书的话）。闲来无事逛逛 GitHub 已经成为了我日常生活的一部分。

在 GitHub 里，星星是对一个项目至高无上的肯定，如果你觉得这本书对你有用的话，欢迎通过右上角的链接进入仓库主页献出你宝贵的星星✨。

## 如何使用 GitHub

如果你还从未在 GitHub 上建立过自己的远程仓库，也没有克隆过别人的代码，那么我建议你从 [GitHub的官方教程](https://docs.github.com/cn/get-started)开始自己的开源之旅。

如果你想时刻关注 GitHub 上一些有趣的开源项目，那么我向你重磅推荐 [HelloGitHub](https://hellogithub.com/) 这个网站以及它的同名微信公众号。它会定期收录 GitHub 上近期开始流行的或者非常有趣的开源项目，让你有机会第一时间接触各类优质资源。

GitHub 之所以成功，我想是得益于“我为人人，人人为我”的开源精神，得益于知识分享的快乐。如果你也想成为下一个万人敬仰的开源大佬，或者下一个 star 破万的项目作者。那就把你在开发过程中灵感一现的 idea 化作代码，展示在 GitHub 上吧～

不过需要提醒的是，开源社区不是法外之地，很多开源软件并不是可以随意复制分发甚至贩卖的，了解各类[开源协议](https://www.runoob.com/w3cnote/open-source-license.html)并遵守，不仅是法律的要求，更是每个开源社区成员的责任。

May 21, 2024

# GNU Make

## 为什么学 GNU Make

大家第一次写 hello world 程序的时候一定都记得，在编辑完 `helloworld.c` 之后，需要用 `gcc` 编译生成可执行文件，然后再执行（如果你不理解前面这段话，请先自行谷歌 *gcc 编译* 并理解相关内容）。但如果你的项目由成百上千个 C 源文件组成，并且星罗棋布在各个子目录下，你该如何将它们编译链接到一起呢？假如你的项目编译一次需要半个小时（大型项目相当常见），而你只修改了一个分号，是不是还需要再等半个小时呢？

这时候 GNU Make 就闪亮登场了，它能让你在一个脚本里（即所谓的 `Makefile`）定义整个编译流程以及各个目标文件与源文件之间的依赖关系，并且只重新编译你的修改会影响到的部分，从而降低编译的时间。

## 如何学习 GNU Make

这里有一篇写得深入浅出的[文档](https://seisman.github.io/how-to-write-makefile/overview.html)供大家参考。

GNU Make 掌握起来相对容易，但用好它需要不断的练习。将它融入到自己的日常开发中，勤于学习和模仿其他优秀开源项目里的 `Makefile` 的写法，总结出适合自己的 template，久而久之，你对 GNU Make 的使用会愈加纯熟。

May 21, 2024

# CMake

## 为什么学习 CMake

CMake 是类似于 GNU make 的跨平台自动软件构建工具，使用 CMakeLists.txt 定义构建规则，相比于 make 它提供了更多的功能，在各种软件构建上广泛使用。**强烈建议学习使用 GNU Make 和熟悉 `Makefile` 后再学习 CMake**。

## 如何学习 CMake

`CMakeLists.txt` 比 `Makefile` 更为抽象，理解和使用难度也更大。现阶段很多 IDE (如 Visual Studio, CLion) 提供了自动生成 `CMakeLists.txt` 的功能，但掌握 `CMakeLists.txt` 的基本用法仍然很有必要。除了 [CMake 官方 Tutorial](https://cmake.org/cmake/help/latest/guide/tutorial/index.html) 外，上海交通大学 IPADS 组新人培训也提供了[大约一小时的视频教程](https://www.bilibili.com/video/BV14h41187FZ)。

May 21, 2024

# LaTeX

## 为什么学 LaTeX

如果你需要写论文，那么请直接跳到下一节，因为你不学也得学。

LaTeX 是一种基于 TeX 的排版系统，由图灵奖得主 Lamport 开发，而 Tex 则是由 Knuth 最初开发，这两位都是计算机界的巨擘。当然开发者强并不是我们学习 LaTeX 的理由，LaTeX 和常见的所见即所得的 Word 文档最大的区别就是用户只需要关注写作的内容，而排版则完全交给软件自动完成。这让没有任何排版经验的普通人得以写出排版非常专业的论文或文章。

Berkeley 计算机系教授 Christos Papadimitriou 曾说过一句半开玩笑的话：

> Every time I read a LaTeX document, I think, wow, this must be correct!

## 如何学习 LaTeX

推荐的学习路线如下：

- LaTeX 的环境配置是个比较头疼的问题。如果你本地配置 LaTeX 环境出现了问题，可以考虑使用 [Overleaf](https://www.overleaf.com/) 这个在线 LaTeX 编辑网站。站内不仅有各种各样的 LaTeX 模版供你选择，还免去了环境配置的难题。
- 阅读下面三篇 Tutorial: [Part-1](https://www.overleaf.com/latex/learn/free-online-introduction-to-latex-part-1), [Part-2](https://www.overleaf.com/latex/learn/free-online-introduction-to-latex-part-2), [Part-3](https://www.overleaf.com/latex/learn/free-online-introduction-to-latex-part-3)。
- 学习 LaTeX 最好的方式当然是写论文，不过从一门数学课入手用 LaTeX 写作业也是一个不错的选择。

其他值得推荐的入门学习资料如下：

- 一份简短的安装 LaTeX 的介绍 [[GitHub](https://github.com/OsbertWang/install-latex-guide-zh-cn)] 或者 TEX Live 指南（texlive-zh-cn）[[PDF](https://www.tug.org/texlive/doc/texlive-zh-cn/texlive-zh-cn.pdf)] 可以帮助你完成安装和环境配置过程
- 一份（不太）简短的 LaTeX2ε 介绍（lshort-zh-cn）[[PDF](https://mirrors.ctan.org/info/lshort/chinese/lshort-zh-cn.pdf)] [[GitHub](https://github.com/CTeX-org/lshort-zh-cn)] 是由 CTEX 开发小组翻译的，可以帮助你快速准确地入门，建议通读一遍
- 刘海洋的《LaTeX 入门》，可以当作工具书来阅读，有问题再查找，跳过 CTEX 套装部分
- [现代 LaTeX 入门讲座](https://github.com/stone-zeng/latex-talk)
- [一份其实很短的 LaTeX 入门文档](https://liam.page/2014/09/08/latex-introduction/)

May 21, 2024

# Docker

## 为什么使用 Docker

使用别人写好的软件/工具最大的障碍是什么——必然是配环境。配环境带来的折磨会极大地消解你对软件、编程本身的兴趣。虚拟机可以解决配环境的一部分问题，但它庞大笨重，且为了某个应用的环境配置好像也不值得模拟一个全新的操作系统。

[Docker](https://www.docker.com/) 的出现让环境配置变得（或许）不再折磨。简单来说 Docker 使用轻量级的“容器”（container）而不是整个操作系统去支持一个应用的配置。应用自身连同它的环境配置被打包为一个个 image 可以自由运行在不同平台的一个个 container 中，这极大地节省了所有人的时间成本。

## 如何学习 Docker

[Docker 官方文档](https://docs.docker.com/)当然是最好的初学教材，但最好的导师一定是你自己——尝试去使用 Docker 才能享受它带来的便利。Docker 在工业界发展迅猛并已经非常成熟，你可以下载它的桌面端并使用图形界面。

当然，如果你像我一样，是一个疯狂的造轮子爱好者，那不妨自己亲手写一个[迷你 Docker](https://github.com/PKUFlyingPig/rubber-docker) 来加深理解。

[KodeKloud Docker for the Absolute Beginner](https://kodekloud.com/courses/docker-for-the-absolute-beginner/) 全面的介绍了 Docker 的基础功能，并且有大量的配套练习，同时提供免费的云环境来完成练习。其余的云相关的课程如 Kubernetes 需要付费，但个人强烈推荐：讲解非常仔细，适合从 0 开始的新手；有配套的 Kubernetes 的实验环境，不用被搭建环境劝退。

May 21, 2024

# Scoop

## 为什么使用 Scoop

在 Windows 下，搭建开发环境一直是一个复杂且困难的问题。由于没有一个统一的标准，导致各种开发环境的安装方式差异巨大，需要付出很多不必要的时间成本。而 Scoop 可以帮助你统一安装并管理常见的开发软件，省去了手动下载安装，配置环境变量等繁琐步骤。

例如安装 python 和 nodejs 只需要执行：

```powershell
scoop install python
scoop install nodejs
```

## 安装 Scoop

Scoop 需要 [Windows PowerShell 5.1](https://aka.ms/wmf5download) 或者 [PowerShell](https://aka.ms/powershell) 作为运行环境，如果你使用的是 Windows 10 及以上版本，Windows PowerShell 是内置在系统中的。而 Windows 7 内置的 Windows PowerShell 版本过于陈旧，你需要手动安装新版本的 PowerShell。

> 由于发现很多同学在设置 Windows 用户时使用了中文用户名，导致了用户目录也变成了中文名。如果按照 Scoop 的默认方式将软件安装到用户目录下，可能会造成部分软件执行错误。所以这里推荐安装到自定义目录，如果需要其他安装方式请参考： [ScoopInstaller/Install](https://github.com/ScoopInstaller/Install)

```powershell
# 设置 PowerShell 执行策略
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
# 下载安装脚本
irm get.scoop.sh -outfile 'install.ps1'
# 执行安装, --ScoopDir 参数指定 Scoop 安装路径
.\install.ps1 -ScoopDir 'C:\Scoop'
```

## 使用 Scoop

Scoop 的官方文档对于新手非常友好，相对于在此处赘述更推荐阅读 [官方文档](https://github.com/ScoopInstaller/Scoop) 或 [快速入门](https://github.com/ScoopInstaller/Scoop/wiki/Quick-Start) 。

## Q&A

### Scoop 能配置镜像源吗？

Scoop 社区仅维护安装配置，所有的软件都是从该软件官方提供的下载链接进行下载，所以无法提供镜像源。如果因为你的网络环境导致多次下载失败，那么你需要一点点 [魔法](https://csdiy.wiki/必学工具/翻墙/)。

### 为什么找不到 Java8？

原因同上，官方已不再提供 Java8 的下载链接，推荐使用 [ojdkbuild8](https://github.com/ScoopInstaller/Java/blob/master/bucket/ojdkbuild8.json) 替代。

### 我需要安装 python2 该如何操作？

对于已经过时弃用的软件，Scoop 社区会将其从 [ScoopInstaller/Main](https://github.com/ScoopInstaller/Main) 中移除并将其添加到 [ScoopInstaller/Versions](https://github.com/ScoopInstaller/Versions) 中。如果你需要这些软件的话需要手动添加 bucket：

```powershell
scoop bucket add versions
scoop install python27
```

May 21, 2024

# 日常学习工作流

> Contributed by [@HardwayLinka](https://github.com/HardwayLinka)

计算机领域的知识覆盖面很广并且更新速度很快，因此保持终身学习的习惯很重要。但在日常开发和学习的过程中，我们获取知识的来源相对复杂且细碎。有成百上千页的文档手册，也有寥寥数语的博客，甚至闲暇时手机上划过的某则新闻和公众号都有可能包含我们感兴趣的知识。因此，如何利用现有的各类工具，形成一套适合自己的学习工作流，将不同来源的知识碎片整合进属于自己的知识库，方便之后的查阅与复习，就显得尤为重要。经过两年工作之余的学习后，我磨合出了以下学习工作流：

![img](https://cdn.jsdelivr.net/gh/Halerfermatqing/images_bed@main/typora/202406031533223.png)

## 底层核心逻辑

一开始我学习新知识时会参考中文博客，但在代码实践时往往会发现漏洞和bug。我逐渐意识到我参考的信息可能是错误的，毕竟发博客的门槛低，文章可信度不高，于是我开始查阅一些相关的中文书籍。

中文书籍的确是比较全面且系统地讲解了知识点，但众所周知，计算机技术更迭迅速，又因为老美在 CS 方面一直都是灯塔，所以一般中文书籍里的内容会滞后于当前最新的知识，导致我跟着中文书籍实践会出现软件版本差异的问题。这时我开始意识到一手信息的重要性，有些中文书籍是翻译英文书籍的，一般翻译一本书也要一两年，这会导致信息传递的延迟，还有就是翻译的过程中信息会有损失。如果一本中文书籍不是翻译的呢，那么它大概率也参考了其他书籍，参考的过程会带有对英文原著中语义理解的偏差。

于是我就顺其自然地开始翻阅英文书籍。不得不说，英文书籍内容的质量整体是比中文书籍高的。后来随着学习的层层深入，以知识的时效性和完整性出发，我发现 `源代码` > `官方文档` > `英文书籍` > `英文博客` > `中文博客`，最后我得出了一张 `信息损失图`：

![img](https://cdn.sspai.com/2022/10/11/bf07c1965a2e5bdf3f00644737789e2e.png)

虽然一手信息很重要，但后面的 N 手信息并非一无是处，因为这 N 手资料里包含了作者对源知识的转化——例如基于某种逻辑的梳理（流程图、思维导图等）或是一些自己的理解（对源知识的抽象、类比、延伸到其他知识点），这些转化可以帮助我们更快地掌握和巩固知识的核心内容，就如同初高中学习时使用的辅导书。 此外，学习的过程中和别人的交流十分重要，这些 N 手信息同时起了和其他作者交流的作用，让我们能采百家之长。所以这提示我们学习一个知识点时先尽量选择质量更高的，信息损失较少的信息源，同时不妨参考多个信息源，让自己的理解更加全面准确。

现实工作生活中的学习很难像学校里一样围绕某个单一知识点由浅入深，经常会在学习过程中涉及到其他知识点，比如一些新的专有名词，一篇没有读过的经典论文，一段未曾接触过的代码等等。这就要求我们勤于思考，刨根究底地“递归”学习，给多个知识点之间建立联系。

## 选择合适的笔记软件

工作流的骨架围绕 `单个知识点多参考源，勤于提问给多个知识点之间建立联系` 的底层核心逻辑建立。我们写论文其实就是遵循这个底层逻辑的。论文一般会有脚注去解释一些关键字，并且论文末尾会有多个参考的来源，但是我们平时写笔记会随意得多，因此需要更灵活的方式。

平时写代码习惯在 IDE 里一键跳转，把相关的函数和实现很好地联系在了一起。你也许会想，如果笔记也能像代码那样可以跳转就好了。现在市面上 `双链笔记软件` 就可以很好地解决这一痛点，例如 Roam Research、Logseq、Notion 和 Obsidian。Roam Research 和 Logseq 都是基于大纲结构的笔记软件，而 `大纲结构` 是劝退我使用这两款软件的原因。一是 `大纲结构` 做笔记容易使文章纵向篇幅太长，二是如果嵌套结构过多会占横向的篇幅。Notion 页面打开慢，弃之。最终我选择了 Obsidian，原因如下：

- Obsidian 基于本地，打开速度快，且可存放很多电子书。我的笔记本是 32g 内存的华硕天选一代，拿来跑 Obsidian 可以快到飞起
- Obsidian 基于 Markdown。这也是一个优势，如果笔记软件写的笔记格式是自家的编码格式，那么不方便其他第三方拓展，也不方便将笔记用其他软件打开，比如 qq 音乐下载歌曲有自己的格式，其他播放器播放不了，这挺恶心人的
- Obsidian 有丰富的插件生态，并且这个生态既大又活跃，即插件数量多，且热门插件的 star 多，开发者会反馈用户 issue，版本会持续迭代。借助这些插件，可以使 Obsidian 达到 `all in one` 的效果，即各类知识来源可以统一整合于一处

## 信息的来源

Obsidian 的插件使其可以支持 pdf 格式，而其本身又支持 Markdown 格式。如果想要 `all in one`，那么可以基于这两个格式，将其他格式文件转换为 pdf 或者 Markdown。 那么现在就面临着两个问题：

- 有什么格式
- 怎么转换为 pdf 或 Markdown

![img](https://cdn.sspai.com/2022/10/11/3801b1c9b94286566fe677e3b12cc7b0.png)

### 有什么格式

文件格式依托于其展示的平台，所以在看有什么格式之前，可以罗列一下我平时获取信息的来源：

![img](https://cdn.sspai.com/2022/10/11/07e97f372850054958d4961a3787a93f.png)

可以看到主要分为 `文章`、`论文`、`电子书`、`课程`四类，包含的格式主要有 `网页`、`pdf` 、`mobi`、`azw`、`azw3`。

### 怎么转换为 pdf 或 Markdown

在线的文章和课程等大多以网页形式呈现，而将网页转换为 Markdown 可以使用剪藏软件，它可以将网页文章转换为多种文本格式文件。我选择的工具是简悦，使用简悦可以将几乎所有平台的文章很好地剪藏为 Markdown 并且导入到 Obsidian。

![img](https://cdn.sspai.com/2022/10/11/211cffa78f20a9e7286a7419e9e0b878.png)

对于论文和电子书而言如果格式本身就是 pdf 则万事大吉，但如果是其他格式则可以使用 calibre 进行转换：

![img](https://cdn.sspai.com/2022/10/11/51575f65f6f4c6edfa6c5b97fd16d625.png)

现在利用 Obsidian 的 pdf 插件和其原生的 markdown 支持就可以畅快无比地做笔记并且在这些文章的对应章节进行无缝衔接地引用跳转啦（具体操作参考下文的“信息的处理”模块）。

![img](https://cdn.sspai.com/2022/10/11/d64a9a2d6406d2d367dcb505ede69c83.png)

### 如何统一管理信息来源

对于 pdf 等文件类资源可以本地或者云端存储，而网页类资源则可以分门别类地放入浏览器的收藏夹，或者剪藏成 markdown 格式的笔记，但是网页浏览器不能实现移动端的网页收藏。为了实现跨端网页收藏我选用了 Cubox，在手机端看到感兴趣的网页时只需小手一划，便能将网页统一保存下来。虽然免费版只能收藏 100 个网页，但其实够用了，还可以在收藏满时督促自己赶紧剪藏消化掉这些网页，让收藏不吃灰。

![img](https://cdn.sspai.com/2022/10/11/ad7ebfcb4619f64a41d328b88e0e3a12.png)

除此之外，回想一下我们平时收藏的网页，就会发现有很多并不是像知乎、掘金这类有完整功能的博客平台，更多的是个人建的小站，而这些小站往往没有移动端应用，这样平时刷手机的时候也看不到，放到浏览器的收藏夹里又容易漏了看，有新文章发布我们也不能第一时间收到通知，这个时候就需要一种叫 `RSS` 的通信协议。

`RSS`（英文全称：RDF Site Summary 或 Really Simple Syndication），中文译作简易信息聚合，也称聚合内容，是一种消息来源格式规范，用以聚合多个网站更新的内容并自动通知网站订阅者。电脑端可以借助 `RSSHub Radar` 来快速发现和生成 `RSS` 订阅源，接着使用 `Feedly` 来订阅这些 `RSS` 订阅源（`RSSHub Radar` 和 `Feedly` 在 chrome 浏览器中均有官方插件）。

![img](https://cdn.sspai.com/2022/10/11/5df6cd9d967f190df35928e781f9185f.png)

到这里为止，收集信息的流程已经比较完备了。但资料再多，分类规整得再漂亮，也得真正内化成自己的才管用。因此在收集完信息后就得进一步地处理信息，即阅读这些信息，如果是英文信息的话还得搞懂英文的语义，加粗高亮重点句子段落，标记有疑问的地方，发散联想相关的知识点，最后写上自己的总结。那么在这过程中需要使用到什么工具呢？

## 信息的处理

### 英文信息

面对英文的资料，我以前是用 `有道词典` 来划词翻译，遇到句子的话就使用谷歌翻译，遇到大段落时就使用 `deepl`，久而久之，发现这样看英语文献太慢了，得用三个工具才能满足翻译这一个需求，如果有一个工具能够同时实现对单词、句子和段落的划词翻译就好了。我联想到研究生们应该会经常接触英语文献，于是我就搜 `研究生` + `翻译软件`，在检索结果里我最终选择了 `Quicker` + `沙拉查词` 这个搭配来进行划词翻译。

![img](https://cdn.sspai.com/2022/10/11/a7ebb1d3c46702b56bd6d171dfcfc075.png)

使用这套组合可以实现在浏览器外的其他软件内进行划词翻译，并且支持单词、句子和段落的翻译，以及每次的翻译会有多个翻译平台的结果。btw，如果查单词时不着急的话，可以顺便看看 `科林斯高阶` 的翻译，这个词典的优点就是会用英文去解释英文，可以提供多个上下文帮助你理解，对于学习英文单词也有帮助，因为用英文解释英文才更接近英语的思维。

![img](https://cdn.sspai.com/2022/10/11/article/827c9a8048c83e504ccb15893702bf09)

### 多媒体信息

处理完文本类的信息后，我们还得思考一下怎么处理多媒体类的信息。此处的多媒体我特指英文视频，因为我没有用播客或录音学习的习惯，而且我已经基本不看中文教程了。现在很多国外名校公开课都是以视频的形式，如果能对视频进行做笔记会不会有帮助呢？不知道大家有没这样的想法，就是如果能把老师上课讲的内容转换成文本就好了，因为平时学习时我们看书的速度往往会比老师讲课的速度快。刚好 `Language Reactor` 这个软件可以将油管和网飞内视频的字幕导出来，同时附上中文翻译。

我们可以把 `Language Reactor` 导出的字幕复制到 `Obsidian` 里面作为文章来读。除了出于学习的需求，也可以在平时看油管的视频时打开这个插件，这个插件可以同时显示中英文字幕，并且可以单击选中英文字幕中你认为生僻的单词后显示单词释义。

![img](https://cdn.sspai.com/2022/10/11/364c8e6ed263affa84d9eee61338b4af.png)

但阅读文本对于一些抽象的知识点来说并不是效率最高的学习方式。俗话说，一图胜千言，能不能将某一段知识点的文本和对应的图片甚至视频画面操作联系起来呢？我在浏览 `Obsidian` 的插件市场时，发现了一个叫 `Media Extended` 的插件，这个插件可以在你的笔记里添加跳转到视频指定时间进度的链接，相当于把你的笔记和视频连接起来了！这刚好可以和我上文提到的生成视频中英文字幕搭配起来，即每一句字幕对应一个时间，并且能根据时间点跳转到视频的指定进度，如此一来如果需要在文章中展示记录了操作过程的视频的话，就不需要自己去截取对应的视频片段，而是直接在文章内就能跳转！

![img](https://cdn.sspai.com/2022/10/11/17554cfdf662d5719ada453674012fdb.gif)

`Obsidian` 里还有一个很强大的插件，叫 `Annotator`，它可以实现笔记内跳转到 pdf 原文

![img](https://cdn.sspai.com/2022/10/11/article/b56994bf9a306830d8b0b8112677d3ec)

现在，使用 `Obsidian` 自带的双链功能，可以实现笔记间相互跳转，结合上述两个插件，可以实现笔记到多媒体的跳转，信息的处理过程已经完备。一般我们学习的过程相当于上山和下山，刚学的时候就好像上山，很陌生、吃力，所谓学而时习之，复习或练习的过程就像下山，没有陌生感，不见得轻松，但非走不可。那么如何把复习这一过程纳入工作流的环节里呢？

## 信息的回顾

`Obsidian` 内已经有一个连接 `Anki` 的插件，`Anki` 就是大名鼎鼎的、基于间隔重复的记忆软件。使用该插件可以截取笔记的片段导出到 `Anki` 并变成一张卡片，卡片内也有跳转回笔记原文的链接

![img](https://cdn.sspai.com/2022/10/11/1f7cebd8dd28f664d77cbf0ab228c406.gif)

## 总结

这个工作流是在我这两年业余时间学习时所慢慢形成的，在学习过程中因为对一些重复性的过程而感到厌倦，正是这种厌倦产生了某种特定的需求，恰好在平时网上冲浪时了解到的一些工具满足了我这些需求。不要为了虚无的满足感而将工具强行拼凑到自己的工作流中，人生苦短，做实事最紧要。

btw，此篇文章是讲解工作流的演化思路，如果对此工作流的实现细节感兴趣，建议阅读完本文后再按顺序阅读以下文章

1. [3000 + 小时积累的学习工作流](https://sspai.com/post/75969)
2. [Obsidian 的高级玩法 | 打造能跳转到任何格式文件的笔记](https://juejin.cn/post/7145351315705577485)

May 21, 2024

# 实用工具箱

## 下载工具

- [Sci-Hub](https://sci-hub.se/): Elbakyan 女神向你挥手，旨在打破知识壁垒的革命性网站。
- [Library Genesis](http://libgen.is/): 电子书下载网站。
- [Z-library](https://zlibrary-global.se/): 电子书下载网站（在 [Tor](https://www.torproject.org/) 下运行较佳，[链接](http://loginzlib2vrak5zzpcocc3ouizykn6k5qecgj2tzlnab5wcbqhembyd.onion/)）。
- [Z-ePub](https://z-epub.com/): ePub 电子书下载网站。
- [PDF Drive](https://www.pdfdrive.com/): PDF 电子书搜索引擎。
- [MagazineLib](https://magazinelib.com/): PDF 电子杂志下载网站。
- [BitDownloader](https://bitdownloader.io/): 油管视频下载器。
- [qBittorrent](https://www.qbittorrent.org/download.php): BitTorrent 客户端。
- [uTorrent](https://www.utorrent.com/): BitTorrent 客户端。
- [全国标准信息公共服务平台](https://std.samr.gov.cn/)：各类标准查询和下载官方平台。
- [标准知识服务系统](http://www.standards.com.cn/)：检索与阅读所需标准。
- [MSDN,我告诉你](https://msdn.itellyou.cn/): Windows 操作系统镜像下载站，也有许多其他软件的下载。

## 设计工具

- [excalidraw](https://excalidraw.com/): 一款手绘风格的绘图工具，非常适合绘制课程报告或者PPT内的示意图。
- [tldraw](https://www.tldraw.com/): 一个绘图工具，适合画流程图，架构图等。
- [draw.io](https://app.diagrams.net/): 强大简洁的在线的绘图网站，支持流程图，UML图，架构图，原型图等等，支持 Onedrive, Google Drive, Github 导出，同时提供离线客户端。
- [origamiway](https://www.origamiway.com/paper-folding-crafts-step-by-step.shtml): 手把手教你怎么折纸。
- [thingiverse](https://www.thingiverse.com/): 囊括各类 2D/3D 设计资源，其 STL 文件下载可直接 3D 打印。
- [iconfont](https://www.iconfont.cn/): 国内最大的图标和插画资源库，可用于开发或绘制系统架构图。
- [turbosquid](https://www.turbosquid.com/): 可以购买各式各样的模型。
- [flaticon](https://www.flaticon.com/): 可下载免费且高质量的图标。
- [标准地图服务系统](http://bzdt.ch.mnr.gov.cn/): 可以下载官方标准地图。
- [PlantUML](https://plantuml.com/zh/): 可以使用代码快速编写 UML 图。

## 编程相关

- [sqlfiddle](http://www.sqlfiddle.com/): 一个简易的在线 SQL Playground。
- [sqlzoo](https://sqlzoo.net/wiki/SQL_Tutorial)：在线练习 sql 语句。
- [godbolt](https://godbolt.org/): 非常方便的编译器探索工具。你可以写一段 C/C++ 代码，选择一款编译器，然后便可以观察生成的具体汇编代码。
- [explainshell](https://explainshell.com/): 你是否曾为一段 shell 代码的具体含义感到困扰？manpage 看半天还是不明所以？试试这个网站！
- [regex101](https://regex101.com/): 正则表达式调试网站，支持各种编程语言的匹配标准。
- [typingtom](https://www.typingtom.com/lessons): 针对程序员的打字练习/测速网站。
- [wrk](https://github.com/wg/wrk): 网站压测工具。
- [gbmb](https://www.gbmb.org/): 数据单位转换。
- [tools](https://tools.fun/): 在线工具合集。
- [github1s](https://github1s.com/): 用网页版 VS Code 在线阅读 GitHub 代码。
- [visualgo](https://visualgo.net/en): 算法可视化网站。
- [DataStructureVisual](http://www.rmboot.com/): 数据结构可视化网站。
- [Data Structure Visualizations](https://www.cs.usfca.edu/~galles/visualization/Algorithms.html): 数据结构与算法的可视化网站。
- [learngitbranching](https://learngitbranching.js.org/?locale=zh_CN): 可视化学习 git。
- [UnicodeCharacter](https://unicode-table.com/en/): Unicode 字符集网站。
- [cyrilex](https://extendsclass.com/regex-tester.html): 一个用于测试和可视化正则表达式的网站，支持各种编程语言标准。
- [mockium](https://softwium.com/mockium/): 生成测试数据的平台。

## 学习网站

- [HFS](https://hepsoftwarefoundation.org/training/curriculum.html): 各类软件教程。
- [Shadertoy](https://www.shadertoy.com/): 编写各式各样的 shader。
- [comments-for-awesome-courses](https://conanhujinming.github.io/comments-for-awesome-courses/): 名校公开课评价网。
- [codetop](https://codetop.cc/home): 企业题库。
- [cs-video-courses](https://github.com/Developer-Y/cs-video-courses): 带有视频讲座的计算机科学课程列表。
- [bootlin](https://elixir.bootlin.com/linux/v2.6.39.4/source/include/linux): 在线阅读 Linux 源码。
- [ecust-CourseShare](https://github.com/tianyilt/ecnu-PGCourseShare): 华东师范大学研究生课程攻略共享计划。
- [REKCARC-TSC-UHT](https://github.com/PKUanonym/REKCARC-TSC-UHT): 清华大学计算机系课程攻略。
- [seu-master](https://github.com/oneman233/seu-master): 东南大学研究生课程资料整理。
- [菜鸟教程](https://www.runoob.com/): 计算机相关知识的简要的教程。
- [FreeBSD 从入门到跑路](https://book.bsdcn.org/): 一本 FreeBSD 的中文教程。
- [MDN Web Docs](https://developer.mozilla.org/zh-CN/docs/Learn): MDN 网络开发入门手册。
- [Hello 算法](https://www.hello-algo.com/): 动画图解、能运行、可提问的数据结构与算法快速入门教程。

## 百科网站/词典性质的网站

- [os-wiki](https://wiki.osdev.org/Main_Page): 操作系统技术资源百科全书。
- [FreeBSD Documentation](https://docs.freebsd.org/en/): FreeBSD 官方文档。
- [Python3 Documentation](https://docs.python.org/zh-cn/3/): Python3 官方中文文档。
- [C++ Reference](https://en.cppreference.com/w/): C++ 参考手册。
- [OI Wiki](https://oi-wiki.org/): 编程竞赛知识整合站点。
- [Microsoft Learn](https://learn.microsoft.com/zh-cn/): 微软官方的学习平台，包含了绝大多数微软产品的文档。
- [Arch Wiki](https://wiki.archlinux.org/): 专为 Arch Linux 而写的 Wiki，包含了大量 Linux 相关的知识。
- [Qt Wiki](https://wiki.qt.io/Main): Qt 官方 Wiki。
- [OpenCV 中文文档](https://opencv.apachecn.org/#/): OpenCV 的社区版中文文档。
- [npm Docs](https://docs.npmjs.com/): npm 官方文档。

## 交流平台

- [GitHub](https://github.com/): 许多开源项目的托管平台，也是许多开源项目的主要交流平台，通过查看 issue 可以解决许多问题。
- [StackExchange](https://stackexchange.com/): Stack Exchange 是由 181 个问答社区组成（其中包括 Stack Overflow）的编程社区。
- [StackOverflow](https://stackoverflow.com/): Stack Overflow 是一个与程序相关的 IT 技术问答网站。
- [Gitee](https://gitee.com/): 一个类似于 GitHub 的代码托管平台，可以在对应项目的 issue 里查找一些常见问题的解答。
- [知乎](https://www.zhihu.com/): 一个类似于 Quora 的问答社区，可以在其中提问，一些问答包含有计算机的知识。
- [博客园](https://www.cnblogs.com/): 一个面向开发者的知识分享社区，拥有一些常见问题的博客，正确率不能保证，请谨慎使用。
- [CSDN](https://blog.csdn.net/): 拥有一些常见问题的博客，正确率不能保证，请谨慎使用。

## 杂项

- [tophub](https://tophub.today/): 新闻热榜合集（综合了知乎、微博、百度、微信等）。
- [feedly](https://feedly.com/): 著名的 RSS 订阅源阅读器。
- [speedtest](https://www.speedtest.net/zh-Hans): 在线网络测速网站。
- [public-apis](https://github.com/public-apis/public-apis): 公共 API 合集列表。
- [numberempire](https://zh.numberempire.com/derivativecalculator.php): 函数求导工具。
- [sustech-application](https://sustech-application.com/#/grad-application/computer-science-and-engineering/README): 南方科技大学经验分享网。
- [vim-adventures](https://vim-adventures.com/): 一款基于 vim 键盘快捷键的在线游戏。
- [vimsnake](https://vimsnake.com/): 利用 vim 玩贪吃蛇。
- [keybr](https://www.keybr.com/): 学习盲打的网站。
- [Awesome C++](https://cpp.libhunt.com/): 很棒的 C/C++ 框架、库、资源精选列表。
- [HelloGitHub](https://hellogithub.com/): 分享 GitHub 上有趣、入门级的开源项目。
- [Synergy](https://github.com/DEAKSoftware/Synergy-Binaries): 一套键鼠能控制多台电脑。

May 21, 2024

# 毕业论文

## 为什么写这份教程

2022年，我本科毕业了。在开始动手写毕业论文的时候，我尴尬地发现，我对 Word 的掌握程度仅限于调节字体、保存导出这些傻瓜功能。曾想转战 Latex，但论文的段落格式要求调整起来还是用 Word 更为方便，经过一番痛苦缠斗之后，总算是有惊无险地完成了论文的写作和答辩。为了不让后来者重蹈覆辙，遂把相关资源整理成一份开箱即用的文档，供大家参考。

## 如何用 Word 写毕业论文

正如将大象装进冰箱需要三步，用 Word 写毕业论文也只需要简单三步：

- 确定论文的格式要求：通常学院都会下发毕业论文的格式要求（各级标题的字体字号、图例和引用的格式等等），如果更为贴心的话甚至会直接给出论文模版（如是此情况请直接跳转到下一步）。很不幸的是，我的学院并没有下发标准的论文格式要求，还提供了一份格式混乱几乎毫无用处的论文模版膈应我，被逼无奈之下我找到了北京大学研究生的[论文格式要求](https://github.com/PKUFlyingPig/Thesis-Template/blob/master/北京大学研究生学位论文写作指南.pdf)，并按照其要求制作了[一份模版](https://github.com/PKUFlyingPig/Thesis-Template/blob/master/论文模版.docx)，大家需要的话自取，本人不承担无法毕业等任何责任。
- 学习 Word 排版：到达这一步的童鞋分为两类，一是已经拥有了学院提供的标准模版，二是只有一份虚无缥缈的格式要求。那现在当务之急就是学习基础的 Word 排版技术，对于前者可以学会使用模版，对于后者则可以学会制作模版。此时切记不要雄心勃勃地选择一个十几个小时的 Word 教学视频开始头悬梁锥刺股，因为生产一份应付毕业的学术垃圾只要学半小时能上手就够了。我当时看的[一个 B 站的教学视频](https://www.bilibili.com/video/BV1YQ4y1M73G?p=1&vd_source=a4d76d1247665a7e7bec15d15fd12349)，短小精悍非常实用，全长半小时极速入门。
- 生产学术垃圾：最容易的一步，大家八仙过海，各显神通吧，祝大家毕业顺利～～

May 21, 2024

# 信息检索

## 前言

*碰到问题，记住第一件事是 **翻阅文档** ，不要一开始就直接搜索或者找人问，翻阅FAQ可能会快速找到答案。*

信息检索，我的理解来说，实际上就是灵活运用搜索引擎中，方便快捷的搜到需要的信息，包括但不限于编程。

编程最重要的，就是 STFW(search the fucking web) 和 RTFM(read the fucking Manual) ，首先要读文档，第二要学会搜索，网上那么多资源，怎么用，就需要信息检索。

要搜索，我们首先要搞清楚搜索引擎是如何工作的：

## 搜索引擎工作原理

搜索引擎的工作过程大体可以分成三阶段：[^1]

1. 爬行和抓取：搜索引擎蜘蛛通过跟踪链接访问网页，获取网页 HTML 代码存入数据库。
2. 预处理：索引程序对抓取来的网页数据进行文字提取，中文分词，索引等处理，以备排名程序调用。
3. 排名：用户输入关键词后，排名程序调用索引库数据，计算相关性，然后按一定格式生成搜索结果页面。

第一步，就是大家经常听说的网络爬虫，一般 Python 卖课的都会吹这个东西。简单可以理解为，我用一个自动的程序，下载网站中的所有文本、图片等相关信息，然后存入本地的磁盘。

第二步是搜索引擎的核心，但是对于我们使用来说，并不是特别关键，大致可以理解为洗干净数据，然后入库页面，每个页面加入关键字等信息方便我们查询。

第三步跟我们息息相关，不管是什么搜索网站， google 、百度、 Bing ，都一样，输入关键字或者需要查询的内容，搜索引擎会给你返回结果。本文就是教你如何获取更好的结果。

## 基础搜索技巧

根据上述的工作原理，我们大致就能明白，其实可以把搜索引擎当作一个比较聪明的数据库，更好的使用查询条件就能更快速的找到你想要的信息，下面介绍一些搜索的技巧：

### 使用英文

首先我们要知道一件事，编程中，最好使用英文搜索。原因主要有几点：

1. 编程和各种软件操作中，英文资料质量比中文资料和其他语言资料高，英文通用性还是更好些
2. 因为翻译问题，英文的名词比中文准确通用
3. 中文搜索中，分词系统不准会导致歧义，比如 Google 搜中文可能会搜不出几条有用结果

如果你英文不好，用百度翻译或者搜狗翻译，足够了。

当然下面的文档为了举例方便，都还是用中文例子。

### 提炼关键词

搜索时不要搜索整句话，虽然搜索引擎会自动帮助我们分词检索，但是整句和关键字搜索出来的结果再准确度和顺序上会有很大差别。搜索引擎是机器，并不是你的老师或者同事，看上面的流程，搜索实际上是去检索搜索引擎爬出来的数据库，你可以理解为关键字比模糊检索要快而且准确。

我们需要提炼问题，确定我们到底需要解决什么问题。

例如，我想知道 vcpkg 如何集成到工程上而不是全局中，那么搜索 `vcpkg如何集成到工程上而不是全局中` 这种长句可能无法找到相关的结果，最好是拆分成单词，`vcpkg 集成到 工程 全局` 这样的搜索。其实这里只是举个例子，针对本条其实都能搜索出相关信息，但是越具体的问题，机器分词越可能出问题，所以最好是拆分关键字，使用词组或者断句来进行搜索。

### 替换关键字

还是上面那个例子，如果搜不出来，可以试试把工程换成项目，或者移出集成，如果不行，试一下高级搜索。

### 高级搜索

普通搜索引擎一般都支持高级搜索，包括 google ， bing ，百度， ecosia ，等等，大部分都支持，不过可能语法不同，一般通用的表示：

- 精准匹配： 精准匹配能保证搜索关键词完全被匹配上，一般是用双引号括起来
- 比如搜索线性代数，可以在输入框内输入 "线性代数"，搜索引擎将只匹配完整包含 “线性代数” 的页面，而不会搜索拆分成线性和代数两个词的页面
- 不包含关键字： 用 - 减号连接关键字，用于排除某些干扰词
- 包含关键字： 用 + 加号连接关键字
- 搜索特定文件类型： `filetype:pdf` 直接搜索 pdf 文件
- 搜索特定网址： `site:stackoverflow.com` 只搜索特定网站内的页面

一般可以参照网站说明，比如百度可以参照 [高级搜索](https://baike.baidu.com/item/高级搜索/1743887?fr=aladdin) ，Bing 可以参照 [高级搜索关键字](https://help.bing.microsoft.com/#apex/bing/zh-CHS/10001/-1) 和 [高级搜索选项](https://help.bing.microsoft.com/apex/index/18/zh-CHS/10002)。

#### GitHub 的高级搜索

可以直接用 [高级搜索页面](https://github.com/search/advanced) 进行搜索，也可以参照 [Github查询语法](https://zhuanlan.zhihu.com/p/273766377) 进行查找，简单说几个:

- `in:name <关键字>` 仓库名称带关键字查询
- `in:description <关键字>` 仓库描述带关键字查询
- `in:readme <关键字>` README 文件带关键字查询
- `stars(fork): >(=) <数字> <关键字>` star 或 fork 数大于(或等于)指定数字的带关键字查询
- `stars(fork): 10..20 <关键词>` star 或 fork 数在 10 到 20 之间的带关键字查询
- `size:>=5000 <关键词>` 限定仓库大于等于 5000K 的带关键字查询
- `pushed(created):>2019-11-15 <关键字>` 更新 或 创建 日期在 2019 年 11 月 16 日之后的带关键字查询
- `license:apache-2.0 <关键字>` LICENSE 为 apache-2.0 的带关键字查询
- `language:java <关键词>` 仓库语言为 Java 的带关键字查询
- `user:<用户名>` 查询某个用户的项目
- `org:<组织名>` 查询某个组织的项目 这些可以混合使用，也可以先查找某一类的 awesome 仓库，然后从 awesome 库里找相关的资源，github 里有很多归纳仓库，可以先看看已有的收集，有时候会节省很多时间

### 更多技巧

使用中，实际上我会去特定网站找一些问题：

- 如果是语言本身相关，比如 c++/Qt/OpenGL 如何实现什么功能，可以直接加上 `site:stackoverflow.com`
- 如果是具体的业务/开发环境或者软件相关，可以先在 BugList 、IssueList ，或者相关论坛里先找一下，比如 Qt 的问题就可以直接去 Qt 论坛，QGis 或者 GDAL 相关问题可以在 stackExchange 里去搜
- QQ 群也是一个提问的地方，但是需要你提的问题有意义，否则大部分人不会回你，而且 QQ 群回复并不及时。
- 知乎专栏、简书、博客园、 CSDN 中有大量中文笔记，这些都是别人嚼烂了的东西，基本是别人踩坑的经验

### 关于百度

大部分编程人都会告诉你别用百度，用 Google 或者 Bing 国际版，但是 Bing 中文搜索的准确率并不高， Google 需要科学上网，如果真的需要，可以使用 Ecosia 、 Yandex 之类的搜索引擎。而且中文搜索来说，百度可能还真是最好的。

百度的问题主要在于排序算法，可能两页都没啥对的内容，但是收录比 Bing 还是好一些的（百度以前并不遵守 robots.txt ，会抓取所有页面，所以有些个人网站甚至专门对百度做了屏蔽），甚至有时候比 Google 好。从数据库来说，百度比 Google 和 Bing 收录的中文内容要多，如果你碰到的时中文相关的问题而且确实找不到相关内容，那么就用百度，搜索引擎是工具，能用好用才是王道。

## 代码搜索

我们除了搜索引擎查找问题，还有可能会搜一些代码，可能是自己写的，也可能是项目中的，下面推荐一些工具：

代码检索有两种，第一是本地的代码检索，第二是要写个啥算法，需要在网上搜索

### 本地代码搜索

- ACK 或者 ACK2，老牌搜索工具，perl 写的
- The Silver Searcher c 实现的
- The Platinum Searcher go 实现的
- FreeCommander 自带的搜索，如果是固态硬盘速度还不错
- IDE 自带的，搜索有些时候并不太好用

### 开源代码搜索

- [Searchcode](https://searchcode.com/) 搜索开源代码，速度比较快
- [一行代码](https://www.alinecode.com/) 国产的，有些国产工具很好用

# 好书推荐

由于版权原因，下面列举的图书中除了开源资源提供了链接，其他的资源请大家自行通过 [libgen](http://libgen.is/) 或 [z-lib](https://zh.singlelogin.re/) 查找。

## 资源汇总

- [Free Programming Books](https://github.com/EbookFoundation/free-programming-books): 开源编程书籍资源汇总
- [CS Textbook Recommendations](https://4chan-science.fandom.com/wiki/Computer_Science_and_Engineering): 计算机科学方向推荐教材列表
- [C Book Guide and List](https://stackoverflow.com/questions/562303/the-definitive-c-book-guide-and-list): C语言相关的编程书籍推荐列表
- [C++ Book Guide and List](https://stackoverflow.com/questions/388242/the-definitive-c-book-guide-and-list): C++语言相关的编程书籍推荐列表
- [Python Book Guide and List](https://pythonbooks.org/): Python语言相关的编程书籍推荐列表
- [Computer Vision Textbook Recommendations](https://www.folio3.ai/blog/best-computer-vision-books/): 计算机视觉方向推荐教材列表
- [Deep Learning Textbook Recommendations](https://www.mostrecommendedbooks.com/lists/best-deep-learning-books): 深度学习方向推荐教材列表

## 系统入门

- Computer Systems: A Programmer's Perspective [[豆瓣](https://book.douban.com/subject/26912767/)]
- Principles of Computer System Design: An Introduction [[豆瓣](https://book.douban.com/subject/3707841/)]

## 操作系统

- [现代操作系统: 原理与实现](https://ipads.se.sjtu.edu.cn/mospi/) [[豆瓣](https://book.douban.com/subject/35208251/)]
- [Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/) [[豆瓣](https://book.douban.com/subject/19973015/)]
- Modern Operating Systems [[豆瓣](https://book.douban.com/subject/27096665/)]
- Operating Systems: Principles and Practice [[豆瓣](https://book.douban.com/subject/25984145/)]

## 计算机网络

- [Computer Networks: A Systems Approach](https://book.systemsapproach.org/foreword.html) [[豆瓣](https://book.douban.com/subject/26417896/)]
- [Computer Networking: A Top-Down Approach](https://www.ucg.ac.me/skladiste/blog_44233/objava_64433/fajlovi/Computer Networking _ A Top Down Approach, 7th, converted.pdf) [[豆瓣](https://book.douban.com/subject/30280001/)]
- How Networks Work [[豆瓣](https://book.douban.com/subject/26941639/)]

## 分布式系统

- [Patterns of Distributed System (Blog)](https://github.com/dreamhead/patterns-of-distributed-systems)
- [Distributed Systems for Fun and Profit (Blog)](http://book.mixu.net/distsys/index.html)
- [Designing Data-Intensive Applications: The Big Ideas Behind Reliable, Scalable, and Maintainable Systems](https://github.com/Vonng/ddia) [[豆瓣](https://book.douban.com/subject/26197294/)]

## 数据库系统

- [Architecture of a Database System](https://dsf.berkeley.edu/papers/fntdb07-architecture.pdf) [[豆瓣](https://book.douban.com/subject/17665384/)]
- [Readings in Database Systems](http://www.redbook.io/) [[豆瓣](https://book.douban.com/subject/2256069/)]
- Database System Concepts : 7th Edition [[豆瓣](https://book.douban.com/subject/30345517/)]

## 编译原理

- Engineering a Compiler [[豆瓣](https://book.douban.com/subject/5288601/)]
- Compilers: Principles, Techniques, and Tools [[豆瓣](https://book.douban.com/subject/1866231/)]
- [Crafting Interpreters](https://craftinginterpreters.com/contents.html)[[豆瓣\]](https://book.douban.com/subject/35548379/)[[开源中文翻译\]](https://github.com/GuoYaxiang/craftinginterpreters_zh)

## 计算机编程语言

- 计算机程序的构造和解释 [[豆瓣](https://book.douban.com/subject/1148282/)]
- [Essentials of Programming Languages](https://eopl3.com/) [[豆瓣](https://book.douban.com/subject/3136252/)]
- [Practical Foundations for Programming Languages](https://www.cs.cmu.edu/~rwh/pfpl.html) [[豆瓣](https://book.douban.com/subject/26782198/)]
- [Software Foundations](https://softwarefoundations.cis.upenn.edu/) [[豆瓣](https://book.douban.com/subject/25712292/)] [[北大相关课程](https://xiongyingfei.github.io/SF/2021/)]
- [Types and Programming Languages](https://www.cis.upenn.edu/~bcpierce/tapl/) [[豆瓣](https://book.douban.com/subject/1761910/)] [[北大相关课程](https://xiongyingfei.github.io/DPPL/2021/main.htm)]

## 体系结构

- 超标量处理器设计: Superscalar RISC Processor Design [[豆瓣](https://book.douban.com/subject/26293546/)]
- Computer Organization and Design RISC-V Edition [[豆瓣](https://book.douban.com/subject/27103952/)]
- Computer Organization and Design: The Hardware/Software Interface [[豆瓣](https://book.douban.com/subject/26604008/)]
- Computer Architecture: A Quantitative Approach [[豆瓣](https://book.douban.com/subject/6795919/)]

## 理论计算机科学

- Introduction to the Theory of Computation [[豆瓣](https://book.douban.com/subject/1852515/)]

## 密码学

- Cryptography Engineering: Design Principles and Practical Applications [[豆瓣](https://book.douban.com/subject/26416592/)]
- Introduction to Modern Cryptography [[豆瓣](https://book.douban.com/subject/2678340/)]

## 逆向工程

- 逆向工程核心原理 [[豆瓣](https://book.douban.com/subject/25866389/)]
- 加密与解密 [[豆瓣](https://book.douban.com/subject/30288807/)]

## 计算机图形学

- [Monte Carlo theory, methods and examples](https://artowen.su.domains/mc/)[[豆瓣](https://book.douban.com/subject/6089923/)]
- Advanced Global Illumination [[豆瓣](https://book.douban.com/subject/2751153/)]
- Fundamentals of Computer Graphics [[豆瓣](https://book.douban.com/subject/26868819/)]
- [Fluid Simulation for Computer Graphics](http://wiki.cgt3d.cn/mediawiki/images/4/43/Fluid_Simulation_for_Computer_Graphics_Second_Edition.pdf) [[豆瓣](https://book.douban.com/subject/2584523/)]
- [Physically Based Rendering: From Theory To Implementation](https://research.quanfita.cn/files/Physically_Based_Rendering_Third_Edition.pdf) [[豆瓣](https://book.douban.com/subject/4306242/)]
- [Real-Time Rendering](https://research.quanfita.cn/files/Real-Time_Rendering_4th_Edition.pdf) [[豆瓣](https://book.douban.com/subject/30296179/)]

## 游戏引擎

- 游戏编程模式: Game Programming Patterns [[豆瓣](https://book.douban.com/subject/26880704/)]
- 实时碰撞检测算法技术 [[豆瓣](https://book.douban.com/subject/4861957/)]
- [Game AI Pro Series](http://www.gameaipro.com/) [[豆瓣](https://search.douban.com/book/subject_search?search_text=Game+AI+Pro&cat=1001)]
- Artificial Intelligence for Games [[豆瓣](https://book.douban.com/subject/3836472/)]
- Game Engine Architecture [[豆瓣](https://book.douban.com/subject/25815142/)]
- Game Programming Gems Series [[豆瓣](https://search.douban.com/book/subject_search?search_text=Game+Programming+Gems&cat=1001)]

## 软件工程

- [Software Engineering at Google](https://abseil.io/resources/swe-book) [[豆瓣](https://book.douban.com/subject/34875994/)]

## 设计模式

- 设计模式: 可复用面向对象软件的基础 [[豆瓣](https://book.douban.com/subject/1052241/)]
- 大话设计模式 [[豆瓣](https://book.douban.com/subject/2334288/)]
- Head First Design Patterns 2nd ed. [[豆瓣](https://book.douban.com/subject/35097022/)]

## 深度学习

- [动手学深度学习](https://zh.d2l.ai/) [[豆瓣](https://book.douban.com/subject/33450010/)]
- [神经网络与深度学习](https://nndl.github.io/) [[豆瓣](https://book.douban.com/subject/35044046/)]
- 深度学习入门 [[豆瓣](https://book.douban.com/subject/30270959/)]
- [简单粗暴 TensorFlow 2 (Tutorial)](https://tf.wiki/)
- [Speech and Language Processing](https://web.stanford.edu/~jurafsky/slp3/) [[豆瓣](https://book.douban.com/subject/5373023/)]

## 计算机视觉

- [Multiple View Geometry in Computer Vision](https://github.com/DeepRobot2020/books/blob/master/Multiple View Geometry in Computer Vision (Second Edition).pdf) [[豆瓣](https://book.douban.com/subject/1841346/)]

## 机器人

- [Probabilistic Robotics](https://docs.ufpr.br/~danielsantos/ProbabilisticRobotics.pdf) [[豆瓣](https://book.douban.com/subject/2861227/)]

## 面试

- 剑指 Offer：名企面试官精讲典型编程题 [[豆瓣](https://book.douban.com/subject/27008702/)]
- Cracking The Coding Interview [[豆瓣](https://book.douban.com/subject/10436668/)]

May 21, 2024

# 数学基础

# MIT Calculus Course

## 课程简介

- 所属大学：MIT
- 先修要求：英语
- 编程语言：无
- 课程难度：🌟🌟
- 预计学时：因人而异

MIT 的微积分课由 MIT18.01: Single Variable Calculus 和 MIT18.02: Multivariable Calculus 两门课组成。对自己数学基础比较自信的同学可以只看课程 notes，写得非常浅显生动并且抓住本质，让你不再疲于做题而是能够真正窥见微积分的本质魅力。

配合油管数学网红 **3Blue1Brown** 的[微积分的本质](https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr)系列视频食用更佳。

## 课程资源

- 课程网站：[18.01](https://ocw.mit.edu/courses/mathematics/18-01sc-single-variable-calculus-fall-2010/syllabus/), [18.02](https://ocw.mit.edu/courses/mathematics/18-02sc-multivariable-calculus-fall-2010/)
- 课程视频：参见课程网站
- 课程教材：参见课程 notes
- 课程作业：书面作业及答案参见课程网站

May 21, 2024

# MIT18.06: Linear Algebra

## 课程简介

- 所属大学：MIT
- 先修要求：英文
- 编程语言：无
- 课程难度：🌟🌟🌟
- 预计学时：因人而异

数学大牛 Gilbert Strang 老先生年逾古稀仍坚持授课，其经典教材 [Introduction to Linear Algebra](https://math.mit.edu/~gs/linearalgebra/) 已被清华采用为官方教材。我当时看完盗版 PDF 之后深感愧疚，含泪花了两百多买了一本英文正版收藏。下面附上此书封面，如果你能完全理解封面图的数学含义，那你对线性代数的理解一定会达到新的高度。

![img](https://cdn.jsdelivr.net/gh/Halerfermatqing/images_bed@main/typora/202406031534095.jpg)

配合油管数学网红 **3Blue1Brown** 的[线性代数的本质](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)系列视频食用更佳。

## 课程资源

- 课程网站：[fall2011](https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/syllabus/)
- 课程视频：参见课程网站
- 课程教材：Introduction to Linear Algebra. Gilbert Strang
- 课程作业：参见课程网站

2023年5月15日，Gilbert Strang 上完了他在 18.06 的[最后一课](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/pages/final-1806-lecture-2023/)，以88岁高龄结束了在其 MIT 61年的教学及科研生涯。但他的线性代数课已经并且还将继续影响一代代青年学子，让我们向老先生致以最崇高的敬意。

May 21, 2024

# MIT6.050J: Information theory and Entropy

## 课程简介

- 所属大学：MIT
- 先修要求：无
- 编程语言：无
- 课程难度：🌟🌟🌟
- 预计学时：100 小时

MIT 面向大一新生的信息论入门课程，Penfield 教授专门为这门课写了一本[教材](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-050j-information-and-entropy-spring-2008/syllabus/MIT6_050JS08_textbook.pdf)作为课程 notes，内容深入浅出，生动有趣。

## 课程资源

- 课程网站：[spring2008](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-050j-information-and-entropy-spring-2008/index.htm)
- 课程教材：[Information and Entropy](https://ocw.mit.edu/courses/6-050j-information-and-entropy-spring-2008/resources/mit6_050js08_textbook/)
- 课程作业：详见课程网站，包含书面作业与 Matlab 编程作业。

May 21, 2024

# 数学进阶

# UCB CS70 : discrete Math and probability theory

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：无
- 编程语言：无
- 课程难度：🌟🌟🌟
- 预计学时：60 小时

伯克利的离散数学入门课程，个人觉得这门课最大的亮点在于并不是单纯的理论知识的讲授，而是在每个模块都会介绍理论知识在实际算法中的运用，让计算机系的学生在夯实理论基础的同时，跳脱出冰冷形式化的数学符号，在实际应用中感受和体会理论的本质。

具体的理论与算法的对应关系列举如下：

- 逻辑证明：稳定匹配算法
- 图论：网络拓扑设计
- 基础数论：RSA 算法
- 多项式环：纠错码设计
- 概率论：哈希表设计、负载均衡等等

课程 notes 也写得非常深入浅出，公式推导与实际例子星罗棋布，阅读体验很好。

## 课程资源

- 课程网站：http://www.eecs70.org/
- 课程教材：参见课程 notes
- 课程作业：参见课程 Schedule

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/UCB-CS70 - GitHub](https://github.com/PKUFlyingPig/UCB-CS70) 中。

May 21, 2024

# UCB CS126 : Probability theory

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS70、微积分、线性代数
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：100 小时

伯克利的概率论进阶课程，涉及到统计学、随机过程等理论相对深入的内容，需要相当的数学基础，我在上这门课的时候也感到有些吃力，不过坚持下来一定会让你对概率论的掌握达到一个新的高度。

同时这门课非常强调理论与实践的结合，课程设计者 Jean Walrand 教授专门写了一本配套的教材[Probability in Electrical Engineering and Computer Science](https://link.springer.com/book/10.1007/978-3-030-49995-2)，书中每个章节都会以一个具体的算法实践作为例子来展示理论在实际当中的运用，例如 PageRank, Route Planing, Speech Recognition 等等，并且全书开源，可以免费下载 PDF 或者 Epub 版。

这还不算完，Jean Walrand 还为整本书里的例子设计了配套的 Python 实现，以 [Jupyter Notebook](https://jeanwalrand.github.io/PeecsJB/intro.html) 的形式在线发布，读者可以在线修改、调试和运行。

与此同时，这门课除了理论作业之外，还有 9 个编程作业，会让你用概率论的知识解决实际问题。

## 课程资源

- 课程网站：https://inst.eecs.berkeley.edu/~ee126/fa20/content.html
- 课程教材：[PDF](https://link.springer.com/content/pdf/10.1007%2F978-3-030-49995-2.pdf), [Epub](https://link.springer.com/download/epub/10.1007%2F978-3-030-49995-2.epub), [Jupyter Notebook](https://jeanwalrand.github.io/PeecsJB/intro.html)
- 课程作业：14 个书面作业 + 9 个编程作业，具体要求参见课程网站。

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/EECS126 - GitHub](https://github.com/PKUFlyingPig/EECS126) 中。

May 21, 2024

# MIT 6.042J: Mathematics for Computer Science

## 课程简介

- 所属大学：MIT
- 先修要求：Calculus, Linear Algebra
- 编程语言：Python preferred
- 课程难度：🌟🌟🌟
- 预计学时：50-70 小时

MIT 的离散数学以及概率综合课程，导师是大名鼎鼎的 **Tom Leighton** ( Akamai 的联合创始人之一)。学完之后对于后续的算法学习大有裨益。

## 课程资源

- 课程网站：[spring2015](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/), [fall2010](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/), [fall2005](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2005/)
- 课程视频：[spring2015](https://www.bilibili.com/video/BV1n64y1i777/?spm_id_from=333.337.search-card.all.click&vd_source=a4d76d1247665a7e7bec15d15fd12349), [fall2010](https://www.bilibili.com/video/BV1L741147VX/?spm_id_from=333.337.search-card.all.click&vd_source=a4d76d1247665a7e7bec15d15fd12349)
- 课程作业：参考课程网站

May 21, 2024

# MIT18.330 : Introduction to numerical analysis

## 课程简介

- 所属大学：MIT
- 先修要求：微积分，线性代数，概率论
- 编程语言：Julia
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

计算机强大的计算能力帮助人们在科学领域不断突破边界，不过计算机的离散本质和这个连续的世界有着天然鸿沟，而如何用离散的表示去估计和逼近那些数学上连续的概念，则是数值分析的重要主题。

这门课会在浮点表示、方程求解、线性代数、微积分、微分方程等领域探讨各类数值分析方法，让你在 Julia 的编程实践中反复体悟（1）如何建立估计（2）如何估计误差（3）如何用算法实现估计 这一系列步骤。

这门课的设计者还编写了配套的开源教材（参见下方链接），里面有丰富的 Julia 实例。

## 课程资源

- 课程网站：https://github.com/mitmath/18330
- 课程教材：https://fncbook.github.io/fnc/frontmatter.html
- 课程作业：10 个 Julia 编程作业

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/MIT18.330 - GitHub](https://github.com/PKUFlyingPig/MIT18.330) 中。

May 21, 2024

# Stanford EE364A: Convex Optimization

## 课程简介

- 所属大学：Stanford
- 先修要求：Python，微积分，线性代数，概率论，数值分析
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

[Stephen Boyd](http://web.stanford.edu/~boyd) 教授是凸优化领域的大牛，其编写的 **Convex Optimization** 这本教材被众多名校采用。另外其研究团队还专门开发了一个用于求解常见凸优化问题的编程框架，支持 Python, Julia 等主流编程语言，其课程作业也是采用这个编程框架去解决实际生活当中的凸优化问题。

在实际运用当中，你会深刻体会到对于同一个问题，建模过程中一个细小的改变，其方程的求解难度会有天壤之别，如何让你建模的方程是“凸”的，是一门艺术。

## 课程资源

- 课程网站：http://stanford.edu/class/ee364a/index.html
- 课程视频：https://www.bilibili.com/video/BV1aD4y1Q7aW
- 课程教材：[Convex Optimization](https://stanford.edu/~boyd/cvxbook/)
- 课程作业：9 个 Python 编程作业

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/Standford_CVX101 - GitHub](https://github.com/PKUFlyingPig/Standford_CVX101) 中。

May 21, 2024

# The Information Theory, Pattern Recognition, and Neural Networks

## 课程简介

- 所属大学：Cambridge
- 先修要求：Calculus, Linear Algebra, Probabilities and Statistics
- 编程语言：Anything would be OK, Python preferred
- 课程难度：🌟🌟🌟
- 预计学时：30-50 小时

剑桥大学 Sir David MacKay 教授的信息论课程。教授是一位十分精通信息论与神经网络的学者，课程对应教材也是信息论领域的一部经典著作。可惜天妒英才...

## 课程资源

- 课程网站：http://www.inference.org.uk/mackay/itila/
- 课程视频：https://www.bilibili.com/video/BV1rs411T71e
- 课程教材：Information Theory, Inference, and Learning Algorithms 在课程网站可以下载到免费的电子版
- 课程作业：在每一节课视频的最后会留教材上的课后习题

## R.I.P Prof. David MacKay

May 21, 2024

# 编程入门

# MIT-Missing-Semester

## 课程简介

- 先修要求：无
- 编程语言：shell
- 课程难度：🌟🌟
- 预计学时：10 小时

正如课程名字所言：“计算机教学中消失的一个学期”，这门课将会教会你许多大学的课堂上不会涉及但却对每个 CSer 无比重要的工具或者知识点。例如 Shell 编程、命令行配置、Git、Vim、`tmux`、`ssh` 等等。如果你是一个计算机小白，那么我非常建议你学习一下这门课，因为它基本涉及了本书必学工具中的绝大部分内容。

除了 MIT 官方的学习资料外，北京大学图灵班开设的前沿计算实践中也开设了相关课程，资料位于[这个网站](http://vcl.pku.edu.cn/course/PFCII/2021-spring/index.html)下，供大家参考。

## 课程资源

- 课程网站：https://missing.csail.mit.edu/2020/
- 课程中文网站: https://missing-semester-cn.github.io/
- 课程视频：https://www.youtube.com/playlist?list=PLyzOVJj3bHQuloKGG59rS43e29ro7I57J
- 课程中文字幕视频：
  - Missing_Semi_中译组（未完结）：https://space.bilibili.com/1010983811?spm_id_from=333.337.search-card.all.click
  - 刘黑黑a（已完结）：https://space.bilibili.com/518734451?spm_id_from=333.337.search-card.all.click
- 课程作业：一些随堂小练习，具体见课程网站。

May 21, 2024

# UCB: Sysadmin DeCal

## 课程简介

- 所属大学：UCB
- 先修要求：无
- 编程语言：shell
- 课程难度：🌟🌟🌟
- 预计学时：20小时

来自 UCB 的一门讲解 Linux 的入门课程，比起定位相同的 MIT 的公开课 Missing Semester，Decal 讲解得更加系统、也更加清晰，这也是我推荐它的主要原因。比起 Missing Semester 更像是给已经开始编程但没有系统使用过这些工具的学生的查缺补漏，DeCal 更像是面向零基础的同学的课程。一共十二周的课程内容，包括 Linux 基础、shell 编程（还有tmux 、vim）、包管理、服务(Services)、基础计算机网络、网络服务、安全(密钥管理)、Git、Docker、Kubernetes、Puppet 和 CUDA。 十分适合新手了解和入门 Linux 环境相关内容。

美中不足的是部分课程作业需要在远程服务器操作，比如关于 ssh 的练习，需要 UCB 内部账号访问。但是大部分作业可以通过自己搭建的虚拟机 + 使用 Xshell 等工具或者直接使用 Linux 桌面版来操作练习，在听完完整课程和做完作业后，相信已经对 Linux 有最基本的了解了。

为弥补无法使用远程服务器的不足以及熟悉 linux 命令行的需求，在此推荐 [bandit](https://overthewire.org/wargames/bandit/) 。bandit 是一款来自OverTheWire 网站的 Wargame，为 CTF 爱好者提供免费的练习靶场。bandit 的前 15 个 level 都是基础的 linux 操作而不涉及任何 CTF 知识。这些练习也正好弥补了 DeCal 外校无法访问的部分（主要是远程链接、文件权限）等内容。

## 课程资源

- 课程网站：[官网](https://decal.ocf.berkeley.edu/)
- 课程视频：原版视频见课程官网，[B站](https://space.bilibili.com/483435468/video)也有搬运。
- 课程教材：无指定教材，但每一周的 labs 之中都有足够的阅读材料供你深入细节。
- 课程作业：见课程官网

May 21, 2024

# Python 语言

# CS61A: Structure and Interpretation of Computer Programs

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：无
- 编程语言：Python, Scheme, SQL
- 课程难度：🌟🌟🌟
- 预计学时：50 小时

伯克利 CS61 系列的第一门课程，也是我的 Python 入门课。

CS61 系列是伯克利 CS 专业的入门课，其中：

- CS61A: 强调抽象，让学生掌握用程序来解决实际问题，而不关注底层的硬件细节。
- CS61B: 注重算法与数据结构以及大规模程序的构建，学生会用 Java 语言结合算法与数据结构的知识来构建千行代码级别的大型项目（一个简易的谷歌地图，一个二维版的 Minecraft）。
- CS61C: 关注计算机体系结构，让学生理解高级语言（例如 C）是如何一步步转换为机器可以理解的 01 串并在 CPU 执行的，学生将会学习 RISC-V 架构并自己用 Logisim 实现一个 CPU。

CS61B 和 CS61C 在本书中均有收录。

回到 CS61A，注意这不仅仅是一门编程语言课，而是会深入到程序构造与运行的原理。最后你将在第 4 个 Project 中用 Python 实现一个 Scheme 的解释器。此外，抽象将是这门课的一大主题，你将学习到函数式编程、数据抽象、面向对象等等知识来让你的代码更易读，更模块化。当然，学习编程语言也是这门课的一大内容，你将会掌握 Python、Scheme 和 SQL 这三种编程语言，在它们的学习和比较中，相信你会拥有快速掌握一门新的编程语言的能力。

注意：如果此前完全没有编程基础，直接上手 CS61A 需要一定的学习能力和自律要求。为避免课程难度过高而导致的信心挫折，可以选择一个更为友好的入门编程课程。例如伯克利的 [CS10](https://cs10.org/sp22/) 或者哈佛大学的 [CS50](https://csdiy.wiki/编程入门/CS50/)。

## 课程资源

- 课程网站: [spring2024](https://inst.eecs.berkeley.edu/~cs61a/sp24), [fall2023](https://inst.eecs.berkeley.edu/~cs61a/fa23/), [spring2023](https://inst.eecs.berkeley.edu/~cs61a/sp23), [fall2022](https://inst.eecs.berkeley.edu/~cs61a/fall22)
- 课程视频: [spring2023](https://www.bilibili.com/video/BV1s3411G7yM/?spm_id_from=333.337.search-card.all.click&vd_source=a4d76d1247665a7e7bec15d15fd12349), [fall2022](https://www.bilibili.com/video/BV1GK411Q7qp/?spm_id_from=333.337.search-card.all.click&vd_source=a4d76d1247665a7e7bec15d15fd12349)
- 课程教材: https://www.composingprograms.com/
- 课程教材中文翻译：https://composingprograms.netlify.app/
- 课程作业: 课程网站会有每个作业对应的文档链接以及代码框架的下载链接。

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CS61A - GitHub](https://github.com/PKUFlyingPig/CS61A) 中。

May 21, 2024

# CS50P Introduction to Programming with Python

## 课程简介

- 所属大学：Harvard University
- 先修要求：无
- 编程语言：Python
- 课程难度：🌟🌟
- 预计学时：30-40 hours

CS50的番外篇，依旧由 David J. Malan 授课。在该课程中你将学会 Python 的基础与进阶语法，以及各种 “Pythonic” 的编程方法。此外对于 Python 特色的代码库、代码测试以及错误处理，该课程也会较为深入地探究。

该课程无需任何编程基础，且相对平易近人。适合所有想要快速入门 Python 语言的各阶段学生。

## 课程资源

- 课程网站：[2022](https://cs50.harvard.edu/python/2022/)
- 课程视频：[2022](https://www.bilibili.com/video/BV1z5411X7wX)
- 课程教材：无
- 课程作业：[2022](https://cs50.harvard.edu/python/2022/)

## 资源汇总

@mancuoj 在学习这门课中用到的所有资源和作业实现都汇总在 [mancuoj/CS50P - GitHub](https://github.com/mancuoj/CS50P) 中。

May 21, 2024

# C 语言

# CS50: This is CS50x

## 课程简介

- 所属大学：Harvard
- 先修要求：无
- 编程语言：C, Python, SQL, HTML, CSS, JavaScript
- 课程难度：🌟🌟
- 预计学时：20 小时

连续多年被哈佛大学学生评为最受欢迎的公选课程。Malan 教授上课非常有激情，撕黄页讲二分法的场面让人记忆犹新（笑）。但因为它的入门以及全校公选的属性，课程内容难度比较温和，但是课程作业质量非常高而且全部免费开源，非常适合小白入门，或者大佬休闲。

## 课程资源

- 课程网站：[2024](https://cs50.harvard.edu/x/2024/), [2023](https://cs50.harvard.edu/x/2023/), [2022](https://cs50.harvard.edu/x/2022/)
- 课程视频：原版参考课程网站，也可以在 B 站找到[中文字幕版](https://www.bilibili.com/video/BV1HW4y1A7Yi/?spm_id_from=333.999.0.0&vd_source=a4d76d1247665a7e7bec15d15fd12349)。
- 课程教材：无
- 课程作业：参考课程网站。

## 资源汇总

@mancuoj 在学习这门课中用到的所有资源和作业实现都汇总在 [mancuoj/CS50x - GitHub](https://github.com/mancuoj/CS50x) 中。

@figuretu 将有价值的提问讨论以及相关学习资源整理在共享文档 [CS50 - 资源总目录](https://uufyjevghz.feishu.cn/docx/DP78d2U5TosTOTx9QCbcjp8GnBh) 中。

May 21, 2024

# Introductory C Programming Specialization

## 课程简介

- 所属大学：Duke
- 先修要求：无
- 编程语言：C
- 课程难度：🌟🌟🌟🌟
- 预计学时：110 小时

非常好的课程，自我感觉收益非常大：

- 侧重基础和基本概念：如 frame、stack memory、heap memory 等讲得很透。
- 针对C最难掌握的指针，有好的练习和编程来加深和强化理解。
- 非常好的 GDB，Valgrind 上手训练，作业也会涉及一些基本的 Git 练习。
- 老师建议作业用 Emacs，所以对 Emacs 小白来说，是个不错的入门。如果你会用 Vim ，我建议你用 Evil 插件。这样你不会丢掉 Vim 的编辑功能，同时可以体会 Emacs 的强大。工具箱里同时有 Emacs 和 Vim 时，效率会有不少提高。Emacs 的 org-mode，和 GDB 的顺滑整合，等等等等，都会让你如虎添翼。
- 虽然可能需要付费，但我觉得值。
- 虽说课名是入门，但兼具广度和深度。

## 课程资源

- 课程网站：https://www.coursera.org/specializations/c-programming
- 课程视频：同上
- 课程教材：同上
- 课程作业：同上

## 资源汇总

@haidongji 在学习这门课中的作业实现都汇总在 [Duke Coursera Intro C](https://code.haidongji.com/Duke_Coursera_Intro_C/) 中。因为时间关系，我最后一课最后一周的几个作业到目前还没有完成。

May 21, 2024

# C++ 语言

# Amirkabir University of Technology 1400-2: Advanced Programming Course

## 课程简介

- 所属大学：Amirkabir University of Technology
- 先修要求：无
- 编程语言：C++
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：50 小时

无意中发现的一个 C++ 课程。课程的 homework 质量很高，每个 homework 相互独立结构简单，且有完善的单元测试，非常适合用来学习 C++ 的编程。本课程共 7 个 homework，如下所示：

1. 实现一个 Matrix 类以及相关函数。
2. 实现一个模拟加密货币客户端/服务端执行过程的程序。
3. 实现一个 Binary Search Tree (BST)。
4. 实现 C++ 中的 SharedPtr 和 UniquePtr 智能指针。
5. 使用继承和多态实现多个类。
6. 使用 STL 库解决 4 个问题。
7. 是个 python 项目，有兴趣的可以看看。

没找到课程的主页，只有在 github 有 homework 的源码（名字为 AP1400-2-HW 的那几个）。

## 课程资源

- 课程网站：无
- 课程代码：https://github.com/courseworks
- 课程教材：无
- 课程作业：7 homework

May 21, 2024

# CS106L: Standard C++ Programming

## 课程简介

- 所属大学：Stanford
- 先修要求：最好掌握至少一门编程语言
- 编程语言：C++
- 课程难度：🌟🌟🌟
- 预计学时：20 小时

我从大一开始一直都是写的 C++ 代码，直到学完这门课我才意识到，我写的 C++ 代码大概只是 C 语言 + `cin`/`cout` 而已。

这门课会深入到很多标准 C++ 的特性和语法，让你编写出高质量的 C++ 代码。例如 auto binding, uniform initialization, lambda function, move semantics，RAII 等技巧都在我此后的代码生涯中被反复用到，非常实用。

值得一提的是，这门课的作业里你会实现一个 HashMap（类似于 STL 中的 `unordered_map`), 这个作业几乎把整个课程串联了起来，非常考验代码能力。特别是 `iterator` 的实现，做完这个作业我开始理解为什么 Linus 对 C/C++ 嗤之以鼻了，因为真的很难写对。

总的来讲这门课并不难，但是信息量很大，需要你在之后的开发实践中反复巩固。Stanford 之所以单开一门 C++ 的编程课，是因为它后续的很多 CS 课程 Project 都是基于 C++的。例如 CS144 计算机网络和 CS143 编译器。这两门课在本书中均有收录。

## 课程资源

- 课程网站：http://web.stanford.edu/class/cs106l/
- 课程视频：https://www.youtube.com/channel/UCSqr6y-eaQT_qZJVUm_4QxQ/playlists
- 课程教材：http://web.stanford.edu/class/cs106l/full_course_reader.pdf
- Assignment1下载网址：https://github.com/snme/cs106L-assignment1
- Assignment2下载网址：https://github.com/snme/cs106L-assignment2
- 课程作业：具体内容见课程网站，我做的时候一共是两个：
- 实现一个 WikiRacer 的小游戏
- 实现一个类似 STL 库的 HashMap

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CS106L - GitHub](https://github.com/PKUFlyingPig/CS106L) 中。

May 21, 2024

# Stanford CS106B/X: Programming Abstractions in C++

## 课程简介

- 所属大学：Stanford
- 先修要求：计算机基础 (CS50/CS106A/CS61A or equivalent)
- 编程语言：C++
- 课程难度：🌟🌟
- 预计学时：50-70 小时

Stanford 的进阶编程课，CS106X 在难度和深度上会比 CS106B 有所提高，但主体内容类似。主要通过 C++ 语言让学生在实际的编程作业里培养通过编程抽象解决实际问题的能力，同时也会涉及一些简单的数据结构和算法的知识，但总体来说没有一门专门的数据结构课那么系统。

## 课程资源

- 课程网站：[CS106B](https://web.stanford.edu/class/cs106b/), [CS106X](https://web.stanford.edu/class/cs106x/)
- 课程教材：https://web.stanford.edu/class/cs106x/res/reader/CS106BX-Reader.pdf
- 课程视频：https://www.bilibili.com/video/BV1G7411k7jG

## 资源汇总

@akun0311 在学习这门课中用到的所有资源和作业实现都汇总在 [akun0311/CS106B-X-CS106L - GitHub](https://github.com/akun0311/CS106B-X-CS106L-) 中。

May 21, 2024

# Java 语言

# MIT 6.092: Introduction To Programming In Java

## 课程简介

- 所属大学：MIT
- 先修要求：无
- 编程语言：Java
- 课程难度：🌟🌟
- 预计学时：少于 15 小时

MIT 的 Java 入门课程，不需要有任何编程基础也可以开始学习。一节课是一小时 Lec （知识点讲解）+一小时 Lab （代码训练），整个课程是七节课。虽说是十四个小时的课时，真正学起来却很快，一天其实差不多就能结束。感觉是比较适合新手上手的强度。

课程内容包括了：

1. 快速入门 Java 所需的基础知识概念，如第一节课的 Java 编译原理、经典代码 "Hello world" 、八大基础类型等。
2. 如何拥有良好的代码风格，如第三节课强调的命名规范、缩进、空格使用等。
3. 如何 Debug ：第六节课的使用 Eclipse warning, Assertion 和第七节课的 Exception 等。

Lab 的 Assignment 倒不是很难，很多前一节课的 Assignment 后一节课 Lec 上就会讲到。唯一需要注意的就是代码是一个很注重实践的技能，新手入门写代码最重要的就是多写多练，无论是 Lec 还是 Lab 上的代码都不要偷懒不写。

学完这门课想要进阶的可以学习 [MIT 6.005/6.031](https://csdiy.wiki/软件工程/6031/) 。

## 课程资源

- 课程网站：[Winter 2010](https://ocw.mit.edu/courses/6-092-introduction-to-programming-in-java-january-iap-2010/pages/syllabus/)
- 课程教材：[How to Think Like a Computer Scientist - 如何像计算机科学家一样思考](https://greenteapress.com/wp/think-java/)
- 课程作业：https://ocw.mit.edu/courses/6-092-introduction-to-programming-in-java-january-iap-2010/pages/assignments/

## 资源汇总

@SinanTang 在学习这门课中用到的所有资源和作业实现都汇总在 [SinanTang/MIT6092-Introduction-to-Programming-in-Java_problem-sets - GitHub](https://github.com/SinanTang/MIT6092-Introduction-to-Programming-in-Java_problem-sets) 中。

@sirrice 在学习这门课中用到的所有资源和作业实现都汇总在 [sirrice/6092 - GitHub](https://github.com/sirrice/6092) 中。

May 21, 2024

# Rust 语言

# CS110L: Safety in Systems Programming

## 课程简介

- 所属大学：Stanford
- 先修要求：最好有一定的编程背景并对计算机系统有初步的认识。
- 编程语言：Rust
- 课程难度：🌟🌟🌟
- 预计学时：30 小时

在这门课中你将会学习 Rust 这门神奇的语言。

如果你学过 C 并接触过一些系统编程的话，应该对 C 的内存泄漏以及指针的危险有所耳闻，但 C 的底层特性以及高效仍然让它在系统级编程中无法被例如 Java 等自带垃圾收集机制的高级语言所替代。而 Rust 的目标则是希望在 C 的高效基础上，弥补其安全不足的缺点。因此 Rust 在设计之初，就有带有很多系统编程的观点。学习 Rust，也能让你之后能用 C 语言编写出更安全更优雅的系统级代码（例如操作系统等）。

这门课的后半部分关注在并发（concurrency）这一主题上，你将会系统地掌握多进程、多线程、基于事件驱动的并发等若干并发技术，并在第二个 Project 中比较它们各自的优劣。Rust 中 “futures” 的概念非常有趣和优雅，这些基础知识对你后续对计算机系统相关课程的学习很有帮助。另外，清华大学的操统实验 rCore 就是基于 Rust 编写的，具体参见[文档](https://rcore-os.github.io/rCore-Tutorial-Book-v3/index.html)。

## 课程资源

- 课程网站：https://reberhardt.com/cs110l/spring-2020/
- 课程视频：https://youtu.be/j7AQrtLevUE
- 课程教材：无
- 课程作业：共 6 个 Lab 和 2 个 Project，作业文档和代码框架详见课程网站。其中两个 Project 非常有趣，分别是：
- 用 Rust 实现一个类似于 GDB 的 debugger
- 用 Rust 实现一个负载均衡器

> [CS 242: Programming Languages, Fall2019](https://stanford-cs242.github.io/f19/) week6 到 week9 关于 Rust 内容的讲解非常细致， 可以作为该课程的讲义补充。 另外， Ryan 在 https://reberhardt.com/cs110l/spring-2021/ 中补充了 2020 版本缺失的关于 Futures Trait 内容的视频。

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CS110L - GitHub](https://github.com/PKUFlyingPig/CS110L) 中。

在2022年 CS110L 没有开源作业源码的背景下，Rust 快速演进导致2020版本课程项目中所使用的库过于老旧。对此，[@fung-hwang](https://github.com/fung-hwang) 尝试进行了适配（时间为2022.11)。其适配过程和作业实现都汇总在 [fung-hwang/CS110L-2020spr - GitHub](https://github.com/fung-hwang/CS110L-2020spr) 中。也许当你开始本课程时 Rust 和这些库又发生了变化，但你仍可以参考并从中获得启发。

May 21, 2024

# CS431: Concurrent Programming

## 课程简介

- 所属大学：KAIST
- 先修要求：Rust 编程基础与对并发的初步了解
- 编程语言：Rust
- 课程难度：🌟🌟🌟🌟
- 预计学时：50 小时

CS431是一门讨论并发编程的课程，主要使用 Rust 语言。课程内容主要包括理论与实践两个部分。理论部分聚焦于建立并发情形下的编程模型，而实践部分则主要是理解 Rust 相关库中锁与无锁数据结构的实现原理。

这门课程同时配有一系列代码量不大但并不简单的作业来巩固你对并发编程的理解，从基于锁的并发安全缓存设计和链表，到无锁的哈希表和著名的 [hazard pointer](https://ieeexplore.ieee.org/document/1291819). 和众多高质量课程一样，这些作业质量较高且配有详细的本地测试，适合自学。

这门课程比我预想的要深入的多，我所知晓的关于自旋锁，互斥锁的知识在该门课程中都是最基础的，而对于 promising semantics, 访存模型和无锁数据结构的介绍让我对并发和 Rust 都有更深入的理解。

## 课程资源

- 课程网站：[Website](https://github.com/kaist-cp/cs431)
- 课程视频：[Youtube](https://www.youtube.com/playlist?list=PL5aMzERQ_OZ9j40DJNlsem2qAGoFbfwb4)
- 课程教材：[Slides](https://docs.google.com/presentation/d/1NMg08N1LUNDPuMxNZ-UMbdH13p8LXgMM3esbWRMowhU/edit?usp=sharing)
- 课程作业：[Homework](https://github.com/kaist-cp/cs431/tree/main/homework)

May 21, 2024

# 函数式语言

# CS3110：OCaml Programming Correct + Efficient + Beautiful

## 课程简介

- 所属大学：Cornell
- 先修要求：了解一门命令式编程语言，类C语言
- 编程语言：OCaml
- 课程难度：🌟🌟🌟
- 预计学时：40 小时

### 课程评价： modern SICP

如果说编程入门的最好的课程是 SICP。在其之后，就是 CS3110。

如果你不知道什么叫函数式编程语言，或者只是听过这个名词，那么这门课程，正如它的名字，会让你体会到什么叫正确，高效和美。

CS3110 不仅局限于函数式编程，更是将理论和实用充分结合。课程内容更进一步，涵盖了 OCaml 语言基础，数据结构和算法，测试开发，形式证明，语言特性实现等诸多内容。而且内容之间并不割裂，而是递进和互补，非常值得学习。

主讲老师 Michael Ryan Clarkson，浸淫编程多年，用词简单，表述清晰，内容环环相扣，剖析一针见血。课程视频甚至用来练听力，听不懂开英文字幕理解起来毫不费力。

### 课程简史，摘自课程教材

CS3110 是康奈尔大学打磨 20 余年的课程。最初发源于 MIT6.001 SICP，在其基础上增加更严格方法和材料，涵盖函数式编程，环境模型，数据结构，算法和语言实现。2008 年，正式名称改为 CS3110，改用 OCaml 语言。2018 年秋季，开始编写[课程教材](https://cs3110.github.io/textbook)。现任课程的主讲老师于 2021 年在 youtube 上公布了[课程视频](https://www.youtube.com/playlist?list=PLre5AT9JnKShBOPeuiD9b-I4XROIJhkIU)。

## 课程资源

- 课程视频油管: https://www.youtube.com/playlist?list=PLre5AT9JnKShBOPeuiD9b-I4XROIJhkIU
- 课程视频B站: https://www.bilibili.com/video/BV1dv4y127Ui/
- 课程教材：https://cs3110.github.io/textbook
- 课程作业：课程教材中 exercises 自选，难度 1 至 4 星，注意 3 星至 4 星的难度跨越很大。

## 资源汇总

@featherwit001 在学习这门课中用到的所有资源和作业实现都汇总在 [featherwit001/CS3110_OCaml_Programming - GitHub](https://github.com/featherwit001/CS3110_OCaml_Programming) 中。

May 21, 2024

# Haskell MOOC

## 课程简介

- 所属大学：University of Helsinki
- 先修要求：无
- 编程语言：Haskell
- 课程难度：🌟🌟
- 预计学时：因人而异

函数式编程正在越来越多的融合入现代编程语言。Java 的 Streams，JavaScript 的 Promises，以及在 ECMAScript 草案阶段的 Record & Tuple。在学习这些内容时，我总是感觉我在死记它们这些 api 的行为，虽然能够使用它们写出一些程序，但总感觉不到掌握了它们。究其原因，它们为什么存在？它们为什么是这样的？设计它们的思想是什么？学完函数式编程会给你答案。

虽然这门课的名字是 Haskell，但它的核心内容是函数式编程思想。就像学习面向对象程序设计，大概率不会选择 Java 之外的语言。

学习 Haskell，但重点不在于使用它。这门课会让你用刚刚够用的 Haskell 语法，刚刚够用的库函数，一丁点的工具，去解释核心的程序语义，也就是函数式编程的核心思想。这不会让你浪费时间陷入语言细节以及语言生态中，我觉得它是这门课的最大优势。

这门课覆盖的内容：

- Pure Function
- Lazy Evaluation
- Strongly Typed
- Type Inferred
- Curry
- Monoid / Functor / Monad / Applicative

如果你有编程经验，课程的 Part1 很简单，难度集中在 Part2 的十三章之后。课程的练习很棒，它有一种在做 [CS61a](https://csdiy.wiki/编程入门/CS61A/) 练习的感觉。练习的注释中有足够的提示，作业在你提交之后会给你标准答案，你还可以在官方的 Telegram 中提问或与他人讨论。

## 课程资源

- 课程网站：https://haskell.mooc.fi/
- 课程视频：无
- 课程教材：https://haskell.mooc.fi/
- 课程作业：https://github.com/moocfi/haskell-mooc
- 社区：https://t.me/haskell_mooc_fi

## 资源汇总

@showtheunli 在学习这门课中用到的所有资源和作业实现都汇总在 [showthesunli/haskell-mooc - GitHub](https://github.com/showthesunli/haskell-mooc) 中。(非常不建议在作业时，参考别人的实现)

May 21, 2024

# 电子基础

# UCB EE16A&B: Designing Information Devices and Systems I&II

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：无
- 编程语言：Python
- 课程难度：🌟🌟🌟
- 预计学时：150 小时

UC Berkeley 电子系学生的大一入门课，通过电路基础知识的讲授，配合各类动手实操的 lab，让学生体验通过电路从环境中收集信息并进行分析，作出预测和反馈。由于疫情的缘故，所有 lab 都有远程在线版，非常适合大家在家自学。

## 课程资源

- 课程网站：[EE16A](https://inst.eecs.berkeley.edu/~ee16a/su20/), [EE16B](https://eecs16b.org/)
- 课程视频：B 站搜索
- 课程教材：参见课程 notes
- 课程作业：参见课程主页

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/EE16A - GitHub](https://github.com/PKUFlyingPig/EE16A) 中。

May 21, 2024

# UCB EE120: Signal and Systems

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS61A, CS70，微积分，线性代数
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：100 小时

这门课最精华的部分就是 6 个超有趣的编程作业了，会让你用 Python 通过学习到的信号与系统的理论知识，解决各类实际问题。例如 lab3 会让你实现 FFT 算法，并和 Numpy 的官方实现进行性能对比；lab4 会通过分析手指头的影像数据推断心率；lab5 就更牛了，会让你给哈勃望远镜拍到的照片进行降噪处理，恢复绚烂清晰的星空；lab6 会让你构造一个反馈系统，平衡小车上的细杆。

## 课程资源

- 课程网站：https://inst.eecs.berkeley.edu/~ee120/fa19/
- 课程教材：参见课程 notes
- 课程作业：5 个书面作业 + 6 个编程作业

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/UCB-EE120 - GitHub](https://github.com/PKUFlyingPig/UCB-EE120) 中。

May 21, 2024

# MIT 6.007 Signals and Systems

## 课程简介

- 所属大学：MIT
- 先修要求：Calculus, Linear Algebra
- 编程语言：Matlab Preferred
- 课程难度：🌟🌟
- 预计学时：50-70 小时

看到课程老师的名字：Prof. Alan V. Oppenheim

好的，上这门课的理由已经足够了。

## 课程资源

- 课程网站：https://ocw.mit.edu/resources/res-6-007-signals-and-systems-spring-2011/index.htm
- 课程视频：https://www.bilibili.com/video/BV1CZ4y1j7hs
- 课程教材：Signals and Systems, 2nd Edition
- 课程作业：https://ocw.mit.edu/resources/res-6-007-signals-and-systems-spring-2011/assignments

May 21, 2024

# 数据结构与算法

# CS61B: Data Structures and Algorithms

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS61A
- 编程语言：Java
- 课程难度：🌟🌟🌟
- 预计学时：60 小时

伯克利 CS61 系列的第二门课程，注重数据结构与算法的设计，同时让学生有机会接触上千行的工程代码，通过 Java 初步领会软件工程的思想。

我上的是 2018 年春季学期的版本，该课的开课老师 Josh Hug 教授慷慨地将 autograder 开源了，大家可以通过网站公开的邀请码在 [gradescope](https://gradescope.com/) 免费加入课程，从而方便地测评自己的代码。

这门课所有的编程作业都是使用 Java 完成的。没有 Java 基础的同学也不用担心，课程会有保姆级的教程，从 IDEA（一款主流的 Java 编程环境）的配置讲起，把 Java 的核心语法与特性事无巨细地讲授，大家完全不用担心跟不上的问题。

这门课的作业质量也是绝绝子。14 个 lab 会让你自己实现课上所讲的绝大部分数据结构，10 个 Homework 会让你运用数据结构和算法解决实际问题， 另外还有 3 个 Project 更是让你有机会接触上千行的工程代码，在实战中磨练自己的 Java 能力。

## 课程资源

- 课程网站：[spring2024](https://sp24.datastructur.es/), [fall2023](https://fa23.datastructur.es/), [spring2023](https://sp23.datastructur.es/), [spring2018](https://sp18.datastructur.es/)
- 课程视频：原版视频参见课程网站，B站有中文翻译搬运。
- 课程教材：无
- 课程作业：每年略有不同，18 年春季学期有 14 个 Lab，10 个 Homework以及 3 个 Project，具体要求详见课程网站。

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CS61B - GitHub](https://github.com/PKUFlyingPig/CS61B) 中。

May 21, 2024

# Coursera: Algorithms I & II

## 课程简介

- 所属大学：Princeton
- 先修要求：CS61A
- 编程语言：Java
- 课程难度：🌟🌟🌟
- 预计学时：60 小时

这是 [Coursera](https://www.coursera.org/) 上评分最高的算法课程。Robert Sedgewick 教授有一种魔力，可以将无论多么复杂的算法讲得极为生动浅显。实不相瞒，困扰我多年的 KMP 以及网络流算法都是在这门课上让我茅塞顿开的，时隔两年我甚至还能写出这两个算法的推导与证明。

你是否觉得算法学了就忘呢？我觉得让你完全掌握一个算法的核心在于理解三点：

- 为什么这么做？（正确性推导，抑或是整个算法的核心本质）
- 如何实现它？（光学不用假把式）
- 用它解决实际问题（学以致用才是真本事）

这门课的构成就非常好地契合了上述三个步骤。观看课程视频并且阅读教授的[开源课本](https://algs4.cs.princeton.edu/home/)有助于你理解算法的本质，让你也可以用非常 生动浅显的话语向别人讲述为什么这个算法得长这个样子。

在理解算法之后，你可以阅读教授对于课程中讲授的所有数据结构与算法的[代码实现](https://algs4.cs.princeton.edu/code/)。 注意，这些实现可不是 demo 性质的，而是工业级的高效实现，从注释到变量命名都非常严谨，模块化也做得相当好，是质量很高的代码。我从这些代码中收获良多。

最后，就是这门课最激动人心的部分了，10 个高质量的 Project，并且全都有实际问题的背景描述，丰富的测试样例，自动的评分系统（代码风格也是评分的一环）。让你在实际生活中 领略算法的魅力。

## 课程资源

- 课程网站：[Algorithm I](https://www.coursera.org/learn/algorithms-part1), [Algorithm II](https://www.coursera.org/learn/algorithms-part2)
- 课程视频：详见课程网站
- 课程教材：https://algs4.cs.princeton.edu/home/
- 课程作业：10个Project，具体要求详见课程网站

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/Princeton-Algorithm - GitHub](https://github.com/PKUFlyingPig/Princeton-Algorithm) 中。

May 21, 2024

# MIT 6.006: Introduction to Algorithms

## 课程简介

- 所属大学：MIT
- 先修要求：计算机导论(CS50/CS61A or equivalent)
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：100h+

MIT-EECS 系的瑰宝。授课老师之一是算法届的奇才 Erik Demaine. 相比较于斯坦福的 [CS106B/X](https://csdiy.wiki/编程入门/cpp/CS106B_CS106X/)（基于 C++ 的数据结构与算法课程），该课程更侧重于算法方面的详细讲解。课程也覆盖了一些经典的数据结构，如 AVL 树等。个人感觉在讲解方面比 CS106B 更加详细，也弥补了 CS106B 在算法方面讲解的不足。适合在 CS106B 入门之后巩固算法知识。

不过该课程也是出了名的难，大家需要做好一定的心理准备。

## 课程资源

- 课程网站：[Fall 2011](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/)
- 课程视频：[Fall 2011](https://www.bilibili.com/video/BV1b7411e7ZP)
- 课程教材：Introduction to Algorithms (CLRS)
- 课程作业：[Fall 2011](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/pages/assignments/)

May 21, 2024

# MIT 6.046: Design and Analysis of Algorithms

## 课程简介

- 所属大学：MIT
- 先修要求：算法入门(6.006/CS61B/CS106B/CS106X or equivalent)
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：100h+

6.006的后续课程。授课老师依旧是 Erik Demaine 和 Srini Devadas，此外还有一位新老师 Nancy Lynch.

相比较于“现学现用”的6.006，6.046更加侧重于如何运用课上所学到的内容举一反三，设计出一套完备的算法并能够证明该算法能解决相应的问题。虽然该课程在板书以及作业中的编程语言为 Python，但基本上没有编程作业；绝大部分的作业都是提出要求，然后需要学生进行算法设计以及合理性证明。所以该课程的难度又提高了一大截:)

在该门课程后还有一门 6.854 高级算法，但对于绝大多数考试以及应聘来说，学完该课程基本上已经能覆盖99%的题目了。

## 课程资源

- 课程网站：[Spring 2015](https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/)
- 课程视频：[Spring 2015](https://www.bilibili.com/video/BV1A7411E737)
- 课程教材：Introduction to Algorithms (CLRS)
- 课程作业：[Spring 2015](https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/pages/assignments/)

May 21, 2024

# CS170: Efficient Algorithms and Intractable Problems

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS61B, CS70
- 编程语言：LaTeX
- 课程难度：🌟🌟🌟
- 预计学时：60 小时

伯克利的算法设计课，更注重算法的理论基础与复杂度分析。课程内容涵盖了分治、图算法、最短路、生成树、贪心、动规、并查集、线性规划、网络流、NP 问题、随机算法、哈希算法等等。

这门课的教材写的很好，证明浅显易懂，非常适合作为工具书查阅。另外，这门课只有书面作业，并且推荐用 LaTeX 编写，大家可以借此机会锻炼自己的 LaTeX 技巧。

## 课程资源

- 课程网站：https://cs170.org/
- 课程视频：https://www.bilibili.com/video/BV1BU4y1b7RK
- 课程教材：详见课程网站 notes
- 课程作业：13 次书面作业，用 LaTeX 编写

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/UCB-CS170 - GitHub](https://github.com/PKUFlyingPig/UCB-CS170) 中。

May 21, 2024

# 软件工程

# MIT 6.031: Software Construction

## 课程简介

- 所属大学：MIT
- 先修要求：掌握至少一门编程语言
- 编程语言：Java
- 课程难度：🌟🌟🌟🌟
- 预计学时：100 小时

这门课的目标就是让学生学会如何写出高质量的代码，所谓高质量，则是满足下面三个目标（课程设计者原话复制，以防自己翻译曲解本意）：

> Safe from bugs. Correctness (correct behavior right now) and defensiveness (correct behavior in the future) are required in any software we build.
>
> Easy to understand. The code has to communicate to future programmers who need to understand it and make changes in it (fixing bugs or adding new features). That future programmer might be you, months or years from now. You’ll be surprised how much you forget if you don’t write it down, and how much it helps your own future self to have a good design.
>
> Ready for change. Software always changes. Some designs make it easy to make changes; others require throwing away and rewriting a lot of code.

为此，这门课的设计者们精心编写了一本书来阐释诸多软件构建的核心原则与前人总结下来的宝贵经验，内容细节到如何编写注释和函数 Specification，如何设计抽象数据结构以及诸多并行编程的内容，并且会让你在精心设计的 Java 编程项目里体验和练习这些编程模式。

2016年春季学期这门课开源了其所有编程作业的代码框架，而最新的课程教材可以在其最新的教学网站上找到，具体链接参见下方。

## 课程资源

- 课程网站：[latest](https://web.mit.edu/6.031/), [Spring 2022](https://web.mit.edu/6.031/www/sp22/), [Spring 2021](https://web.mit.edu/6.031/www/sp21/), [Spring 2016](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-005-software-construction-spring-2016/)
- 课程视频：无
- 课程教材：参见课程网站的课程 notes
- 课程作业：4 个编程作业 + 1 个 Project

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/MIT6.031-software-construction - GitHub](https://github.com/PKUFlyingPig/MIT6.031-software-construction) 中。

@pengzhangzhi 完成了这门课的作业并记录了笔记, 代码开源在 [pengzhangzhi/self-taught-CS/Software Construction - Github](https://github.com/pengzhangzhi/self-taught-CS/tree/main/Software Construction)。

May 21, 2024

# UCB CS169: software engineering

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：无
- 编程语言：Ruby/JavaScript
- 课程难度：🌟🌟🌟🌟
- 预计学时：100 小时

伯克利的软件工程课程，不同于很多传统的软件工程课强调各种类图、文档设计 (plan and document 模式)，这门课专注于最近逐渐流行起来的敏捷开发 (Agile Development)模式，利用云平台提供软件即服务 (software as a service)。为此，课程设计者编写了 [Software as a service](https://github.com/PKUFlyingPig/CS169-Software-Engineering/blob/master/saasbook.pdf) 这本教材，通过 Ruby/Rails 框架来阐释 SaaS 这个概念，并且有丰富的配套编程练习。

这门课在 [Edx](https://www.edx.org/) 这个由 MIT 和 Harvard 大学发起的在线教育平台全资料开源，大家可以在 Edx 自行搜索 *Agile SaaS Development* 这门课程进行学习。课程内容基本按照教材的顺序带你一步步以敏捷开发的方式搭建一个软件并免费部署在云平台上。

## 课程资源

- 课程网站：http://www.saasbook.info/courses
- 课程视频：参见 Edx 课程主页。
- 课程教材：[Software as a service](https://github.com/PKUFlyingPig/CS169-Software-Engineering/blob/master/saasbook.pdf)
- 课程作业：参见 Edx 课程主页。

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CS169-Software-Engineering - GitHub](https://github.com/PKUFlyingPig/CS169-Software-Engineering) 中。

May 21, 2024

# CMU 17-803: Empirical Methods

## 课程简介

- 所属大学：CMU
- 先修要求：面向从事软件工程实证研究的博士生开设，虽然没有硬性先修要求但最好有一定的计算机基础
- 编程语言：不限
- 课程难度：🌟🌟🌟
- 预计学时：100 小时

这门课专注于一个相对“陌生”的领域——包括但不限于软件工程领域的实证研究，由 [Bogdan Vasilescu](https://bvasiles.github.io/) 讲授，他在实证研究和开源软件研究方面非常深入。

这门课是 CMU 为从事该方向研究的博士生开设的，涵盖一系列定性与定量研究方法，如访谈、定性编码、调查设计以及多种数据统计分析方法，帮助学生了解、学习与从事实证研究。课程还会介绍挖掘和整合 GitHub 和 Stack Overflow 等软件存储库中的数据，并运用统计建模、社交网络分析等数据分析技术。

尽管计算机领域在传统上更注重工程技术，但对于工具、技术的设计、评估以及其可能的社会价值来说，实证研究是必需的。例如评估新算法或新技术框架，对某个领域进行相关数据分析，去了解从业者可能面临的挑战。这门课可以扩展和补充专注于技术领域视角。对于想要从事涉及软件工程领域实证研究的科研方向的朋友，这门课可能是一个很好的入门课程。

## 课程资源

- 课程网站：[Spring 2024](https://bvasiles.github.io/empirical-methods/), [Fall 2022](https://bvasiles.github.io/empirical-methods/fall-2022/), [Spring 2021](https://bvasiles.github.io/empirical-methods/spring-2021/), [Fall 2018](https://bvasiles.github.io/empirical-methods/fall-2018/)
- 课程视频：[Spring 2024](https://www.youtube.com/playlist?list=PLuPUOEODcOmsiOxD7LK5EcQcj34Y9NwYg), [Fall 2022](https://www.youtube.com/watch?v=IDtePCle3Qc)
- 课程教材：未公开，每节课前会有阅读材料
- 课程作业：未公开

## 资源汇总

这门课中用到的所有资源都汇总在 [bvasiles/empirical-methods - GitHub](https://github.com/bvasiles/empirical-methods) 中。

May 21, 2024

# CMU CS15213: CSAPP

## 课程简介

- 所属大学：CMU
- 先修要求：CS61A, CS61B
- 编程语言：C
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

CMU 大名鼎鼎的镇系神课，以其内容庞杂，Project 巨难而闻名遐迩。课程内容覆盖了汇编语言、体系结构、操作系统、编译链接、并行、网络等，作为系统入门课，兼具深度和广度，如果自学确实需要相当的毅力和代码功底。

这门课配合的教材由 CMU 计算机系主任 Bryant 教授执笔，也即所谓的 CSAPP。这也是我第一本认认真真一页一页读过去的计算机教材，虽然很难啃，但着实收获良多。

北大购买了这门课的版权并开设了 Introduction to Computer System 这门课，但其实 CSAPP 所有的课程资源和实验代码都能在它的官方主页上访问到（具体参见下方链接）。

这门课由于过于出名，全世界的码农争相学习，导致其 Project 的答案在网上几乎唾手可得。但如果你真的想锻炼自己的代码能力，希望你不要借鉴任何第三方代码。

认真学完这一门课，你对计算机系统的理解绝对会上升一个台阶。

## 课程资源

- 课程网站：http://csapp.cs.cmu.edu/
- 课程视频：https://www.bilibili.com/video/BV1iW411d7hd
- 课程教材：Computer Systems: A Programmer's Perspective, 3/E
- 课程作业：11 个 Project，[代码框架全部开源](http://csapp.cs.cmu.edu/3e/labs.html)

英语有困难的同学可以参考B站UP主[九曲阑干](https://space.bilibili.com/354767108/)对 CSAPP 的[中文讲解](https://www.bilibili.com/video/BV1cD4y1D7uR)（据说CMU的中国留学生也在CMU的课堂上看这个视频呢）。另外如果大家在看完 CSAPP 后对书中的第七章链接有一定的疑问，推荐阅读《程序员的自我修养》这本书，书的副标题是链接，装载与库。这本书能够帮助我们完善对程序链接的理解，相信你在看完这本书以后可以对程序的链接，ELF 文件，动态库都将有一个更加深入的理解。十分推荐在读完 CSAPP，对计算机系统有一定的了解以后作为补充资料来阅读。

有关 Lab 部分，同学们亦可参考 [Arthals](https://arthals.ink/about-me) 在北大计算机系统导论（ICS）课程中所做的详尽笔记：

- [Data Lab](https://arthals.ink/posts/experience/data-lab)
- [Bomb Lab](https://arthals.ink/posts/experience/bomb-lab)
- [Attack Lab](https://arthals.ink/posts/experience/attack-lab)
- [Arch Lab](https://arthals.ink/posts/experience/arch-lab)
- [Cache Lab](https://arthals.ink/posts/experience/cache-lab)
- [Tsh Lab](https://arthals.ink/posts/experience/tsh-lab)
- [Malloc Lab](https://arthals.ink/posts/experience/malloc-lab)
- [Proxy Lab](https://arthals.ink/posts/experience/proxy-lab)

May 21, 2024

# CS110: Principles of Computer Systems

## 课程简介

- 所属大学：Stanford
- 先修要求：编程基础、Unix、GDB、Valgrind
- 编程语言：C/C++
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150小时

这门课程在 [CS107](https://web.stanford.edu/class/archive/cs/cs107/cs107.1246/calendar) 的基础知识上进行拓展，深入研究计算机系统和程序构建。它专注于设计大型系统、跨多台机器的软件以及并行计算。课程的目标是教授学生计算机软件和硬件系统工程的原理和实践。

课程涵盖了广泛的主题，包括你的程序如何映射到计算机系统的组件上，理解程序行为和执行，理解大型系统的设计和权衡，编写跨多台机器的软件，以及编写在单台机器上并行运行任务的软件。

这门课程的教学风格是引人入胜且实用的。教师通过理论知识和丰富的编程实验，引导学生理解计算机系统中众多的技术挑战和设计原则。每周的实验让你为项目增加新功能，这些项目专注于提高学生的实践技能，让你有机会初步了解计算机系统的每一个方面，并且会公布答案，让你及时检查自己对关键知识点的掌握情况。

除了实验外，课程还包括旨在提供大量编程实践经验并加深对课程材料理解的项目作业。每项作业配有完整的测试框架。

## 课程资源

- 课程网站：[winter20](https://web.stanford.edu/class/archive/cs/cs110/cs110.1204/)
- 课程视频：[spring19](https://www.youtube.com/playlist?list=PLai-xIlqf4JmTNR9aPCwIAOySs1GOm8sQ)
- 课程教材：[Computer Systems: A Programmer’s Perspective](https://www.cs.sfu.ca/~ashriram/Courses/CS295/assets/books/CSAPP_2016.pdf)
- 课程作业：7 labs + 8 assignments，参见课程网站。

## 资源汇总

@xuzheng465 在学习这门课中用到的所有资源和作业实现都汇总在 [xuzheng465/Stanford_CS110 - GitHub](https://github.com/xuzheng465/Stanford_CS110) 中。

May 21, 2024

# 体系结构

# Coursera: Nand2Tetris

## 课程简介

- 所属大学：希伯来大学
- 先修要求：无
- 编程语言：任选一个编程语言
- 课程难度：🌟🌟🌟
- 预计学时：40 小时

[Coursera](https://www.coursera.org/) 上被数万人评为满分，在全球四百多所高校、高中被采用，让一个完全没有计算机基础的人从与非门开始造一台计算机，并在上面运行俄罗斯方块小游戏。

听起来就很酷对不对？实现起来更酷！这门课分为硬件和软件两个部分。在硬件部分，你将进入 01 的世界，用与非门构造出逻辑电路，并逐步搭建出一个 CPU 来运行一套课程作者定义的简易汇编代码。在软件部分，你将编写一个编译器，将作者开发的一个名为Jack的高级语言编译为可以运行在虚拟机上的字节码，然后进一步翻译为汇编代码。你还将开发一个简易的 OS，让你的计算机支持输入输出图形界面。至此，你可以用 Jack 开发一个俄罗斯方块的小游戏，将它编译为汇编代码，运行在你用与非门搭建出的 CPU 上，通过你开发的 OS 进行交互。学完这门课程，你将对整个计算机的体系结构有一个全局且深刻的理解，对于你后续课程的学习有着莫大的帮助。

你也许会担心课程会不会很难，但这门课面向的人群是完全没有计算机基础的人，课程作者的目标是让高中生都能理解。因此，只要你按部就班跟着课程规划走，一个月内学完应该绰绰有余。麻雀虽小但是五脏俱全，这门课很好地提取出了计算机的本质，而不过多地陷于现代计算机为了性能而设计出的众多复杂细节。让学习者能在轻松愉快的学习体验中感受计算机的优雅与神奇。

## 课程资源

- 课程网站：[Nand2Tetris I](https://www.coursera.org/learn/build-a-computer/home/week/1), [Nand2Tetris II](https://www.coursera.org/learn/nand2tetris2/home/welcome)
- 课程视频：详见课程网站
- 课程教材：[计算机系统要素：从零开始构建现代计算机](https://github.com/PKUFlyingPig/NandToTetris/blob/master/[计算机系统要素：从零开始构建现代计算机].(尼萨).周维.扫描版.pdf)
- 课程作业：10 个 Project 带你造台计算机，具体要求详见课程网站

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/NandToTetris - GitHub](https://github.com/PKUFlyingPig/NandToTetris) 中。

May 21, 2024

# CS61C: Great Ideas in Computer Architecture

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS61A, CS61B
- 编程语言：C
- 课程难度：🌟🌟🌟🌟
- 预计学时：100 小时

伯克利 CS61 系列的最后一门课程，深入计算机的硬件细节，带领学生逐步理解 C 语言是如何一步步转化为 RISC-V 汇编并在 CPU 上执行的。和 [Nand2Tetris](https://csdiy.wiki/体系结构/N2T/) 不同，这门课 在难度和深度上都会提高很多，具体会涉及到流水线、Cache、虚存以及并发相关的内容。

这门课的 Project 也非常新颖有趣。Project1 会让你用 C 语言写一个小程序，20 年秋季学期是著名的游戏 *Game of Life*。Project2 会让你用 RISC-V 汇编编写一个神经网络，用来 识别 MNIST 手写数字，非常锻炼你对汇编代码的理解和运用。Project3 中你会用 Logisim 这个数字电路模拟软件搭建出一个二级流水线的 CPU，并在上面运行 RISC-V 汇编代码。Project4 会让你使用 OpenMP, SIMD 等方法并行优化矩阵运算，实现一个简易的 Numpy。

总而言之，这是个人上过的最好的计算机体系结构的课程。

## 课程资源

- 课程网站：https://cs61c.org/su20/
- 课程视频：[B 站](https://www.bilibili.com/video/BV1fC4y147iZ), [Youtube](https://www.youtube.com/playlist?list=PLDoI-XvXO0aqgoMQvogzmf7CKiSMSUS3M)
- 课程教材：无
- 课程作业：11 个 Lab，4 个 Project，具体要求详见课程网站

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CS61C-summer20 - GitHub](https://github.com/PKUFlyingPig/CS61C-summer20) 中。

May 21, 2024

# ETH Zurich：Digital Design and Computer Architecture

## 课程简介

- 所属大学：ETH Zurich
- 先修要求：CS50 或同阶课程，最好有 C 语言基础。
- 编程语言：C，Verilog，MIPS 汇编，LC3 汇编
- 课程难度：🌟🌟🌟
- 预计学时：100 小时

体系结构领域的大牛 Onur Mutlu 来教你数字电路和计算机体系结构。课程完全从计算机设计的角度出发，从晶体管、逻辑门开始，一直讲解到微架构、缓存和虚拟内存，还会介绍 很多体系结构领域最新的研究进展。课程共有 9 个 lab，使用 Basys 3 FPGA 开发板（可自行购买）和 Xilinx 公司的 [Vivado 软件](https://china.xilinx.com/products/design-tools/vivado.html)（可在官网免费下载使用）进行电路设计，从组合电路 和时序电路开始，一直到最后部署一个完整的 CPU。课程资料除了 lab 答案和当期考试答案之外全部开源，学完之后你可以掌握计算机相关的数字电路，Verilog 硬件描述语言，MIPS 与 C 之间的转换关系，MIPS 单周期多周期流水线 CPU 的设计和性能分析，缓存，虚拟内存等重要概念。

## 课程资源

- 课程网站：[2020](https://safari.ethz.ch/digitaltechnik/spring2020/),[2023](https://safari.ethz.ch/digitaltechnik/spring2023/)
- 课程视频：[youtube](https://www.youtube.com/playlist?list=PL5Q2soXY2Zi_FRrloMa2fUYWPGiZUBQo2), [B站2020年版本搬运](https://www.bilibili.com/video/BV1MA411s7qq/?vd_source=77d47fcb2bac41ab4ad02f265b3273cf)
- 课程教材1：Patt and Patel, Introduction to Computing Systems
- 课程教材2：Harris and Harris, Digital Design and Computer Architecture (MIPS Edition) 中文译本为《数字设计和计算机体系结构(原书第2版)》
- 课程实验：9 个实验从零开始设计 MIPS CPU，详见课程网站

May 21, 2024

# ETH: Computer Architecture

## 课程简介

- 所属大学：ETH Zurich
- 先修要求：[DDCA](https://csdiy.wiki/体系结构/DDCA/)
- 编程语言：C/C++，verilog
- 课程难度：🌟🌟🌟🌟
- 预计学时：70 小时 +

讲解计算机体系结构，授课教师是 Onur Mutlu 教授。本课程根据课程描述应该是[DDCA](https://csdiy.wiki/体系结构/DDCA/)的进阶课程，课程目标是学习如何为类MIPS处理器设计控制和数据通路硬件，如何通过流水线和简单的超标量执行使机器指令同时执行，以及如何设计快速的内存和存储系统。根据同学反馈，从课程本身的难度上说，至少高于 CS61C ，课程的部分内容十分前沿，B站搬运UP主建议大家作为卡内基梅隆大学18-447的补充。所提供的阅读材料十分丰富，相当于听了一学期讲座。

以下是官网的介绍：

> We will learn the fundamental concepts of the different parts of modern computing systems, as well as the latest major research topics in Industry and Academia. We will extensively cover memory systems (including DRAM and new Non-Volatile Memory technologies, memory controllers, flash memory), new paradigms like processing-in-memory, parallel computing systems (including multicore processors, coherence and consistency, GPUs), heterogeneous computing, interconnection networks, specialized systems for major data-intensive workloads (e.g. graph analytics, bioinformatics, machine learning), etc. We will focus on fundamentals as well as cutting-edge research. Significant attention will be given to real-life examples and tradeoffs, as well as critical analysis of modern computing systems.

编程实践采取 Verilog 设计和模拟类 MIPS 流水线处理器的寄存器传输（RT）实现，以此加强对理论课程的理解。因此前几个实验会有 verilog 的 CPU 流水线编程。同时还将使用C语言开发一个周期精确的处理器模拟器，并使用该模拟器探索处理器设计选项。

## 课程资源

- 课程网站：[2020 Fall](https://safari.ethz.ch/architecture/fall2022/doku.php?id=start), [2022 Fall](https://safari.ethz.ch/architecture/fall2022/doku.php?id=start)
- 课程视频：官方视频详见课程网站。B站有个[2020年版本搬运](https://www.bilibili.com/video/BV1Vf4y1i7YG/?vd_source=77d47fcb2bac41ab4ad02f265b3273cf)。
- 课程教材：无指定教材，每个 lecture 都有大量文献可供阅读
- 课程作业：5 个 Project ，大多与内存和cache相关，具体内容见[课程网站的lab界面](https://safari.ethz.ch/architecture/fall2022/doku.php?id=labs)

## 资源汇总

国内有高校引入了这门课，因此有需要的同学可以搜索到一些资源。

May 21, 2024

# 操作系统

# MIT 6.S081: Operating System Engineering

## 课程简介

- 所属大学：麻省理工学院
- 先修要求：体系结构 + 扎实的 C 语言功底 + RISC-V 汇编语言
- 编程语言：C, RISC-V
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

麻省理工学院大名鼎鼎的 PDOS 实验室开设的面向MIT本科生的操作系统课程。开设这门课的教授之一 —— Robert Morris 教授曾是一位顶尖黑客，世界上第一个蠕虫病毒 Morris 就是出自他之手。

这门课的前身是 MIT 著名的课程 6.828，MIT 的几位教授为了这门课曾专门开发了一个基于 x86 的教学用操作系统 JOS，被众多名校作为自己的操统课程实验。但随着 RISC-V 的横空出世，这几位教授又基于 RISC-V 开发了一个新的教学用操作系统 xv6，并开设了 MIT6.S081 这门课。由于 RISC-V 轻便易学的特点，学生不需要像此前 JOS 一样纠结于众多 x86 “特有的”为了兼容而遗留下来的复杂机制，而可以专注于操作系统层面的开发。

这几位教授还专门写了一本[教程](https://pdos.csail.mit.edu/6.828/2021/xv6/book-riscv-rev2.pdf)，详细讲解了 xv6 的设计思想和实现细节。

这门课的讲授也很有意思，老师会带着学生依照 xv6 的源代码去理解操作系统的众多机制和设计细节，而不是停留于理论知识。每周都会有一个 lab，让你在 xv6 上增加一些新的机制和特性，非常注重学生动手能力的培养。整个学期一共有 11 个 lab，让你全方位地深刻理解操作系统的每个部分，非常有成就感。而且所有的lab都有着非常完善的测试框架，有的测试代码甚至上千行，让人不得不佩服 MIT 的几位教授为了教好这门课所付出的心血。

这门课的后半程会讲授操作系统领域的多篇经典论文，涉及文件系统、系统安全、网络、虚拟化等等多个主题，让你有机会接触到学界最前沿的研究方向。

## 课程资源

- 课程网站：https://pdos.csail.mit.edu/6.828/2021/schedule.html
- 课程视频：https://www.youtube.com/watch?v=L6YqHxYHa7A，每节课的链接详见课程网站
- 课程视频翻译文档：https://mit-public-courses-cn-translatio.gitbook.io/mit6-s081/
- 课程教材：https://pdos.csail.mit.edu/6.828/2021/xv6/book-riscv-rev2.pdf
- 课程作业：https://pdos.csail.mit.edu/6.828/2021/schedule.html，11个lab，具体要求详见课程网站

## xv6 补充资源

- [xv6 操作系统的深入讲解](https://space.bilibili.com/1040264970/)
- [xv6 中文文档](https://th0ar.gitbooks.io/xv6-chinese/content/index.html)
- [xv6 关键源码逐行解读 + 整体架构分析](https://www.youtube.com/playlist?list=PLbtzT1TYeoMhTPzyTZboW_j7TPAnjv9XB)
- [课程教材翻译 xv6-riscv-book-zh-cn](https://blog.betteryuan.top/archives/xv6-riscv-book-zh-cn)
- [课程教材翻译源码 xv6-riscv-book-zh-cn](https://github.com/HelloYJohn/xv6-riscv-book-zh-cn.git)

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/MIT6.S081-2020fall - GitHub](https://github.com/PKUFlyingPig/MIT6.S081-2020fall) 中。

@[KuangjuX](https://github.com/KuangjuX) 编写了 MIT 6.S081 的 lab 的[题解](https://github.com/KuangjuX/xv6-riscv-solution)，里面有详细的解法和补充知识。另外，@[KuangjuX](https://github.com/KuangjuX) 还使用 Rust 语言重新实现了 xv6-riscv 操作系统：[xv6-rust](https://github.com/Ko-oK-OS/xv6-rust)，里面对于 xv6-riscv 有更为详细的思考和讨论，感兴趣的同学可以看一下哦。

### 一些可以参考的博客

- [doraemonzzz](http://doraemonzzz.com/tags/6-S081/)
- [Xiao Fan (樊潇)](https://fanxiao.tech/posts/2021-03-02-mit-6s081-notes/)
- [Miigon&#39;s blog](https://blog.miigon.net/categories/mit6-s081/)
- [Zhou Fang](https://walkerzf.github.io/categories/6-S081/index.html)
- [Yichun's Blog](https://www.yichuny.page/tags/Operating System)
- [解析Ta](https://blog.csdn.net/u013577996/article/details/108679997)
- [PKUFlyingPig](https://github.com/PKUFlyingPig/MIT6.S081-2020fall)
- [星遥见](https://www.cnblogs.com/weijunji/tag/XV6/)
- [tzyt 的博客](https://ttzytt.com/tags/xv6/)

May 21, 2024

# CS162: Operating System

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS61A, CS61B, CS61C
- 编程语言：C, x86汇编
- 课程难度：🌟🌟🌟🌟🌟🌟
- 预计学时：200 小时+，上不封顶

这门课让我记忆犹新的有两个部分：

首先是教材，这本书用的教材 *Operating Systems: Principles and Practice (2nd Edition)* 一共四卷，写得非常深入浅出，很好地弥补了 MIT6.S081 在理论知识上的些许空白，非常建议大家阅读。相关资源会分享在本书的经典书籍推荐模块。

其次是这门课的 Project —— Pintos。Pintos 是由 Ben Pfaff 等人在 x86 平台上编写的教学用操作系统，Ben Pfaff 甚至专门发了篇 [paper](https://benpfaff.org/papers/pintos.pdf) 来阐述 Pintos 的设计思想。

和 MIT 的 xv6 小而精的 lab 设计理念不同，Pintos 更注重系统的 Design and Implementation。Pintos 本身仅一万行左右，只提供了操作系统最基本的功能。而 4 个Project，就是让你在这个极为精简的操作系统之上，分别为其增加线程调度机制 (Project1)，系统调用 (Project2)，虚拟内存 (Project3) 以及文件系统 (Project4)。所有的 Project 都给学生留有很大的设计空间，总代码量在 2000 行左右。根据 Stanford 学生[自己的反馈](https://www.quora.com/What-is-it-like-to-take-CS-140-Operating-Systems-at-Stanford)，在 3-4 人组队的情况下，后两个 Project 的人均耗时也在 40 个小时以上。

虽然难度很大，但 Stanford, Berkeley, JHU 等多所美国顶尖名校的操统课程均采用了 Pintos。如果你真的对操作系统很感兴趣，Pintos 会极大地提高你编写和 debug 底层系统代码的能力。在本科阶段，能自己设计、实现并 debug 一个大型系统，是一段非常珍贵的经历。

北大 2022 年春季学期的操作系统实验班也将会首次引入 Pintos 作为课程 Project。我和该课程的[另一位助教](https://github.com/AlfredThiel)整理并完善了 Pintos 的[实验文档](https://pkuflyingpig.gitbook.io/pintos)，并利用 Docker 配置了跨平台的实验环境，想自学的同学可以按文档自行学习。在毕业前的最后一个学期，希望能用这样的尝试，让更多人爱上系统领域，为国内的系统研究添砖加瓦。

## 课程资源

- 课程网站：https://cs162.org/
- 课程视频：https://www.youtube.com/watch?v=YfHY0pvpRkk，每节课的链接参见课程网站
- 课程教材：[Operating Systems: Principles and Practice (2nd Edition)](http://ospp.cs.washington.edu/)
- 课程作业：https://cs162.org/，6 个 Homework, 3 个 Project，具体要求参见课程网站

## 资源汇总

由于北大的操统实验班采用了该课程的 Project，为了防止代码抄袭，我的代码实现没有开源。

May 21, 2024

# NJU OS: Operating System Design and Implementation

## 课程简介

- 所属大学：南京大学
- 先修要求：体系结构 + 扎实的 C 语言功底
- 编程语言：C 语言
- 课程难度：🌟🌟🌟🌟
- 预计学时：150 小时

之前一直听说南大的蒋炎岩老师开设的操作系统课程讲得很好，久闻不如一见，这学期有幸在 B 站观看了蒋老师的课程视频，确实收获良多。蒋老师作为非常年轻的老师，有着丰富的一线代码的经验，因此课程讲授有着满满的 Hacker 风格，课上经常“一言不合”就在命令行里开始写代码，很多重要知识点也都配有生动直白的代码示例。让我印象最为深刻的就是老师为了让学生更好地理解动态链接库的设计思想，甚至专门实现了一个迷你的可执行文件与一系列的二进制工具，让很多困扰我多年的问题都得到了解答。

这门课的讲授思路也非常有趣，蒋老师先从“程序就是状态机”这一视角入手，为“万恶之源”并发程序建立了状态机的转化模型，并在此基础上讲授了并发控制的常见手段以及并发 bug 的应对方法。接着蒋老师将操作系统看作一系列对象（进程/线程、地址空间、文件、设备等等）以及操作它们的 API （系统调用）并结合丰富的实际例子介绍了操作系统是如何利用这系列对象虚拟化硬件资源并给应用软件提供各类服务的。最后的可持久化部分，蒋老师从 1-bit 的存储介质讲起，一步步构建起各类存储设备，并通过设备驱动抽象出一组接口来方便地设计与实现文件系统。我之前虽然上过许多门操作系统的课程，但这种讲法确实独此一家，让我收获了很多独到的视角来看待系统软件。

这门课除了在理论知识的讲授部分很有新意外，注重实践也是蒋老师的一大特点。在课堂和编程作业里，蒋老师会有意无意地培养大家阅读源码、查阅手册的能力，这也是计算机从业者必备的技能。在完成第五个 MiniLab 期间，我第一次仔仔细细阅读了微软的 FAT 文件系统手册，收获了一次非常有价值的经历。

编程作业共由 5个 MiniLab 和 4个 OSLab 组成。美中不足的是作业的评测机是不对校外开放的，不过在邮件“骚扰”后蒋老师还是非常慷慨地让我成功蹭课。由于课余时间有限我只完成了 5个 MiniLab，总体体验非常棒。尤其是第二个协程实验让我印象最为深刻，在不到百行的小实验里深刻体验了上下文切换的美妙与“可怕”。另外其实几个 MiniLab 都能非常方便地进行本地测试，就算没有评测机也不影响自学，因此希望大家不要聚众“骚扰”老师以图蹭课。

最后再次感谢蒋老师设计并开放了这样一门非常棒的操作系统课程，这也是本书收录的第一门国内高校自主开设的计算机课程。正是有蒋老师这些年轻的新生代教师在繁重的 Tenure 考核之余的用爱发电，才让无数学子收获了难忘的本科生涯。也期待国内能有更多这样的良心好课，我也会第一时间收录进本书中让更多人受益。

## 课程资源

- 课程网站：https://jyywiki.cn/OS/2022/index.html
- 课程视频：https://space.bilibili.com/202224425/channel/collectiondetail?sid=192498
- 课程教材：http://pages.cs.wisc.edu/~remzi/OSTEP/
- 课程作业：https://jyywiki.cn/OS/2022/index.html

## 资源汇总

按蒋老师的要求，我的作业实现没有开源。

May 21, 2024

# HIT OS: Operating System

## 课程简介

- 所属大学：哈尔滨工业大学
- 先修要求：C 语言
- 编程语言：C 语言、汇编
- 课程难度：🌟🌟🌟🌟
- 预计学时：100 小时+

如果你在知乎上搜索“操作系统如何自学”、“操作系统的公开课推荐”、“有哪些让你相见恨晚的计算机课程”等问题，哈工大李治军老师的操作系统课程大概率都会在某条高赞回答的推荐里。这是一门知名度较高、颇受欢迎的中文计算机课程。

这门课善于站在学生角度循循善诱。例如，课程从“弱弱地问，什么是操作系统”来“揭开操作系统钢琴的盖子”，从 CPU 的直观管理引出进程概念，从“那就首先让程序进入内存”引出内存管理。

这门课注重理论和实践相结合。操作系统是看得见摸得着的东西，李老师反复强调一定要做实验，如果只看视频纸上谈兵，是学不好操作系统的。课程基于实际的 Linux 0.11 源码（总代码量约两万行）进行讲解和实验，共有八个小实验，四个大实验。

当然，这门课也有一些瑕不掩瑜的地方。例如，Linux 0.11 是很早期工业界的代码，不是为了教学而设计的。因此在实验过程中会有一些避不开的晦涩难懂的原生代码，但它们对理解操作系统其实并没有太大帮助。

## 课程资源

- 课程网站：https://www.icourse163.org/course/HIT-1002531008
- 课程视频：https://www.bilibili.com/video/BV19r4y1b7Aw/?p=1
- 课程教材一：[《Linux 内核完全注释》](https://book.douban.com/subject/1231236//)
- 课程教材二：[《操作系统原理、实现与实践》](https://book.douban.com/subject/30391722/)
- 课程作业：https://www.lanqiao.cn/courses/115

## 资源汇总

@NaChen95 在学习这门课中的八个实验作业的原理分析和实现都汇总在 [NaChen95 / Linux0.11](https://github.com/NaChen95/Linux0.11) 中。

May 21, 2024

# 并行与分布式系统

# CMU 15-418/Stanford CS149: Parallel Computing

## 课程简介

- 所属大学：CMU 和 Stanford
- 先修要求：计算机体系结构，熟悉 C++
- 编程语言：C++
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

[Kayvon Fatahalian](http://www.cs.cmu.edu/~kayvonf) 教授此前在 CMU 开了 15-418 这门课，后来他成为 Stanford 的助理教授后又开了类似的课程 CS149。但总体来说，15-418 包含的课程内容更丰富，并且有课程回放，但 CS149 的编程作业更 fashion 一些。我个人是观看的 15-418 的课程录影但完成的 CS149 的作业。

这门课会带你深入理解现代并行计算架构的设计原则与必要权衡，并学会如何充分利用硬件资源以及软件编程框架（例如 CUDA，MPI，OpenMP 等）编写高性能的并行程序。由于并行计算架构的复杂性，这门课会涉及诸多高级体系结构与网络通信的内容，知识点相当底层且硬核。与此同时，5 个编程作业则是从软件的层面培养学生对上层抽象的理解与运用，具体会让你分析并行程序的瓶颈、编写多线程同步代码、学习 CUDA 编程、OpenMP 编程以及前段时间大热的 Spark 框架等等。真正意义上将理论与实践完美地结合在了一起。

## 课程资源

- 课程网站：[CMU15418](http://15418.courses.cs.cmu.edu/spring2016/), [CS149](https://gfxcourses.stanford.edu/cs149/fall21)
- 课程视频：http://15418.courses.cs.cmu.edu/spring2016/lectures
- 课程教材：无
- 课程作业：https://gfxcourses.stanford.edu/cs149/fall21，5 个编程作业

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CS149-parallel-computing - GitHub](https://github.com/PKUFlyingPig/CS149-parallel-computing) 中。

May 21, 2024

# MIT6.824: Distributed System

## 课程简介

- 所属大学：MIT
- 先修要求：计算机体系结构，并行编程
- 编程语言：Go
- 课程难度：🌟🌟🌟🌟🌟🌟
- 预计学时：200 小时

这门课和 MIT 6.S081 一样，出品自 MIT 大名鼎鼎的 PDOS 实验室，授课老师 Robert Morris 教授曾是一位顶尖黑客，世界上第一个蠕虫病毒 Morris 病毒就是出自他之手。

这门课每节课都会精读一篇分布式系统领域的经典论文，并由此传授分布式系统设计与实现的重要原则和关键技术。同时其课程 Project 也是以其难度之大而闻名遐迩，4 个编程作业循序渐进带你实现一个基于 Raft 共识算法的 KV-store 框架，让你在痛苦的 debug 中体会并行与分布式带来的随机性和复杂性。

同样，这门课由于太过出名，网上答案无数，希望大家不要参考，而是力图自主实现整个 Project。

## 课程资源

- 课程网站：https://pdos.csail.mit.edu/6.824/schedule.html
- 课程视频：参见课程网站链接
- 课程视频中文翻译：https://mit-public-courses-cn-translatio.gitbook.io/mit6-824/
- 课程教材：无，以阅读论文为主
- 课程作业：4 个非常虐的 Project，具体要求参见课程网站

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/MIT6.824 - GitHub](https://github.com/PKUFlyingPig/MIT6.824) 中。

@[OneSizeFitsQuorum](https://github.com/OneSizeFitsQuorum) 的 [Lab 文档](https://github.com/OneSizeFitsQuorum/MIT6.824-2021) 较为清晰地介绍了实现 lab 1-4 和 challenge 1-2 时需要考虑的许多细节，在遇到瓶颈期时可以阅读一下~~

May 21, 2024

# 计算机系统安全

# UCB CS161: Computer Security

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS61A, CS61B, CS61C
- 编程语言：C, Go
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

伯克利的计算机系统安全课程，课程内容分为5个部分：

- Security principles: how to design a secure system
- Memory safety: buffer overflow attack
- Cryptography: symmetric encryption, asymmetric encryption, MAC, digital signature .........
- Web: SQL-injection, XSS, XSRF .......
- Networking: attacks for each layer

这门课让我印象最为深刻的部分是 Project2，让你用 Go 语言设计和实现一个安全的文件分享系统。我花了整整三天才完成了这个非常虐的 Project，总代码量超过 3k 行。这样密集型的开发过程，能极大地锻炼你设计和实现一个安全系统的能力。

2020 年夏季学期的版本开源了课程录影，大家可以在下面的课程网站链接里找到。

## 课程资源

- 课程网站：https://su20.cs161.org/
- 课程视频：参见课程网站
- 课程教材：https://textbook.cs161.org/
- 课程作业：7 个在线 HW + 3 个 Lab + 3 个 Project

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/UCB-CS161 - GitHub](https://github.com/PKUFlyingPig/UCB-CS161) 中。

May 21, 2024

# MIT6.1600: Foundations of Computer Security

## 课程简介

- 所属大学：MIT
- 先修要求：离散数学，编程基础，计算机系统基础
- 编程语言：Python3
- 课程难度：🌟🌟🌟
- 预计学时：50小时

MIT 的计算机系统安全本科生课程，共分为 authentication, transport security, platform security, software security, 和 human/end-user security 五个模块。课程组织还是相当清晰的：authentication 关注于认证安全，即如何证明计算机世界的“你”确实是“你”。接着讲解大家了解较多的通信安全，例如数据传输的加密解密，密钥的交换等。但传输是一方面，代码最终需要在终端上执行，这就涉及到运行代码的平台本身甚至软件代码本身的安全性。最后课程还会讲一些关于隐私安全的内容，上升到社会学的范畴去讨论群体信息安全。学完该课程，你将会掌握计算机安全的很多重要基本概念，例如公钥私钥加密算法、哈希算法、电子签名、密钥交换算法等等。除了稍显复杂枯燥的数学和定理证明外，课程中还会结合具体知识点讲解很多现实发生的安全漏洞，让你对这些安全概念有更感性的认识。此外，还有6个课程实验让你通过编程实现很多漏洞的利用，在实际中加深对知识的理解，个人感觉还是很有意思的。

## 课程资源

- 课程网站：[fall23](https://61600.csail.mit.edu/2023/), [fall22](https://61600.csail.mit.edu/2022/)
- 课程视频：参见课程网站
- 课程教材：没有指定教材，每节课有 notes
- 课程作业：一共6个实验，难度适中

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/MIT6.1600 - GitHub](https://github.com/PKUFlyingPig/MIT6.1600) 中。

May 21, 2024

# MIT 6.858: Computer System Security

## 课程简介

- 所属大学：MIT
- 先修要求：计算机体系结构，对计算机系统有初步了解
- 编程语言：C, Python
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

MIT 的计算机系统安全课程，实验环境是一个 Web Application Zoobar。学生学习攻防技术并应用于该 Web Application。

- Lab 1: you will explore the zoobar web application, and use buffer overflow attacks to break its security properties.
- Lab 2: you will improve the zoobar web application by using privilege separation, so that if one component is compromised, the adversary doesn't get control over the whole web application.
- Lab 3: you will build a program analysis tool based on symbolic execution to find bugs in Python code such as the zoobar web application.
- Lab 4: you will improve the zoobar application against browser attacks.

这个课我主要是做了 Lab 3。Lab 3 是通过混合符号执行来遍历程序的所有分支，理解了符号执行的思想后 Lab 并不难做。这个 Lab 直观展示符号执行这种技术的使用方法。

这个课的 Final Project 是实现 [SecFS](https://github.com/mit-pdos/secfs-skeleton)，一个远端文件系统，面对完全不可信的服务器，提供机密性和完整性。参考论文为 [SUNDR](https://www.usenix.org/legacy/event/osdi04/tech/full_papers/li_j/li_j.pdf)。

## 课程资源

- 课程网站：http://css.csail.mit.edu/6.858/2022/
- 课程视频：参见课程网站
- 课程教材：无
- 课程作业：4 个 Lab + Final Project / Lab5

May 21, 2024

# ASU CSE365: Introduction to Cybersecurity

## 课程简介

- 所属大学：Arizona State University
- 先修要求：无
- 编程语言：C, Python, x86 assembly
- 课程难度：🌟🌟🌟🌟
- 预计学时：因人而异

亚利桑那州立大学 Web 安全的导论课，课程以模块化的形式构成，主要包含以下方面：

- Program Misuse: Linux commandline, privilege escalation
- Web fundamentals: http, server, intercept
- Assembly: registers, memory, control flow
- Cryptography: Symmetric/Asymmetric encryption, hashing, trust
- Web security: Command/HTML/SQL/Stack injection

课程以 Challenge 为主，Lectures and Reading 为辅。Challenge 中的习题以 CTF 的形式展开，难度依次递增。

对于基础较弱的学习者，卡关是正常现象。如果在解题过程中遇到困难，可以在首页 Chat 栏目中给出的 Discord Server 寻求帮助。

## 课程资源

- 课程网站：https://dojo.pwn.college/cse365/
- 课程视频：参见课程网站
- 课程教材：无
- 课程作业：7 个模块（167 个 challenge）

## 资源汇总

- Lectures on YouTube: https://youtube.com/pwncollege
- Live Broadcasts on Twitch: https://twitch.tv/pwncollege
- Chat on Discord: https://pwn.college/discord
- Open Source on GitHub: https://github.com/pwncollege
- Contact us via Email: [pwn-college@asu.edu](mailto:pwn-college@asu.edu)

另外，出于评定 ASU 学生课程成绩的重要因素，官方不鼓励上传解题思路，每个模块的前两题除外。

May 21, 2024

# ASU CSE466: Computer Systems Security

## 课程简介

- 所属大学：Arizona State University
- 先修要求：无
- 编程语言：C, Python, x86 assembly
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：因人而异

亚利桑那州立大学系统安全的核心课，课程以模块化的形式构成，主要包含以下方面：

- Linux commandline: Program misuse, program interaction
- Shellcoding: Assembly, shellcode injection, prevention
- Reverse Engineering: Function frame, static/dynamic reversing tools
- Program Exploitation: Hijacking to shellcode, JIT spray
- System Exploitation: Kernel modules, privilege escalation
- Miscellaneous: Sandboxing, Memory Errors, Race conditions

与 CSE365 相同，课程以 Challenge 为主，Lectures and Reading 为辅。Challenge 中的习题以 CTF 的形式展开，难度依次递增。

习题质量挺高的，但某些模块难度较大，尤其是涉及到内核的部分，有的时候一天都写不出一道题。如果在解题过程中遇到困难，可以在首页 Chat 栏目中给出的 Discord Server 寻求帮助。

## 课程资源

- 课程网站：https://dojo.pwn.college/cse466/
- 课程视频：参见课程网站
- 课程教材：无
- 课程作业：13 个模块（358 个 challenge）

## 资源汇总

- Lectures on YouTube: https://youtube.com/pwncollege
- Live Broadcasts on Twitch: https://twitch.tv/pwncollege
- Chat on Discord: https://pwn.college/discord
- Open Source on GitHub: https://github.com/pwncollege
- Contact us via Email: [pwn-college@asu.edu](mailto:pwn-college@asu.edu)

另外，出于评定 ASU 学生课程成绩的重要因素，官方不鼓励上传解题思路，每个模块的前两题与逆向部分的 16 题除外。

May 21, 2024

# SEEDLabs

## 课程简介

- 所属大学：雪城大学
- 先修要求：无
- 编程语言：C，汇编
- 课程难度：🌟🌟🌟🌟
- 预计学时：150 小时

雪城大学的网安课程，由 NSF 提供130万美元的资金支持，为网安教育开发了动手实践性的实验练习（称为 SEED Lab）。课程理论教学和动手实践并重，包含详细的 [开源讲义](https://github.com/seed-labs/seed-labs) 、视频教程、教科书（被印刷为多种语言）、开箱即用的基于虚拟机和 docker 的攻防环境等。目前全球有1050家研究机构在使用该项目。

涵盖计算机和信息安全领域的广泛主题，包括软件安全、网络安全、Web 安全、操作系统安全和移动应用安全。

## 课程资源

- 课程网站：https://seedsecuritylabs.org/index.html
- 课程视频：https://www.handsonsecurity.net/video.html
- 课程教材：https://www.handsonsecurity.net/index.html
- 课程作业：四十多个安全领域的lab，实验环境可由课程提供的定制虚拟机和 docker [快速搭建](https://seedsecuritylabs.org/labsetup.html)，并且提供详细的原理讲解、实验指导。以 [缓冲区溢出实验](https://seedsecuritylabs.org/Labs_20.04/Software/Buffer_Overflow_Setuid/) 为例，该实验属于 [软件安全主题](https://seedsecuritylabs.org/Labs_20.04/Software/) ，这里是它的 [实验指导](https://seedsecuritylabs.org/Labs_20.04/Files/Buffer_Overflow_Setuid/Buffer_Overflow_Setuid.pdf) ，这里是它对应的 [教材内容](https://www.handsonsecurity.net/files/chapters/buffer_overflow_c.pdf)

## 资源汇总

@LaPhilosophie 在学习这门课中用到的所有资源和作业实现都汇总在 [LaPhilosophie/seedlab - GitHub](https://github.com/LaPhilosophie/seedlab) 中。

May 21, 2024

# 计算机网络

# USTC Computer Networking:A Top-Down Approach

## 课程简介

- 所属大学：中国科学技术大学
- 授课教师：郑烇、杨坚
- 先修要求：操作系统（非必需）
- 编程语言：无
- 课程难度：🌟🌟🌟
- 预计学时：40 小时

这门课应该是中文互联网上比较火的计算机网络课了，教材采用神书计算机网络（自顶向下方法），授课风格更偏向实际而非纯理论（**强烈建议**先阅读教材预习再看课，否则上课时*可能*会有些懵圈）。

课程内容包括**大部分**自顶向下方法里的内容，同时**涵盖**考试内容，可放心观看。

课程视频是郑烇老师本人在哔哩哔哩上上传的，且从2020年至今一直坚持在评论区答疑，属实负责且认真。

## 课程资源

- 课程网站：http://staff.ustc.edu.cn/~qzheng/teaching.html
- 课程视频：https://www.bilibili.com/video/BV1JV411t7ow/
- 课程课件：http://staff.ustc.edu.cn/~qzheng/cn.zip
- 课程教材：计算机网络（自顶向下方法 第7版），机械工业出版社，2016

May 21, 2024

# Computer Networking: A Top-Down Approach

## 课程简介

- 所属大学：马萨诸塞大学
- 先修要求：有一定的计算机系统基础
- 编程语言：无
- 课程难度：🌟🌟🌟
- 预计学时：40 小时

《自顶向下方法》是计算机网络领域的一本经典教材，两位作者 Jim Kurose 和 Keith Ross 精心制作了教材配套的课程网站，并且公开了自己录制的网课视频，交互式的在线章节测试，以及利用 WireShark 进行抓包分析的 lab。唯一遗憾的是这门课并没有硬核的编程作业，而 Stanford 的 [CS144](https://csdiy.wiki/计算机网络/CS144/) 能很好地弥补这一点。

## 课程资源

- 课程网站：https://gaia.cs.umass.edu/kurose_ross/index.php
- 课程视频：https://gaia.cs.umass.edu/kurose_ross/lectures.php
- 课程教材：Computer Networking: A Top-Down Approach
- 课程作业：https://gaia.cs.umass.edu/kurose_ross/wireshark.php

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/Computer-Network-A-Top-Down-Approach - GitHub](https://github.com/PKUFlyingPig/Computer-Network-A-Top-Down-Approach) 中。

May 21, 2024

# CS144: Computer Network

## 课程简介

- 所属大学：Stanford
- 先修要求：一定的计算机系统基础，CS106L
- 编程语言：C++
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：100 小时

这门课的主讲人之一是网络领域的巨擘 [Nick McKeown](http://yuba.stanford.edu/~nickm/index.html) 教授。这位拥有自己创业公司的学界业界双巨佬会在他慕课每一章节的最后采访一位业界的高管或者学界的高人，非常开阔眼界。

在这门课的 Project 中，你将用 C++ 循序渐进地搭建出整个 TCP/IP 协议栈，实现 IP 路由以及 ARP 协议，最后利用你自己的协议栈代替 Linux Kernel 的网络协议栈和其他学生的计算机进行通信，非常 amazing！

## 课程资源

- 课程网站：https://cs144.github.io/
- 课程视频：https://www.youtube.com/watch?v=r2WZNaFyrbQ&list=PL6RdenZrxrw9inR-IJv-erlOKRHjymxMN
- 课程教材：无
- 课程作业：https://cs144.github.io/，8 个 Project 带你实现整个 TCP/IP 协议栈

## 资源汇总

- [PKUFlyingPig](https://github.com/PKUFlyingPig/CS144-Computer-Network)
- [Lexssama&#39;s Blogs](https://lexssama.github.io/tags/CS144/)
- [huangrt01](https://github.com/huangrt01/CS-Notes/blob/master/Notes/Output/Computer-Networking-Lab-CS144-Stanford.md)
- [kiprey](https://kiprey.github.io/tags/CS144/)
- [康宇PL&#39;s Blog](https://www.cnblogs.com/kangyupl/p/stanford_cs144_labs.html)
- [doraemonzzz](http://doraemonzzz.com/tags/CS144/)
- [ViXbob&#39;s libsponge](https://vixbob.moe/25.html)
- [吃着土豆坐地铁的博客](https://www.epis2048.net/categories/Code/Stanford-CS144/)
- [Smith](https://www.inlighting.org/archives/2021-cs144-notes/)
- [星遥见](https://www.cnblogs.com/weijunji/tag/CS144/)
- [EIMadrigal](https://www.cnblogs.com/EIMadrigal/p/15500472.html)
- [Joey](http://yuzijun.life/2021-02/CS144)

May 21, 2024

# 数据库系统

# UCB CS186: Introduction to Database System

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS61A, CS61B, CS61C
- 编程语言：Java
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

如何编写 SQL 查询？SQL 命令是如何被一步步拆解、优化、转变为一个个磁盘查询指令的？如何实现高并发的数据库？如何实现数据库的故障恢复？什么又是非关系型数据库？这门课会带你深入理解关系型数据库的内部细节，并在掌握理论知识之后，动手用 Java 实现一个支持 SQL 并发查询、B+ 树 Index 和故障恢复的关系型数据库。

从实用角度来说，这门课还会在编程作业中锻炼你编写 SQL 查询以及 NoSQL 查询的能力，对于构建一些全栈的工程项目很有帮助。

## 课程资源

- 课程网站：https://cs186berkeley.net/
- 课程视频：https://www.bilibili.com/video/BV13a411c7Qo
- 课程教材：无
- 课程作业：6 个 Project

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CS186 - GitHub](https://github.com/PKUFlyingPig/CS186) 中。

May 21, 2024

# CMU 15-445: Database Systems

## 课程简介

- 所属大学：CMU
- 先修要求：C++，数据结构与算法，CMU 15-213 (A.K.A. CS:APP，这也是 CMU 内部对每年 Enroll 同学的先修要求)
- 编程语言：C++
- 课程难度：🌟🌟🌟🌟
- 预计学时：100 小时

作为 CMU 数据库的入门课，这门课由数据库领域的大牛 Andy Pavlo 讲授（“这个世界上我只在乎两件事，一是我的老婆，二就是数据库”）。

这是一门质量极高，资源极齐全的 Database 入门课，这门课的 Faculty 和背后的 CMU Database Group 将课程对应的基础设施 (Autograder, Discord) 和课程资料 (Lectures, Notes, Homework) 完全开源，让每一个愿意学习数据库的同学都可以享受到几乎等同于 CMU 本校学生的课程体验。

这门课的亮点在于 CMU Database Group 专门为此课开发了一个教学用的关系型数据库 [bustub](https://github.com/cmu-db/bustub)，并要求你对这个数据库的组成部分进行修改，实现上述部件的功能。

具体来说，在 15-445 中你需要在四个 Project 的推进中，实现一个面向磁盘的传统关系型数据库 Bustub 中的部分关键组件。

包括 Buffer Pool Manager (内存管理), B Plus Tree (存储引擎), Query Executors & Query Optimizer (算子们 & 优化器), Concurrency Control (并发控制)，分别对应 `Project #1` 到 `Project #4`。

值得一提的是，同学们在实现的过程中可以通过 `shell.cpp` 编译出 `bustub-shell` 来实时地观测自己实现部件的正确与否，正反馈非常足。

此外 bustub 作为一个 C++ 编写的中小型项目涵盖了程序构建、代码规范、单元测试等众多要求，可以作为一个优秀的开源项目学习。

## 课程资源

- 课程网站：[Fall 2019](https://15445.courses.cs.cmu.edu/fall2019/schedule.html), [Fall 2020](https://15445.courses.cs.cmu.edu/fall2020/schedule.html), [Fall 2021](https://15445.courses.cs.cmu.edu/fall2021/schedule.html), [Fall 2022](https://15445.courses.cs.cmu.edu/fall2022/schedule.html), [Spring 2023](https://15445.courses.cs.cmu.edu/spring2023/schedule.html)
- 课程视频：课程网站免费观看, Fall 2022 的 [Youtube 全开源 Lectures](https://www.youtube.com/playlist?list=PLSE8ODhjZXjaKScG3l0nuOiDTTqpfnWFf)
- 课程教材：Database System Concepts
- 课程作业：5 个 Project 和 5 个 Homework

在 Fall 2019 中，`Project #2` 是做哈希索引，`Project #4` 是做日志与恢复。

在 Fall 2020 中，`Project #2` 是做 B 树，`Project #4` 是做并发控制。

在 Fall 2021 中，`Project #1` 是做缓存池管理，`Project #2` 是做哈希索引，`Project #4` 是做并发控制。

在 Fall 2022 中，与 Fall 2021 相比只有哈希索引换成了 B+ 树索引，其余都一样。

在 Spring 2023 中，大体内容和 Fall 2022 一样（缓存池，B+ 树索引，算子，并发控制），只不过 `Project #0` 换成了 `Copy-On-Write Trie`，同时增加了很好玩的注册大小写函数的 Task，可以直接在编译出的 `bustub-shell` 中看到自己写的函数的实际效果，非常有成就感。

值得注意的是，现在 bustub 在 2020 年以前的 version 都已经停止维护。

Fall 2019 的最后一个 `Logging & Recovery` 的 Project 已经 broken 了（在19年的 `git head` 上也许还可以跑，但尽管如此 Gradescope 应该也没有提供公共的版本，所以并不推荐大家去做，只看看代码和 Handout 就可以了）。

或许在 Fall 2023 的版本 Recovery 相关的功能会被修复，届时也可能有全新的 `Recovery Project`，让我们试目以待吧🤪

如果大家有精力的话可以都去尝试一下，或者在对书中内容理解不是很透彻的时候，尝试做一做对应的 Project 会加深你的理解（个人建议还是要全部做完，相信一定对你有帮助）。

## 资源汇总

非官方的 [Discord](https://discord.com/invite/YF7dMCg) 是一个很好的交流平台，过往的聊天记录几乎记载了其他同学踩过的坑，你也可以提出你的问题，或者帮忙解答别人的问题，相信这是一份很好的参考。

关于 Spring 2023 的通关指南，可以参考 [@xzhseh](https://github.com/xzhseh) 的这篇[CMU 15-445/645 (Spring 2023) Database Systems 通关指北](https://zhuanlan.zhihu.com/p/637960746)，里面涵盖了全部你需要的通关道具，和通关方式建议，以及最重要的，我自己在做 Project 的过程中遇到的，看到的，和自己亲自踩过的坑。

@ysj1173886760 在学习这门课中用到的所有资源和作业实现都汇总在 [ysj1173886760/Learning: db - GitHub](https://github.com/ysj1173886760/Learning/tree/master/db) 中。

由于 Andy 的要求，仓库中没有 Project 的实现，只有 Homework 的 Solution。特别的，对于 Homework1，@ysj1173886760 还写了一个 Shell 脚本来帮大家执行自动判分。

另外在课程结束后，推荐阅读一篇论文 [Architecture Of a Database System](https://github.com/ysj1173886760/paper_notes/tree/master/db)，对应的中文版也在上述仓库中。论文里综述了数据库系统的整体架构，让大家可以对数据库有一个更加全面的视野。

## 后续课程

[CMU15-721](https://15721.courses.cs.cmu.edu/spring2020/) 主要讲主存数据库有关的内容，每节课都有对应的 paper 要读，推荐给希望进阶数据库的小伙伴。@ysj1173886760 目前也在跟进这门课，完成后会在这里提 PR 以提供进阶的指导。

May 21, 2024

# Caltech CS 122: Database System Implementation

## 课程简介

- 所属大学：Caltech
- 先修要求：无
- 编程语言：Java
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

加州理工的这门课，不同于没有提供 SQL 层功能的 CMU15-445 课程。CS122 课程 Lab 的侧重点在于 SQL 层的相关实现，涉及查询优化器的各个模块，比如SQL的解析，Translate，如何实现 Join，统计信息以及代价估计，子查询实现，Agg，Group By 的实现等。除此之外，还有 B+树，WAL 相关实验。本门课程适合在学完 CMU15-445 课程之后，对查询优化相关内容有兴趣的同学。

下面介绍一下这门课的前 3 个 Assignment 也就是实验 Lab 所要实现的功能：

### Assignment1

- 为 NanoDB 提供 delete，update 语句的支持。
- 为 Buffer Pool Manager 添加合适的 pin/unpin 代码。
- 提升 insert 语句的性能， 同时不使数据库文件大小过分膨胀。

### Assignment2

- 实现一个简单的计划生成器，将各种已经 Parser 过的 SQL 语句转化为可执行的执行计划。
- 使用 nested-loop join 算法，实现支持 inner- and outer-join 的 Join 计划节点。
- 添加一些单元测试， 保证 inner- and outer-join 功能实现正确。

### Assignment3

- 完成收集表的统计信息。
- 完成各种计划节点的计划成本计算。
- 计算可出现在执行计划中的各种谓词的选择性。
- 根据谓词更新计划节点输出的元组统计信息。

剩余 Assignment 和 Challenges 可以查看课程介绍，推荐使用 IDEA 打开工程，Maven 构建，注意日志相关配置。

## 课程资源

- 课程网站：http://courses.cms.caltech.edu/cs122/
- 课程代码：https://gitlab.caltech.edu/cs122-19wi
- 课程教材：无
- 课程作业：7 Assignments + 2 Challenges

May 21, 2024

# Stanford CS 346: Database System Implementation

## 课程简介

- 所属大学：Stanford
- 先修要求：无
- 编程语言：C++
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

RedBase 是 cs346 的一个项目，实现了一个简易的数据库系统，项目是高度结构化的。整个项目能够被分为以下几个部分（同时也是 4 个需要完善的 lab）：

1. The record management component：记录管理组件。
2. The index component：B+ 索引管理。
3. The System Management Component：ddl语句、命令行工具、数据加载命令、元数据管理。
4. The Query Language Component：在这个部分需要实现 RQL Redbase 查询语言。RQL 要实现 select、insert、delete、update 语句。
5. Extension Component：除了上述数据库系统的基本功能组件，还需要实现一个扩展组件，可以是 Blob 类型、 网络模块、连接算法、CBO 优化器、OLAP、事务等。

RedBase 适合在学完 CMU 15-445 后继续学习数据库系统中的其他组件，因为其代码量不多，可以方便的根据需要扩展代码。同时代码完全由 C++ 编写，也可以用于练习 C++ 编程技巧。

## 课程资源

- 课程网站：https://web.stanford.edu/class/cs346/2015/
- 课程代码：https://github.com/junkumar/redbase.git
- 课程教材：无
- 课程作业：4 Projects + 1 Extension

May 21, 2024

# CMU 15-799: Special Topics in Database Systems

## 课程简介

- 所属大学：CMU
- 先修要求：CMU 15-445
- 编程语言：C++
- 课程难度：🌟🌟🌟
- 预计学时：80 小时

这门课目前只开了两次：fall2013 和 spring2022，讨论了数据库领域的一些前沿主题。fall2013 讨论了 Streaming、Graph DB、NVM 等，spring2022 主要讨论 Self-Driving DBMS，都提供有相关论文。

spring2022 版课程任务：

任务一：基于 `PostgreSQL` 进行手动性能调优；

任务二：基于 [NoisePage Pilot](https://github.com/cmu-db/noisepage-pilot) 改进 Self-Driving DBMS，不限特性。

授课更贴近讲座的形式，编程任务较少。对一般同学可以开拓一下视野，对专精数据库的同学可能帮助较大。

## 课程资源

- 课程主页
- [CMU15-799 - Special Topics in Database Systems](https://15799.courses.cs.cmu.edu/fall2013)
- [CMU15-799 - Special Topics: Self-Driving Database Management Systems](https://15799.courses.cs.cmu.edu/spring2022/)
- 课程视频：暂无
- 课程作业：2 Projects + 1 Group Project

May 21, 2024

# 编译原理

# PKU 编译原理实践

## 课程简介

- 所属大学：北京大学
- 先修要求：计算机系统基础、数据结构与算法、编程基础
- 编程语言：C/C++/Rust 任选其一
- 课程难度：🌟🌟🌟🌟
- 预计学时：60 小时

北京大学的编译原理实践课程旨在实现一个从精简版的 C 语言 —— SysY 编译到 RISC-V 汇编的编译器。和其他提供了框架代码的课程不同，该课程给予了你极大的自由度，测试程序只会对你输出的汇编代码的正确性进行测试，而不会对你编译器的具体设计甚至使用的编程语言做任何限制。你需要从一个空文件夹开始一步步构建出独属于你自己的编译器。但平地起高楼即使对于北大的同学也是相当有难度的，因此课程助教 [@MaxXing](https://github.com/MaxXSoft) 在2022年对课程实验进行重大升级，为课程专门设计了一种中间表示 Koopa IR (intermediate representation)。Koopa IR 在设计上更为合理，在形式上类似于 LLVM IR，但简化了相当多的内容，只专注于实践需要的部分。与此同时，还为 Koopa IR 设计了配套的运行时库，你可以借助这套运行时库轻松地解析/生成/修改/输出 Koopa IR，完全不需要对其他无用的细节做过多考虑。另外，还有一份保姆级的文档将构建编译器这样一个大工程循序渐进地拆分成了9个小步骤，让任何愿意花时间的同学都可以更容易地实现自己的编译器。

以下内容摘自 @MaxXing 在其 [Blog](https://blog.maxxsoft.net/index.php/archives/145/) 中对该课程实验的介绍：

---

你可能已经见过无数个教你写编译器的教程了，但它们也许或多或少存在各种问题，导致你看了它们之后，依然觉得无从下手：

- 教程并非面向“零编译器基础”的人群，理解起来比较费劲。
- 只教了怎么做一个编译器，但没教为什么这么做，读完之后还是觉得一头雾水。
- 开始编码之前，需要复杂的环境配置，开局劝退。
- 上来先做和“编译一个程序”这件事八竿子打不着的东西，跟着教程学一个月才能看到自己的编译器编出一个能跑的程序，反馈周期过长。
- 最终写出来的只是个解释器，或者不能编译到真实的 ISA（例如输出了某种字节码），或者高度依赖其他框架（例如 LLVM），让人体会不到那种“我真的写出个编译器”的成就感，以及“所有事情都由自己实现”的酣畅感。
- 实现的编译器只能编译一些过于简单的程序，比如排序算法等等，看起来非常无聊。谁会没事干排序玩啊？
- 教程及其配套资源非中文，或需要付费，且不开源。

研究生期间，我一直在担任本科编译原理课程的助教。为了让本科生更好地理解编译器工作的原理，在参考多个其他教程之后，我设计了一套全新的，教你从零开始写个编译器的教程：

- 你可以使用 C/C++/Rust 开发你的编译器，教程只要求你具备使用这些语言编程的能力，不要求任何编译原理的基础和相关实践经验。
- 教程除了告诉你要如何写一个编译器，还会告诉你为什么这么做，以及除此之外还能怎么做。
- 教程采用增量式、迭代式的思路，引导你从一个只能处理 main 函数的编译器开始，逐步扩展实现一个能处理包括控制流、函数调用、数组在内的，类 C 语言的编译器。编译器可以输出 RISC-V 汇编。
- 提供基于 Docker 的实验环境，一键配置。环境中还附带自动测试脚本，一键测试你写的编译器。
- 教程介绍了相关工具，可以为你代劳一些枯燥的苦力活，比如生成 lexer/parser，解析和生成 IR 等等。剩下的事情，如构建 AST、语义分析、生成 IR 以及生成目标代码，完全由你自己编程实现。
- 你最终实现的编译器足以编译很多复杂的程序，例如 Mandelbrot 集绘制程序，或者 Lisp 解释器（这个解释器甚至可以解释另一个 Lisp 解释器）。我们会提供这些程序，让你用你写的编译器体验到最真实的快乐。
- 教程及其配套工具、实验环境等，全部开源，完全免费！
- 你可以从 GitHub Pages 上访问到这个教程：[北京大学编译实践课程在线文档](https://pku-minic.github.io/online-doc/#/)。如果你之前从来没有尝试过自己写一个编译器，不如现在就来试一下吧！

我的愿望是，让每个人都感受到写编译器的快乐。

---

最后，向 @MaxXing 致以我崇高的敬意。—— from PKUFlyingPig

May 21, 2024

# Stanford CS143: Compilers

## 课程简介

- 所属大学：Stanford
- 先修要求：计算机体系结构
- 编程语言：Java 或 C++
- 课程难度：🌟🌟🌟🌟🌟
- 预计学时：150 小时

斯坦福的编译原理课程，设计者开发了一个 Class-Object-Oriented-Language，简称 COOL 语言。这门课的核心就是通过理论知识的学习，为 COOL 语言实现一个编译器，将 COOL 高级语言编译为 MIPS 汇编并在 Spim 这个 MIPS 模拟器上成功执行。

理论部分基本按照龙书的顺序覆盖了词法分析、语法分析、语义分析、运行时环境、寄存器分配、代码优化与生成等内容，实践部分则相应地分为词法分析、语法分析、语义分析、代码生成四个阶段，难度循序渐进，并在优化部分给学生留下了很大的设计空间。

## 课程资源

- 课程网站：http://web.stanford.edu/class/cs143/
- 课程视频：https://www.bilibili.com/video/BV17K4y147Bz
- 课程教材：龙书
- 课程作业：5 个书面作业 + 5 个编程作业带你实现一个编译器

## 资源汇总

@skyzluo 在学习这门课中用到的所有资源和作业实现都汇总在 [skyzluo/CS143-Compilers-Stanford - GitHub](https://github.com/skyzluo/CS143-Compilers-Stanford) 中。

May 21, 2024

# NJU 编译原理

## 课程简介

- 所属大学：南京大学
- 先修要求：离散数学
- 编程语言：Java
- 课程难度：🌟🌟🌟
- 预计学时：80 小时

南京大学的编译原理课程，设计者选用了当下热门的 ANTLR （ANother Tool for Language Recognition） v4 编程语言解析生成工具辅助教学，能让使用者专心词法或者语法分析的设计，而让 ANTLR 4 来生成重复的模板代码。IDE 也有其插件，装上后，可以实现即时的可视化语法树，方便学生理解。

ANTLR 4 是 LL 解析器生成器，比起 LR 和 LALR 解析器生成器，它可处理语法的范围相对狭窄。但另一方面其生成的解析器有易于理解和使用的优势。此外，因为其支持“无限长的 token 超前扫描”，所以可处理语法范围狭窄的问题也得到了很好的改善。

老师通过适当的图解和生活例子，幽默风趣地讲述编译原理，让人听来不算乏闷。尤其是今年这版，采取先实际使用 ANTLR 4 完成一些小例子，再补足理论知识的方式。让人能带着问题去找到适配的理论，更让人印象深刻。通过理论知识的学习，逐渐揭开 C 语言的“神秘面纱”。

理论部分基本按照龙书节奏叙述。包括词法分析、语法分析、语义分析、运行时环境、寄存器分配、代码优化与生成等内容。

实践则是本课程的亮点，一步步的，由简单到复杂地实现一个属于自己的编译器。

教授本课的老师极为慷慨，校外学生同样能享受到 Online Judge 以及参与课程讨论，老师还极为细心地整理历年来的学习资料，在课程网站里十分容易找到。

老师还把教学班的 [Zulip](https://2024-compilers-at-software-nju.zulipchat.com/join/wxwq3fib56ltlff2mk6qyrz5/) 地址公开（若有变更，在课程网站也能找到），这意味着你有任何问题，都能在上面提问，同时你也能看到跟你一起学习的南大学生的问题，这些问题都会得到助教和老师的回答，所以我并不用再赘述踩了哪些坑或者经验，因为你能在一个平台上，和一帮正在学习相同内容的人，一起交流问题。

最大感受是，心里不再对实现一个编译器有畏难情绪，也不再无从下手，学完课程，会有一套初步的行之有效的思路，让我们面对挑战。

## 课程资源

- 课程网站：http://docs.compilers.cpl.icu/
- 课程视频：https://space.bilibili.com/479141149/channel/collectiondetail?sid=2312309
- 课程教材：龙书等
- 课程作业：10 个书面作业 + 8 ~ 10 个编程作业带你实现一个编译器

May 21, 2024

# 编程语言设计与分析

# CS242 Programming Languages

## 课程简介

- 所属大学：Stanford
- 先修要求：对计算机系统和编程语言理论有初步了解
- 编程语言：OCaml, Rust
- 课程难度：🌟🌟🌟🌟
- 预计学时：60 小时

CS242是一门讲程序语言 (Programming Language, PL) 的课程，但不是传统意义上的纯理论导向。这门课程首先介绍了如 Lambda 演算，类型系统这样的经典 PL 理论，然后借助系统编程的思想和实际的编程语言来驱动学生理解这些理论，展示了它们是如何在实际编程中帮助开发者避免各种错误。

主讲老师 Will Crichton 还将他的课程设计思想写成了论文 [From Theory to Systems: A Grounded Approach to Programming Language Education](https://arxiv.org/abs/1904.06750)，阐述了这条从理论走向系统的教学路线。

我们通过简单介绍每个作业来帮助读者了解这门课程的具体内容：

- 对 JSON 的形式化与证明
- PL 中经典的 Lambda 演算
- 以 OCaml 为例的函数式编程入门
- 使用 OCaml 实现一个函数式语言的类型检查器和解释器，同样是 PL 的经典作业
- WebAssembly 的理论与实践
- Linear Type 和 Rust 的所有权机制
- Rust 的异步编程基础
- 利用 Rust 类型系统设计状态机和实现 session-typed TCP 库
- 最后的大作业有四个可选项：
  1. 使用 Lean 进行定理证明
  2. 使用 Rust 实现 Read-Log-Update 同步机制
  3. 利用 F* 语言验证文件系统的正确性
  4. 在程序语言视角下使用 OCaml 实现一个深度学习框架

这些作业涵盖知识跨度非常大，从最经典的编程语言理论证明和实践到以 Rust 为例的编程语言对于编程和系统设计的影响，再到最后各有特色的大作业。几乎所有的编程作业都有详尽的本地测试，尤其是大作业中的深度学习框架更有超过 200 个测试，适合自学。

前面几次的作业偏 PL 理论，后面几次的作业偏系统编程。 如果你觉得前面几次的课程内容和作业过于理论，可以重点尝试使用 OCaml 实现解释器的作业，它既能让你对之前的理论有更深刻的理解，又能让你实战一个函数式语言的类型检查和解释。

而后面的作业则更倾向于利用理论来指导系统编程与设计，尤其是 Rust 和它独特的所有权机制与类型系统。虽然我们要经常与编译器搏斗，但这也恰好说明了类型系统和理论对于编程和设计的意义。

个人自学过程中感觉作业还是偏难的，但收获很大，在后续作业的编程实践和前面所学的理论知识产生交集时会有恍然大悟的愉悦。如果你在完成作业时遇到了困难，这是十分正常的，请静下心来认真思考，或者再读一遍实验指导。

## 课程资源

- 课程网站：[官网](https://stanford-cs242.github.io/f19/)
- 课程视频：无，主要学习途径是课程笔记和完成作业
- 课程教材：前半部分是著名的[TAPL](https://www.cis.upenn.edu/~bcpierce/tapl/)，后半部分则无固定教材
- 课程作业：[实验指导](https://stanford-cs242.github.io/f19/assignments/)与[作业仓库](https://github.com/stanford-cs242/f19-assignments)

May 21, 2024

# NJU 软件分析

## 课程简介

- 所属大学：南京大学
- 先修要求：数据结构与算法，至少熟悉一门编程语言
- 编程语言：Java
- 课程难度：🌟🌟🌟
- 预计学时：60 小时

软件分析是由南京大学李樾老师和谭添老师共同开设的一门课程，主要介绍了程序分析，在这里特指静态分析的理论与实践。 静态分析的理念是在不运行程序的情况下，通过分析其源代码和各种表示来获得关于程序特定性质的**近似**结论。 这门课从程序的抽象语法树，控制流图和中间表示这些基础知识开始介绍，再到数据流分析和指针分析的理论与实践，最后介绍了若干高级主题，如 IFDS 等。

这门课程值得学习的原因在我看来有两部分：

- 授课。程序分析一般来说并不太好上手，但两位老师讲的尤其细致入微，还会在课上带你一步一步走某一个算法的流程。个人认为只要认真听课，对于课上的知识不存在学不懂或者讲的不清楚的问题。
- 作业。作业围绕其自创的 Java 程序分析框架太阿进行。 八个作业涵盖多种静态分析技术，包括编译优化（活跃变量分析、常量传播、死代码检测），基础程序分析（程序调用图构建、非/上下文敏感指针分析），以及程序分析在软件安全性的应用（污点分析）。 课程同时还提供**所有人**可用的在线评测系统，适合自学。

作业主要是实现课上的伪代码算法，从而更好的帮助你理解课上所讲的知识。我感觉难度并不是特别大，特别适合在上完课后完成对应的实验来检验自己对课上知识的掌握程度。 不过想要通过每个作业的所有测试点还是很有难度的。

## 课程资源

- 课程网站：[主页](https://tai-e.pascal-lab.net/lectures.html)
- 课程视频：[Bilibili](https://www.bilibili.com/video/BV1b7411K7P4/?spm_id_from=333.999.0.0&vd_source=b58da8cd0259ee873ef3dc2c9aa36d74)
- 课程教材：无
- 课程作业：[实验主页](https://tai-e.pascal-lab.net/intro/overview.html)
- 在线评测： [OJ](https://oj.pascal-lab.net/problem)

May 21, 2024

# 北京大学 软件分析技术

## 课程简介

- 所属大学：北京大学
- 先修要求：数据结构与算法，至少熟悉一门编程语言
- 编程语言：Java, Python
- 课程难度：🌟🌟🌟🌟
- 预计学时：60 小时

软件分析技术是由北京大学熊英飞老师开设的一门课程，主要介绍了以下内容：

1. 基于抽象解释的程序分析（数据流分析、过程间分析、指针分析、抽象解释等）
2. 基于约束求解的程序分析（SAT、SMT、符号执行等）
3. 软件分析应用（程序合成、缺陷定位、缺陷修复等）

和南京大学的[软件分析课程](https://csdiy.wiki/编程语言设计与分析/NJU-SoftwareAnalysis/)对比，这门课程的特点是讲了**更多更全面**的程序分析的理论与实践相关内容，难度也更大。这门课程我的主要的学习途径是听课，熊老师上课十分有趣，除了理论内容讲的很好偶尔也会讲一些学术相关的小段子:)

而本实验的的课程项目是实现一个Java上的指针分析系统和一个程序合成工具，也是十分有趣的实践。

## 课程资源

- 课程网站：[主页](https://xiongyingfei.github.io/SA/2020/main.htm) 这是 2020 年的课程主页，在[熊老师的主页](https://xiongyingfei.github.io/)上可以找到更多年份的课程内容。
- 课程视频：[2020 燕云直播](https://liveclass.org.cn/cloudCourse/#/courseDetail/8mI06L2eRqk8GcsW)
- 课程教材：无

May 21, 2024

# Cambridge: Semantics of Programming Languages

## 课程简介

- 所属大学：University of Cambridge
- 先修要求：基础离散数学
- 编程语言：OCaml/ML
- 课程难度：🌟🌟🌟
- 预计学时：20 至 30 小时

这门课程系统性地讲述了编程语言中的语义学 (Semantics)。它在定义和设计语言的背景下，为编程语言的构造和规范声明提供了一个非常适合初学者，但同样严谨且形式化的介绍。这也是为数不多的提供公开视频的编程语言理论课程之一。

课程内容涵盖了从操作语义 (Operational Semantics) 到指称语义 (Denotational Semantics) 的各个主题。课程开始会先介绍一个使用 BNF 约束的简单命令式语言的基本操作语义，然后逐步引入形式类型系统，使用归纳法，特别是结构归纳法 (Structural Induction) 来构建基于规则的归纳证明，介绍了程序语言语义学中的许多基本性质及其证明。然后讨论在函数式编程视角下如何操作数据，并介绍着重子类型和函数处理。最后讨论语义等价性、一致性性质以及在并发环境下的语义学。

这门课在校内面向二年级本科生，难度不高，但同时引入了一些非常重要的概念。它将是进一步研究类型理论、范畴理论、霍尔逻辑和模型检测的关键要素。

## 课程资源

- 课程网站：[Latest](https://www.cl.cam.ac.uk/teaching/2324/Semantics/)
- 课程视频：[YouTube](https://www.youtube.com/playlist?list=PL-2hPK7m5S3hVagseKDPxCBZEqg0PqZhs)
- 课程教材：
- Pierce, B.C. (2002). *Types and programming languages*. MIT Press.
- Winskel, G. (1993). *The formal semantics of programming languages*. MIT Press.
- 课程作业：考试真题中的相关题目汇总在 [这里](https://www.cl.cam.ac.uk/teaching/exams/pastpapers/t-SemanticsofProgrammingLanguages.html)，但是相关作业题 (Cambridge 内部的 supervision) 以及所有题目的答案均不公开。

May 21, 2024

# 计算机图形学

# GAMES101

## 课程简介

- 所属大学：UCSB
- 先修要求：线性代数，高等数学，C++
- 编程语言：C++
- 课程难度：🌟🌟🌟
- 预计学时：80 小时

官方介绍:

> 本课程将全面而系统地介绍现代计算机图形学的四大组成部分：（1）光栅化成像，（2）几何表示，（3）光的传播理论，以及（4）动画与模拟。每个方面都会从基础原理出发讲解到实际应用，并介绍前沿的理论研究。通过本课程，你可以学习到计算机图形学背后的数学和物理知识，并锻炼实际的编程能力。 作为入门，本课程会尽可能的覆盖图形学的方方面面，把每一部分的基本概念都尽可能说清楚，让大家对计算机图形学有一个完整的、自上而下的全局把握。全局的理解很重要，学完本课程后，你会了解到图形学不等于 OpenGL，不等于光线追踪，而是一套生成整个虚拟世界的方法。从本课程的标题，大家还可以看到“现代”二字，也就是说，这门课所要给大家介绍的都是现代化的知识，也都是现代图形学工业界需要的图形学基础。

GAMES101 是国内相当有名的图形学公开课。和大家印象中满是数学和算法的图形学不同，这门课以十分生动的方式带我们进入了图形学这个领域的大门。

每个project代码量都不会很多，但是却都十分有趣。在做这些project的过程中，我们会实现简单的光栅化，并渲染一个简易的模型，我们还会实现光线追踪，以追求渲染更好的质量。每个project中还有选做的拓展作业，可以让我们渲染的模型具有更好的质量，更快的渲染速度。

喜欢玩游戏的同学应该对实时光线追踪有一定的了解，这门课的老师闫令琪就对这一技术有直接的推动作用。

跟着课程的视频，做完每一个project，相信你会和我一样对图形学，以及现代的渲染技术产生浓厚的兴趣。

## 课程资源

- 课程网站：[GAMES101](http://games-cn.org/intro-graphics/), [GAMES101](https://sites.cs.ucsb.edu/~lingqi/teaching/games101.html)
- 课程视频：[bilibili](https://www.bilibili.com/video/BV1X7411F744?p=1), [官网](http://games-cn.org/graphics-intro-ppt-video/)
- 课程教材：Fundamentals of Computer Graphics
- 课程作业：[8 个 project](http://games-cn.org/forums/topic/allhw/)

## 资源汇总

@ysj1173886760 在学习这门课中用到的所有资源和作业实现都汇总在[ysj1173886760/Learning: graphics/GAMES101 - GitHub](https://github.com/ysj1173886760/Learning/tree/master/graphics/GAMES101) 中。

May 21, 2024

# GAMES202

## 课程简介

- 所属大学：UCSB
- 先修要求：线性代数，高等数学，C++，GAMES101
- 编程语言：C++
- 课程难度：🌟🌟🌟🌟
- 预计学时：60 小时

官方介绍:

> 本课程将全面地介绍现代实时渲染中的关键问题与解决方法。由于实时渲染 (>30 FPS) 对速度要求极高，因此本课程的关注点将是在苛刻的时间限制下，人们如何打破速度与质量之间的权衡，同时保证实时的高速度与照片级的真实感。
>
> 本课程将以专题的形式呈现，课程内容会覆盖学术界与工业界的前沿内容，包括：（1）实时软阴影的渲染；（2）环境光照；（3）基于预计算或无预计算的全局光照；（4）基于物理的着色模型与方法；（5）实时光线追踪；（6）抗锯齿与超采样；以及一些常见的加速方式等等。
>
> 除了最新最全的内容之外，本课程与其它任何实时渲染的教程还有一个重要的区别，那就是本课程不会讲授任何与游戏引擎的使用相关的内容，并且不会特别强调具体的着色器实现技术，而主要讲授实时渲染背后的科学与知识。本课程的目标是在你学习完这门课的时候，你将有深厚的功底去开发一个属于你自己的实时渲染引擎。

作为 GAMES101 的进阶课程，难度有一定的提升，但不会很大，相信完成了 GAMES101 的同学都有能力完成这门课程。每个 project 代码量都不会很多，但是都需要一定的思考。

## 课程资源

- 课程网站：[GAMES202](https://sites.cs.ucsb.edu/~lingqi/teaching/games202.html)
- 课程视频：[bilibili](https://www.bilibili.com/video/BV1YK4y1T7yY)
- 课程教材：Real-Time Rendering, 4th edition.
- 课程作业：[5个project](http://games-cn.org/forums/topic/games202zuoyehuizong/)

May 21, 2024

# GAMES103

## 课程简介

- 所属大学：Style3D/OSU
- 先修要求：线性代数，高等数学，大学物理，编程能力，基本图形知识
- 编程语言：C#
- 课程难度：🌟🌟🌟🌟
- 预计学时：50 小时

官方介绍：

> 本课程将作为基于物理的计算机动画技术入门，着重介绍各种基础的物理动画模拟技术。
>
> 该课程主要涵盖四个方向，分别为：1）刚体模拟；2）质点弹簧、约束与布料模拟；3）基于有限元的弹性体模拟；4）流体模拟。
>
> 本课程内容将不会涉及具体的物理模拟引擎，但会讨论各种引擎背后的技术，以及它们的优缺点等等。由于开发学习物理模拟需要一定的数学基础，课程初始阶段也会花一定的时间复习必备的数学知识。顺利完成课程之后，同学们应该会对基础的物理模拟技术有深入理解，对高级的模拟技术也会有部分接触。

图形学可粗略分为渲染、模拟、几何三个领域。GAMES101 和 GAMES202 主要以渲染为主，而对于物理模拟，GAMES103 则是很棒的学习资源。

## 课程资源

- 课程网站：[GAMES103](http://games-cn.org/games103/)
- 课程视频：[bilibili](https://www.bilibili.com/video/BV12Q4y1S73g)
- 参考资料：[课程PPT](https://www.aliyundrive.com/s/YGuzfDCzw4n/folder/61824d985307bbf3920044b4afd48abb633441f6)
- 课程作业：共四次作业，可见官方BBS小程序或非官方的Repo：[GAMES103 HW](https://github.com/indevn/GAMES103/tree/main/HW)

## 资源汇总

@indevn 在学习这门课中用到的所有资源和作业要求都汇总在 [GAMES103 Unoffical](https://github.com/indevn/GAMES103) 中。对于作业的具体实现，在知乎上有很多相关文章进行了细致讲解可以参考。

May 21, 2024

# Stanford CS148

## 课程简介

- 所属大学：Stanford
- 先修要求：线性代数，高等数学，Python
- 编程语言：Python
- 课程难度：🌟🌟🌟
- 预计学时：40 小时

官方介绍:

这是一门计算机图形学的入门课程，这门课的一开始使用 Blender 去生成图像，并且理解底层的数学知识，包括三角形、法向量、插值、纹理映射、凹凸贴图等等。之后会介绍光线和颜色以及它们如何影响计算机的显示和打印。同时也会介绍 BRDF 以及一些基本的光照和着色模型。课程的最后，会涉及到光线追踪、反走样、加速结构等内容。

具体课程信息可以查看[课程网站](https://web.stanford.edu/class/cs148/index.html)。

这门课程比起 GAMES101 浅一些，编程语言使用的是 Python，对于不熟悉 C++ 的同学比较友好。

## 课程资源

- 课程网站：[CS148](https://web.stanford.edu/class/cs148/index.html)
- 课程视频：无，直接看[lecture](https://web.stanford.edu/class/cs148/lectures.html)就可以了，也可以参考 GAMES101 视频
- 课程教材：Fundamentals of Computer Graphics
- 课程作业：[8 个 hw, 1 个 final project](https://web.stanford.edu/class/cs148/assignments.html)

May 21, 2024

# CMU 15-462 : COMPUTER GRAPHICS

## 课程简介

- 所属大学：CMU
- 先修要求：基础的向量微积分和线性代数 , 基础的 C/C++ 编程能力。
- 编程语言：C/C++
- 课程难度：🌟🌟🌟🌟
- 预计学时：100 小时

本课程全面介绍了计算机图形学。它侧重于基本概念和技术，以及它们与图形中多个问题领域（渲染、动画、几何、成像）的交叉关系。主题包括：采样、混叠、插值、光栅化、几何变换、参数化、可见性、合成、过滤、卷积、曲线和曲面、几何数据结构、细分、网格划分、空间层次结构、光线追踪、辐射测量、反射率、光场、几何光学，蒙特卡洛渲染，重要性采样，相机模型，高性能光线追踪，微分方程，时间积分，数值微分，基于物理的动画，优化，数值线性代数，逆运动学，傅立叶方法，数据拟合.

## 课程资源

- 课程网站：http://15462.courses.cs.cmu.edu/fall2022/
- 课程视频：
  - [Youtube](https://www.youtube.com/watch?v=W6yEALqsD7k&list=PL9_jI1bdZmz2emSh0UQ5iOdT2xRHFHL7E&index=1)
  - [bilibili](https://www.bilibili.com/video/BV1QZ4y1K7ga)
- 课程教材：15-462 没有唯一的课本, 提供了各种书籍供你参考. 如下:
  - [Fundamentals of Computer Graphics. A K Peters, 2009](http://www.amazon.com/Fundamentals-Computer-Graphics-Peter-Shirley/dp/1568814690)
  - [Computer Graphics: Principles and Practice](http://www.amazon.com/Computer-Graphics-Principles-Practice-3rd/dp/0321399528/ref=sr_1_2?s=books&ie=UTF8&qid=1440872554&sr=1-2&keywords=foundations+of+3d+computer+graphics)
  - [Physically Based Rendering: From Theory to Implementation](http://www.amazon.com/gp/product/0123750792?ie=UTF8&tag=pharr-20&linkCode=as2&camp=1789&creative=390957&creativeASIN=0123750792)
- 课程作业：参见课程主页

May 21, 2024

# USTC Computer Graphics

## 课程简介

- 所属大学：中国科学技术大学
- 先修要求：微积分，线性代数，C/C++编程，数据结构
- 编程语言：C/C++
- 课程难度：🌟🌟🌟
- 预计学时：100小时

中科大数学学院的刘利刚老师在20年疫情期间上传的课程，个人感觉跟 Games101 的注重渲染相比在内容上更全面，有着后者所没有的离散几何处理等内容，看起来更加数学化，可以与 Games101 进行互补，课程资料全面公开。

## 课程资源

- 课程网站：http://staff.ustc.edu.cn/~lgliu/Courses/ComputerGraphics_2020_spring-summer/default.htm
- 课程视频：https://www.bilibili.com/video/BV1iT4y1o7oM/?spm_id_from=333.880.my_history.page.click&vd_source=eea47a16439992e41b232bc5d5684e27
- 课程教材：本课程不规定使用规定教材，以学术前沿论文为主，以下教材仅仅为参考 E. Angel, Interactive Computer Graphics — A top-down approach using OpenGL™, 6th ed., 2011. （中文翻译版：交互式计算机图形学—基于 OpenGL 的自顶向下方法（第五版），电子工业出版社，2012）
- 课程作业：http://staff.ustc.edu.cn/~lgliu/Courses/ComputerGraphics_2020_spring-summer/default.htm ，九个作业加一个 Project ，具体看官网

May 21, 2024

# Web开发

# MIT Web Development Crash Course

## 课程简介

- 所属大学：MIT
- 先修要求：掌握至少一门编程语言
- 编程语言：JavaScript/HTML/CSS/NoSQL
- 课程难度：🌟🌟🌟
- 预计学时：因人而异

MIT 在每年 1 月份会有一个为期 4 周的 [Independent Activities Period](https://elo.mit.edu/iap/) (IAP)，在这个月里，MIT 的学生和老师可以自由地开设很多有趣的课程，而这门网站开发课程就是其中之一。

在一个月的时间里，你会从零开始掌握一个网站的设计、搭建、美化、交互等等核心内容，基本覆盖了 Web 开发的前后端大部分技术栈。如果你不需要系统地学习网络开发，而只是出于兴趣想把它加入自己的技能包里，那么这门课将非常适合你。

## 课程资源

- 课程网站：https://weblab.mit.edu/schedule/
- 课程视频：参见课程网站链接
- 课程作业：参见课程 Schedule

May 21, 2024

# Stanford CS142: Web Applications

## 课程简介

- 所属大学：Stanford
- 先修要求：有一定的编程经验
- 编程语言：JavaScript/HTML/CSS
- 课程难度：🌟🌟🌟🌟
- 预计学时：100 小时

斯坦福的 Web 应用开发课程，内容覆盖了 HTML, CSS, JavaScript, ReactJs, NodeJS, ExpressJS, Web安全等等。8 个 Project 会让你在实战中锻炼自己的 Web 开发技巧。

## 课程资源

- 课程网站：https://web.stanford.edu/class/cs142/index.html
- 课程视频：https://web.stanford.edu/class/cs142/lectures.html
- 课程教材：无
- 课程作业：https://web.stanford.edu/class/cs142/projects.html

May 21, 2024

# University of Helsinki: Full Stack open 2022

## 课程简介

- 所属大学：University of Helsinki
- 先修要求：具备良好的编程技能、基本的网络编程和数据库知识，并且了解使用 Git 这个版本控制系统的基础知识。
- 编程语言：JavaScript/HTML/CSS/NoSQL/SQL
- 课程难度：🌟🌟
- 预计学时：因人而异

本课程是介绍如何使用 JavaScript 开发现代Web应用程序。 课程的重点是使用 ReactJS 构建单页面应用程序（SPA），并使用由 Node.js 构建 REST API。该课程还包含介绍 GraphQL 的部分，这是 REST API 的现代替代方案。

课程还包括测试、配置和环境管理，以及使用 MongoDB 来存储应用的数据。

## 课程资源

- 课程网站：https://fullstackopen.com/zh/
- 课程作业：参见课程网站
- 课程 Discord 群组：https://study.cs.helsinki.fi/discord/join/fullstack/
- 课程 Telegram 群组：https://t.me/fullstackcourse/

May 21, 2024

# CS571 Building UI (React & React Native)

## 课程简介

- 所属大学：威斯康星大学麦迪逊分校（University of Wisconsin, Madison）
- 先修要求：CS400（高级 Java，但个人觉得先修不必要，掌握至少一门编程语言即可）
- 编程语言：JavaScript/HTML/CSS
- 课程难度：🌟🌟🌟
- 预计学时：每周 2 小时（讲座）+ 每周 4–10 小时（作业），持续 12 周

该课程提供了 React 前端开发和 React Native 移动端开发的最佳实践介绍，完整的同时又提纲挈领。采用 React 和 React Native 的最新版本，课程网站每学期都会更新。对于各门工具迭出的前端开发难能可贵。

同时，该课程也提供了很好的训练机会。在整个学期中，需要为较大作业量做好准备。作业所涉及的技术和知识点会在课上讲解，但不会手把手写代码（个人认为手把手写代码效率非常低，而 Udemy 上多为此类型）。由于不是保姆级课程，如果写作业时对于 React 的某些功能不确定怎么写，建议在动手之前多花些时间仔细阅读 [react.dev](https://react.dev/reference/react) 上的相关章节。作业的 starter code 提供的训练起点也恰好合适，不用为配 Node.js 环境伤脑筋。

尽管这门课程不要求预先会 Javascript/HTML/CSS，课堂上对 syntax 的介绍比较有限，建议学习和写码遇到语法问题时勤查勤问。

此外，本课程还对 Google 旗下的 ChatBot 开发工具 Dialog Flow 有较为深入的介绍和练习。还对 UX Design 的实用原则和技术有所讲解。

所有课程资料和作业都是开源的，但你需要向授课教师 Cole Nelson (ctnelson2@wisc.edu) 发送电子邮件以获取 X-CS571-ID。该 ID 是向 API 发送 request 必需。在发送邮件时，建议附上自我介绍。目前还不清楚老师是否愿意给所有人提供ID，如果老师表示无法分享，请[在 GitHub repo 里提一个 issue](https://github.com/PKUFlyingPig/cs-self-learning/issues/new/choose)。

## 课程资源

- 课程网站：[https://cs571.org](https://cs571.org/)
- 课程视频：请参考课程网站上标有“R”的链接
- 课程作业：请参考课程网站上的相关信息

May 21, 2024

# 数据科学

# UCB Data100: Principles and Techniques of Data Science

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：Data8, CS61A，线性代数
- 编程语言：Python
- 课程难度：🌟🌟🌟
- 预计学时：80 小时

伯克利的数据科学入门课程，内容相对基础，覆盖了数据清洗、特征提取、数据可视化以及机器学习和推理的基础内容，也会讲授 Pandas, Numpy, Matplotlib 等数据科学常用工具。其丰富有趣的编程作业也是这门课的一大亮点。

## 课程资源

- 课程网站：https://ds100.org/
- 课程视频：参见课程网站
- 课程教材：https://www.textbook.ds100.org/intro.html
- 课程作业：参见课程网站

May 21, 2024

# 人工智能

# CS50’s Introduction to AI with Python

## 课程简介

- 所属大学：Harvard
- 先修要求：基本概率论 + Python 基础
- 编程语言：Python
- 课程难度：🌟🌟🌟
- 预计学时：30 小时

一门非常基础的 AI 入门课，让人眼前一亮的是 12 个设计精巧的编程作业，都会用学到的 AI 知识去实现一个简易的游戏 AI，比如用强化学习训练一个 Nim 游戏的 AI，用 alpha-beta 剪枝去扫雷等等，非常适合新手入门或者大佬休闲。

## 课程资源

- 课程网站：https://cs50.harvard.edu/ai/2020/
- 课程视频：https://cs50.harvard.edu/ai/2020/
- 课程教材：无
- 课程作业：https://cs50.harvard.edu/ai/2020/，12个精巧的编程作业

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/cs50_ai - GitHub](https://github.com/PKUFlyingPig/cs50_ai) 中。

May 21, 2024

# CS188: Introduction to Artificial Intelligence

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS70
- 编程语言：Python
- 课程难度：🌟🌟🌟
- 预计学时：50 小时

伯克利的人工智能入门课，课程 notes 写得非常深入浅出，基本不需要观看课程视频。课程内容的安排基本按照人工智能的经典教材 *Artificial intelligence: A Modern Approach* 的章节顺序，覆盖了搜索剪枝、约束满足问题、马尔可夫决策过程、强化学习、贝叶斯网络、隐马尔可夫模型以及基础的机器学习和神经网络的相关内容。

2018年秋季学期的版本免费开放了 gradescope，大家可以在线完成书面作业并实时得到测评结果。同时课程的 6 个 Project 也是质量爆炸，复现了经典的 Packman（吃豆人）小游戏，会让你利用学到的 AI 知识，去实现相关算法，让你的吃豆人在迷宫里自由穿梭，躲避鬼怪，收集豆子。

## 课程资源

- 课程网站：[Fall 2022](https://inst.eecs.berkeley.edu/~cs188/fa22/)，[Fall 2018](https://inst.eecs.berkeley.edu/~cs188/fa18/index.html)
- 课程视频：[Fall 2022](https://inst.eecs.berkeley.edu/~cs188/fa22/)，[Fall 2018](https://inst.eecs.berkeley.edu/~cs188/fa18/index.html)，每节课的链接详见课程网站
- 课程教材：Artificial intelligence: A Modern Approach
- 课程作业：在线测评书面作业和 Projects，详见课程网站

May 21, 2024

# 机器学习

# Coursera: Machine Learning

## 课程简介

- 所属大学：Stanford
- 先修要求：AI 入门 + 熟练使用 Python
- 编程语言：Python
- 课程难度：🌟🌟🌟
- 预计学时：100 小时

说起吴恩达，在 AI 届应该无人不晓。他是著名在线教育平台 [Coursera](https://www.coursera.org/) 的创始人之一，同时也是 Stanford 的网红教授。这门机器学习入门课应该算得上是他的成名作之一（另一个是深度学习课程），在 Coursera 上拥有数十万的学习者（注意这是花钱买了证书的人，一个证书几百刀），白嫖学习者数量应该是另一个数量级了。

这门课对新手极其友好，吴恩达拥有把机器学习讲成 1+1=2 一样直白的能力。你将会学习到线性回归、逻辑回归、支持向量机、无监督学习、降维、异常检测和推荐系统等等知识，并且在编程实践中夯实自己的理解。作业质量自然不必多言，保姆级代码框架，作业背景也多取自生活，让人学以致用。

当然，这门课作为一个公开慕课，难度上刻意放低了些，很多数学推导大多一带而过，如果你有志于从事机器学习理论研究，想要深究这些算法背后的数学理论，可以参考 [CS229](https://csdiy.wiki/机器学习/CS229/) 和 [CS189](https://csdiy.wiki/机器学习/CS189/)。

## 课程资源

- 课程网站：https://www.coursera.org/learn/machine-learning
- 课程视频：参见课程网站
- 课程教材：无
- 课程作业：参见课程网站

## 资源汇总

当时重装系统误删了文件，我的代码实现消失在了磁盘的 01 串中。不过这门课由于太过出名，网上想搜不到答案都难，相关课程资料 Coursera 上也一应俱全。

May 21, 2024

# CS229: Machine Learning

## 课程简介

- 所属大学：Stanford
- 先修要求：高数，概率论，Python，需要较深厚的数学功底
- 编程语言：无
- 课程难度：🌟🌟🌟🌟
- 预计学时：100 小时

同样是吴恩达讲授，但是这是一门研究生课程，所以更偏重数学理论，不满足于调包而想深入理解算法本质，或者有志于从事机器学习理论研究的同学可以学习这门课程。课程网站上提供了所有的课程 notes，写得非常专业且理论，需要一定的数学功底。

## 课程资源

- 课程网站：http://cs229.stanford.edu/syllabus.html
- 课程视频：https://www.bilibili.com/video/BV1JE411w7Ub
- 课程教材：无，课程 notes 写得非常好
- 课程作业：不对公众开放

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CS229 - GitHub](https://github.com/PKUFlyingPig/CS229) 中。

May 21, 2024

# CS189: Introduction to Machine Learning

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS188, CS70
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟
- 预计学时：100 小时

这门课我没有系统上过，只是把它的课程 notes 作为工具书查阅。不过从课程网站上来看，它比 CS229 好的是开源了所有 homework 的代码以及 gradescope 的 autograder。同样，这门课讲得相当理论且深入。

## 课程资源

- 课程网站：https://www.eecs189.org/
- 课程视频：https://www.youtube.com/playlist?list=PLOOm2AoWIPEyZazQVnIcaK2KnezpGZV-X
- 课程教材：https://www.eecs189.org/
- 课程作业：https://www.eecs189.org/

May 21, 2024

# 机器学习系统

# 智能计算系统

## 课程简介

- 所属大学：中国科学院大学
- 先修要求：体系结构，深度学习
- 编程语言：Python, C++, BCL
- 课程难度：🌟🌟🌟
- 预计学时：100 小时+

智能计算系统是智能的核心物质载体，每年全球要制造数以十亿计的智能计算系统（包括智能手机、智能服务器、智能可穿戴设备等），需要大量的智能计算系统的设计者和开发者。智能计算系统人才的培养直接关系到我国智能产业的核心竞争力。因此，对智能计算系统的认识和理解是智能时代计算机类专业学生培养方案中不可或缺的重要组成部分，是计算机类专业学生的核心竞争力。

国内的陈云霁老师开的课，在其他若干个大学也都有开对应的课程。这门课用一个个实验带大家以一个完整的视野理解人工智能的技术栈。从上层的深度学习框架，到用底层语言编写算子，再到硬件中 MLU 的设计，让大家形成系统思维，体会自上而下，融会贯通的乐趣。

我做了其中的 2,3,4,5 这几个实验，其中综合实验和硬件实验没有做，如果有做了的同学欢迎大家补上你的链接。

个人体会是第三章实现算子的实验让我对深度学习框架的了解加深了很多。第五章的实验BCL语言编写算子如果了解 CUDA 的话会感觉很熟悉。

推荐去买一本教材看一看，会让我们理解整体的技术栈。熟悉深度学习的同学可以直接从第五章开始看，看看深度学习框架底层到底是什么样的。

我因为这门课的启发，参考一本书（书名在仓库中）写了一个简易的[深度学习框架](https://github.com/ysj1173886760/PyToy)。在这个框架里可以看到智能计算系统实验中的一些影子。同时受到 build-your-own-x 系列的启发，我也打算写一下教程，教大家写一个自己的深度学习框架。代码用 Python 写的，代码量较少，适合有一定基础的同学阅读。之后打算添加更多的算子，有望实现一个较为全面的框架，并希望移植到 C++ 中，以兼顾性能与开发效率。

## 课程资源

- 课程网站：[官网](https://novel.ict.ac.cn/aics/)
- 课程视频：[bilibili](https://space.bilibili.com/494117284)
- 课程教材：智能计算系统（陈云霁）

## 资源汇总

### 2024年新版实验

- 2024 年的智能计算系统实验内容对知识体系、实验题目及实验手册进行了大范围的调整，调整内容包括全面使用 PyTorch ，不再使用 TensorFlow 以及添加大模型相关实验等。
- 由于新版实验题目及实验手册未在寒武纪论坛进行更新，因此提供以下存储仓库，用于存储新版智能计算系统的实验题目、实验手册以及个人的实验答案
- 新版实验的资源跟随国科大 2024 年春季学期的课程进度进行更新，预计 2024 年 6 月更新完毕
- @Yuichi 编写的 2024 新版实验题目、手册及答案：https://github.com/Yuichi1001/2024-AICS-EXP

### 旧版实验

- 旧版课程作业：6 个实验(包括编写卷积算子，为 TensorFlow 添加算子，用 BCL 编写算子并集成到 TensorFlow 中等)(具体内容在官网可以找到)
- 旧版实验手册：[实验 2.0 指导手册](https://forum.cambricon.com/index.php?m=content&c=index&a=show&catid=155&id=708)
- 学习笔记：https://sanzo.top/categories/AI-Computing-Systems/，参考实验手册总结的笔记(已失效)
- @ysj1173886760 在学习这门课中用到的所有资源和作业实现都汇总在 [ysj1173886760/Learning: ai-system - GitHub](https://github.com/ysj1173886760/Learning/tree/master/ai-system) 中。

May 21, 2024

# CMU 10-414/714: Deep Learning Systems

## 课程简介

- 所属大学：CMU
- 先修要求：系统入门(eg.15-213)、深度学习入门、基本的数学知识
- 编程语言：Python, C++
- 课程难度：🌟🌟🌟
- 预计学时：100小时

深度学习的快速发展和广泛使用很大程度上得益于一系列简单好用且强大的编程框架，例如 Pytorch 和 Tensorflow 等等。但大多数从业者只是这些框架的“调包侠”，对于这些框架内部的细节实现却了解甚少。如果你希望从事深度学习底层框架的开发，或者只是像我一样好奇这些框架的内部实现，那么这门课将会是一个很好的起点。

课程的内容大纲覆盖了深度学习系统“全栈”的知识体系。从现代深度学习系统框架的顶层设计，到自微分算法的原理和实现，再到底层硬件加速和实际生产部署。为了更好地掌握理论知识，学生将会在5个课程作业中从头开始设计和实现一个完整的深度学习库 Needle，使其能对计算图进行自动微分，能在 GPU 上实现硬件加速，并且支持各类损失函数、数据加载器和优化器。在此基础上，学生将实现几类常见的神经网络，包括 CNN，RNN，LSTM，Transformer 等等。

即使你是深度学习领域的小白也不必过于担心，课程将会循序渐进地从简单分类问题和反向传播优化讲起，一些相对复杂的神经网络都会有配套的 jupyter notebook 详细地描述实现细节。如果你有一定的相关基础知识，那么在学习完自微分部分的内容之后便可以直接上手课程作业，难度虽然不大但相信一定会给你带来新的理解。

这门课两位授课教师 [Zico Kolter](https://zicokolter.com/) 和 [Tianqi Chen](https://tqchen.com/) 将所有课程内容都发布了对应的开源版本，但在线评测账号和课程论坛的注册时间已经结束，只剩下框架代码里的本地测试供大家调试代码。或许可以期待明年秋季学期的课程还会发布相应的在线版本供大家学习。

## 课程资源

- 课程网站：[https://dlsyscourse.org](https://dlsyscourse.org/)
- 课程视频：https://www.youtube.com/watch?v=qbJqOFMyIwg
- 课程作业：https://dlsyscourse.org/assignments/

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CMU10-714 - GitHub](https://github.com/PKUFlyingPig/CMU10-714) 中。

May 21, 2024CMU 10-414/714: Deep Learning Systems

## 课程简介

- 所属大学：CMU
- 先修要求：系统入门(eg.15-213)、深度学习入门、基本的数学知识
- 编程语言：Python, C++
- 课程难度：🌟🌟🌟
- 预计学时：100小时

深度学习的快速发展和广泛使用很大程度上得益于一系列简单好用且强大的编程框架，例如 Pytorch 和 Tensorflow 等等。但大多数从业者只是这些框架的“调包侠”，对于这些框架内部的细节实现却了解甚少。如果你希望从事深度学习底层框架的开发，或者只是像我一样好奇这些框架的内部实现，那么这门课将会是一个很好的起点。

课程的内容大纲覆盖了深度学习系统“全栈”的知识体系。从现代深度学习系统框架的顶层设计，到自微分算法的原理和实现，再到底层硬件加速和实际生产部署。为了更好地掌握理论知识，学生将会在5个课程作业中从头开始设计和实现一个完整的深度学习库 Needle，使其能对计算图进行自动微分，能在 GPU 上实现硬件加速，并且支持各类损失函数、数据加载器和优化器。在此基础上，学生将实现几类常见的神经网络，包括 CNN，RNN，LSTM，Transformer 等等。

即使你是深度学习领域的小白也不必过于担心，课程将会循序渐进地从简单分类问题和反向传播优化讲起，一些相对复杂的神经网络都会有配套的 jupyter notebook 详细地描述实现细节。如果你有一定的相关基础知识，那么在学习完自微分部分的内容之后便可以直接上手课程作业，难度虽然不大但相信一定会给你带来新的理解。

这门课两位授课教师 [Zico Kolter](https://zicokolter.com/) 和 [Tianqi Chen](https://tqchen.com/) 将所有课程内容都发布了对应的开源版本，但在线评测账号和课程论坛的注册时间已经结束，只剩下框架代码里的本地测试供大家调试代码。或许可以期待明年秋季学期的课程还会发布相应的在线版本供大家学习。

## 课程资源

- 课程网站：[https://dlsyscourse.org](https://dlsyscourse.org/)
- 课程视频：https://www.youtube.com/watch?v=qbJqOFMyIwg
- 课程作业：https://dlsyscourse.org/assignments/

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CMU10-714 - GitHub](https://github.com/PKUFlyingPig/CMU10-714) 中。

May 21, 2024

# Machine Learning Compilation

## 课程简介

- 所属大学：Bilibili 大学
- 先修要求：机器学习/深度学习基础
- 编程语言：Python
- 课程难度：🌟🌟🌟
- 预计学时：30小时

这门课是机器学习编译领域的顶尖学者陈天奇在2022年暑期开设的一门在线课程。其实机器学习编译无论在工业界还是学术界仍然是一个非常前沿且快速更迭的领域，国内外此前还没有为这个方向专门开设的相关课程。因此如果对机器学习编译感兴趣想有个全貌性的感知的话，可以学习一下这门课。

本课程主要以 [Apache TVM](https://tvm.apache.org/) 这一主流的机器学习编译框架为例（陈天奇是这个框架的创始人之一），聚焦于如何将开发模式下（如 Tensorflow, Pytorch, Jax）的各类机器学习模型，通过一套普适的抽象和优化算法，变换为拥有更高性能并且适配各类底层硬件的部署模式。课程讲授的知识点都是相对 High-Level 的宏观概念，同时每节课都会有一个配套的 Jupyter Notebook 来通过具体的代码讲解知识点，因此如果从事 TVM 相关的编程开发的话，这门课有丰富且规范的代码示例以供参考。

所有的课程资源全部开源并且有中文和英文两个版本，B站和油管分别有中文和英文的课程录影。

## 课程资源

- 课程网站：https://mlc.ai/summer22-zh/
- 课程视频：[Bilibili](https://www.bilibili.com/video/BV15v4y1g7EU?spm_id_from=333.337.search-card.all.click&vd_source=a4d76d1247665a7e7bec15d15fd12349)
- 课程笔记：https://mlc.ai/zh/index.html
- 课程作业：https://github.com/mlc-ai/notebooks/blob/main/assignment

May 21, 2024

# 深度学习

# UMich EECS 498-007 / 598-005: Deep Learning for Computer Vision

## 课程简介

- 所属大学：UMich
- 先修要求：Python基础，矩阵论(熟悉矩阵求导即可)，微积分
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟
- 预计学时：60～80 小时

UMich 的 Computer Vision 课，课程视频和作业质量极高，涵盖的主题非常全，同时 Assignments 的难度由浅及深，覆盖了 CV 主流模型发展的全阶段，是一门非常好的 Computer Vision 入门课。

你在每个 Assignment 里会跟随 Handouts 搭建与训练 Lectures 中提到的模型/框架。

你不需要有任何的深度学习框架的使用经验，在开始的 Assignment 里，这门课会从零开始教导每个学生如何使用 Pytorch，后续也可以当成工具书，随时翻阅。

同时由于每个 Assignment 之间涉及到的主题都不同，你在递进式的 Assignment 中不仅可以亲身体会到 CV 主流模型的发展历程，领略到不同的模型和训练的方法对最终效果/准确率的影响，同时也能 Hands On 地实现它们。

在 A1 中，你会学习 Pytorch 和 Google Colab 的使用。

在 A2 中你会亲自搭建 Linear Classifier 以及一个两层的神经网络，最后你有机会亲自接触 MNIST 数据集并在此基础上训练并评估你搭建起的神经网络。

在 A3 中，你会接触到最为经典的 Convolutional Neural Network (A.K.A. CNN)，亲自感受卷积神经网络的魅力。

而在 A4 中，你将实际触及搭建物体检测模型的全流程，同时跟随 Handout 实现两篇论文中的 One-Stage Detector 和 Two-Stage Detector。

到了 A5，就是从 CNN 到 RNN 的时刻了，你将有机会亲自搭建起两种不同的基于注意力的模型，RNNs (Vanilla RNN & LSTM) 和大名鼎鼎的 Transfomer。

在最后一个 Assignment（A6）中，你将有机会实现两种更为 Fancy 的模型，VAE 和 GAN，并应用在 MINST 数据集上。最后，你会实现网络可视化和风格迁移这两个非常酷炫的功能。

在 Assignments 之外，你还可以自己实现一个 Mini-Project，亲自搭建起一个完整的深度学习 Pipeline，具体可以参考课程主页。

课程所涉及的资源，如 Lectures/Notes/Assignments 都是开源的，美中不足的是 Autograder 只对本校 Enrolled 的学生开放，但因为在提供的 `*.ipynb`（也就是 Handout） 中已经可以确定实现的正确性，以及预期的结果，所以我个人觉得 Autograder 的缺失没有任何影响。

值得一提的是，这门课的主讲教授 Justin Johnson 正是 Fei-Fei Li 的博士毕业生，现在在 UMich 当 Assistant Professor。

而现在开源的 2017 年版本的 Stanford CS231N 的主讲人就是 Justin Johnson。

同时因为 CS231N 主要是由 Justin Johnson 和 Andrej Karpathy 建设起来的，这门课也沿用了 CS231N 的一些材料，所以学过 CS231N 的同学可能会觉得这门课的某些材料比较熟悉。

最后，我推荐每一个 Enroll 这门课的同学都去看一看 Youtube 上面的 Lectures，Justin Johnson 的讲课方式和内容都非常清晰和易懂，是非常棒的参考。

## 课程资源

- 课程网站：https://web.eecs.umich.edu/~justincj/teaching/eecs498/WI2022/
- 课程视频：https://www.youtube.com/playlist?list=PL5-TkQAfAZFbzxjBHtzdVCWE0Zbhomg7r
- 课程教材：仅有推荐教材，链接：https://www.deeplearningbook.org/
- 课程作业：见课程主页，6 个 Assignment 和一个 Mini-Project

## 资源汇总

@Michael-Jetson 本人所做的二三十万字的笔记（并没有包括作业等），可以当做一个参考[Michael-Jetson/ML_DL_CV_with_pytorch](https://github.com/Michael-Jetson/ML_DL_CV_with_pytorch)

May 21, 2024

# Coursera: Deep Learning

## 课程简介

- 所属大学：Stanford
- 先修要求：机器学习基础 + Python
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟
- 预计学时：80 小时

吴恩达在 Coursera 开设的另一门网红课程，学习者无数，堪称圣经级的深度学习入门课。深入浅出的讲解，眼花缭乱的 Project。从最基础的神经网络，到 CNN, RNN，再到最近大热的 Transformer。学完这门课，你将初步掌握深度学习领域必备的知识和技能，并且可以在 [Kaggle](https://www.kaggle.com/) 中参加自己感兴趣的比赛，在实践中锻炼自己。

## 课程资源

- 课程网站：https://www.coursera.org/specializations/deep-learning
- 课程视频：https://www.coursera.org/specializations/deep-learning，B站有搬运
- 课程教材：无
- 课程作业：https://www.coursera.org/specializations/deep-learning

May 21, 2024

# 国立台湾大学：李宏毅机器学习

## 课程简介

- 所属大学：國立台灣大學
- 先修要求：熟练掌握 Python
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟
- 预计学时：80 小时

李宏毅老师是国立台湾大学的教授，其风趣幽默的授课风格深受大家喜爱，并且尤其喜欢在 PPT 中插入宝可梦等动漫元素，是个非常可爱的老师。

这门课挂着机器学习的牌子，但其课程内容之广实在令人咋舌，其作业一共包含 15 个 lab，分别是 Regression、Classification、CNN、Self-Attention、Transformer、GAN、BERT、Anomaly Detection、Explainable AI、Attack、Adaptation、 RL、Compression、Life-Long Learning 以及 Meta Learning。可谓是包罗万象，能让学生对于深度学习的绝大多数领域都有一定了解，从而可以进一步选择想要深入的方向进行学习。

大家也大可不必担心作业的难度，因为所有作业都会提供助教的示例代码，帮你完成数据处理、模型搭建等，你只需要在其基础上进行适量的修改即可。这也是一个学习别人优质代码的极好机会，大家需要水课程大作业的话，这里也是一个不错的资料来源。

## 课程资源

- 课程网站：https://speech.ee.ntu.edu.tw/~hylee/ml/2022-spring.php
- 课程视频：https://speech.ee.ntu.edu.tw/~hylee/ml/2022-spring.php，每节课的链接参见课程网站
- 课程教材：无
- 课程作业：https://speech.ee.ntu.edu.tw/~hylee/ml/2022-spring.php，15 个 lab，几乎覆盖了主流深度学习的所有领域

May 21, 2024

# CS231n: CNN for Visual Recognition

## 课程简介

- 所属大学：Stanford
- 先修要求：机器学习基础
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟
- 预计学时：80 小时

Stanford 的 CV 入门课，由计算机领域的巨佬李飞飞院士领衔教授（CV 领域划时代的著名数据集 ImageNet 的研究团队），但其内容相对基础且友好，如果上过 CS230 的话可以直接上手 Project 作为练习。

## 课程资源

- 课程网站：http://cs231n.stanford.edu/
- 课程视频：https://www.bilibili.com/video/BV1nJ411z7fe
- 课程教材：无
- 课程作业：http://cs231n.stanford.edu/schedule.html，3个编程作业

May 21, 2024

# CS224n: Natural Language Processing

## 课程简介

- 所属大学：Stanford
- 先修要求：深度学习基础 + Python
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟
- 预计学时：80 小时

Stanford 的 NLP 入门课程，由自然语言处理领域的巨佬 Chris Manning 领衔教授（word2vec 算法的开创者）。内容覆盖了词向量、RNN、LSTM、Seq2Seq 模型、机器翻译、注意力机制、Transformer 等等 NLP 领域的核心知识点。

5 个编程作业难度循序渐进，分别是词向量、word2vec 算法、Dependency parsing、机器翻译以及 Transformer 的 fine-tune。

最终的大作业是在 Stanford 著名的 SQuAD 数据集上训练 QA 模型，有学生的大作业甚至直接发表了顶会论文。

## 课程资源

- 课程网站：http://web.stanford.edu/class/cs224n/index.html
- 课程视频：B 站搜索 CS224n
- 课程教材：无
- 课程作业：http://web.stanford.edu/class/cs224n/index.html，5 个编程作业 + 1 个 Final Project

## 资源汇总

@PKUFlyingPig 在学习这门课中用到的所有资源和作业实现都汇总在 [PKUFlyingPig/CS224n - GitHub](https://github.com/PKUFlyingPig/CS224n) 中。

May 21, 2024

# CS285: Deep Reinforcement Learning

## 课程简介

- 所属大学：UC Berkeley
- 先修要求：CS188, CS189
- 编程语言：Python
- 课程难度：🌟🌟🌟🌟
- 预计学时：80 小时

CS285 这一课程现由 Sergey Levine 教授讲授，课程内容覆盖了深度强化学习领域的各方面内容，适合有一定机器学习基础的同学进行学习，具体要求包括了解马尔可夫决策过程（MDP）等。整门课程中含有较多的公式，上课前需要有一定的心理准备。此外，教授会根据每年最新的研究进展更新课程内容以及作业，课程中能感受到教授尝试将深度强化学习领域的所有基础知识以及最近的发展在短短的数节课中进行传达。

有关课程内容获取，22Fall 的授课方式为课前观看提前录制的视频，课上主要为 Q&A 环节，教授选择部分或者所有视频内的知识进行讲解同时回答学生现场提出的问题，因此所提供的课程视频链接实际上是已经包含了所有内容。课程作业则由5个编程作业组成，每一次作业主要为复现经典模型以及进行模型间的对比，偶尔也包含一些对最近提出的模型的复现，最后递交一份报告。考虑到作业本身已经提供了框架，且都是根据 hint 进行代码填空，因此作业难度并不大。

总的来说，该课程适合新手入门深度强化学习。虽然学到后面越来越感觉到难，但整门课下来个人感觉还是收获颇丰。

（另外 Levine 教授人真的很 nice）

## 课程资源

- 课程网站：http://rail.eecs.berkeley.edu/deeprlcourse/
- 课程视频：https://www.youtube.com/playlist?list=PL_iWQOsE6TfX7MaC6C3HcdOf1g337dlC9
- 课程教材：无
- 课程作业：http://rail.eecs.berkeley.edu/deeprlcourse/，5个编程作业

May 21, 2024

# 机器学习进阶

# 机器学习进阶

此路线图适用于已经学过了基础机器学习 (ML, NLP, CV, RL) 的同学 (高年级本科生或低年级研究生)，已经发表过至少一篇顶会论文 (NeurIPS, ICML, ICLR, ACL, EMNLP, NAACL, CVPR, ICCV) 想要走机器学习科研路线的选手。

此路线的目标是为读懂与发表机器学习顶会论文打下理论基础，特别是 Probabilistic Methods 这个 track 下的文章。

机器学习进阶可能存在多种不同的学习路线，此路线只能代表作者 [Yao Fu](https://franxyao.github.io/) 所理解的最佳路径，侧重于贝叶斯学派下的概率建模方法，也会涉及到各项相关学科的交叉知识。

## 必读教材

- PRML: Pattern Recognition and Machine Learning. Christopher Bishop
- AoS: All of Statistics. Larry Wasserman

这两本书分别是经典贝叶斯学派和经典频率学派的教材，刚好相辅相成。

## 字典

- MLAPP: Machine Learning: A Probabilistic Perspective. Kevin Murphy
- Convex Optimization. Stephen Boyd and Lieven Vandenberghe

## 进阶书籍

- W&J: Graphical Models, Exponential Families, and Variational Inference. Martin Wainwright and Michael Jordan
- Theory of Point Estimation. E. L. Lehmann and George Casella

## 如何阅读

### Guidelines

- 必读教材就是一定要读的教材
- 字典的意思是，一般情况下不管它，但当遇到了不懂的概念的时候，就去字典里面查（而不是维基百科）
- 进阶书籍先不读，先读完必读书籍。必读书籍一般都是要前前后后反复看过 N 遍才算读完
- 读的过程中，最重要的读法就是对比阅读 (contrastive-comparative reading)：同时打开两本书讲同一主题的章节，然后对比相同点和不同点和联系
- 读的过程中，尽量去回想之前读过的论文，比较论文和教材的相同点与不同点

### 基础路径

- 先读 AoS 第六章: Models, Statistical Inference and Learning，这一部分是最基础的科普
- 然后读 PRML 第 10, 11 章
- 第 10 章的内容是 Variational Inference, 第 11 章的内容是 MCMC, 这两种方法是贝叶斯推断的两条最主要路线
- 如果在读 PRML 的过程中发现有任何不懂的名词，就去翻前面的章节。很大概率能够在第 3，4 章找到相对应的定义；如果找不到或者不够详细，就去查 MLAPP
- AoS 第 8 章 (Parametric Inference) 和第 11 章 (Bayesian Inference) 也可以作为参考。最好的方法是多本书对比阅读，流程如下
  - 假设我在读 PRML 第 10 章的时候发现了一个不懂的词：posterior inference
  - 于是我往前翻，翻到了第 3 章 (Linear Model for Regression)，看到了最简单的 posterior
  - 然后我接着翻 AoS，翻到了第 11 章，也有对 posterior 的描述
  - 然后我对比 PRML 第 10 章，第 3 章，AoS 第 11 章，三处不同地方对 posterior 的解读，比较其相同点和不同点和联系
- 读完 PRML 第 10 和 11 章之后，接着读 AoS 第 24 章 (Simulation Methods)，然后把它和 PRML 第 11 章对比阅读 -- 这俩都是讲 MCMC
- 如果到此处发现还有基础概念读不懂，就回到 PRML 第 3 章，把它和 AoS 第 11 章对比阅读
- Again，对比阅读非常重要，一定要把不同本书的类似内容同时摆在面前相互对比，这样可以显著增强记忆
- 然后读 PRML 第 13 章（跳过第 12 章），这一章可以和 MLAPP 的第 17, 18 章对比阅读
- MLAPP 第 17 章是 PRML 第 13.2 章的详细版，主要讲 HMM
- MLAPP 第 18 章是 PRML 第 13.3 章的详细版，主要讲 LDS
- 读完 PRML 第 13 章之后，再去读 PRML 第 8 章 (Graphical Models) -- 此时这部分应该会读得很轻松
- 以上的内容可以进一步对照 CMU 10-708 PGM 课程材料

到目前为止，应该能够掌握

- 概率模型的基础定义
- 精准推断 - Sum-Product
- 近似推断 - MCMC
- 近似推断 - VI

然后就可以去做更进阶的内容

May 21, 2024

# CMU 10-708: Probabilistic Graphical Models

## 课程简介

- 所属大学：CMU
- 先修要求：Machine Learning, Deep Learning, Reinforcement Learning
- 课程难度：🌟🌟🌟🌟🌟
- 课程网站：https://sailinglab.github.io/pgm-spring-2019/
- 课程网站包含了所有的资源：slides, notes, video, homework, and project

这门课程是 CMU 的图模型基础 + 进阶课，授课老师为 Eric P. Xing，涵盖了图模型基础，与神经网络的结合，在强化学习中的应用，以及非参数方法，相当硬核。

May 21, 2024

# Columbia STAT 8201: Deep Generative Models

## 课程简介

- 所属大学：Columbia University
- 先修要求：Machine Learning, Deep Learning, Graphical Models
- 课程难度：🌟🌟🌟🌟🌟🌟
- 课程网站：http://stat.columbia.edu/~cunningham/teaching/GR8201/

这门课是一门 PhD 讨论班，每周的内容是展示 + 讨论论文，授课老师是 John Cunningham。Deep Generative Models （深度生成模型） 是图模型与神经网络的结合，也是现代机器学习最重要的方向之一。

May 21, 2024

# STA 4273 Winter 2021: Minimizing Expectations

## 课程简介

- 所属大学：U Toronto
- 先修要求：Bayesian Inference, Reinforcement Learning
- 课程难度：🌟🌟🌟🌟🌟🌟🌟
- 课程网站：https://www.cs.toronto.edu/~cmaddis/courses/sta4273_w21/

这是一门较为进阶的 Ph.D. 研究课程，核心内容是 inference 和 control 之间的关系。授课老师为 Chris Maddison (AlphaGo founding member, NeurIPS 14 best paper)。

May 21, 2024

# STATS214 / CS229M: Machine Learning Theory

## 课程简介

- 所属大学：Stanford
- 先修要求：Machine Learning, Deep Learning, Statistics
- 课程难度：🌟🌟🌟🌟🌟🌟
- 课程网站：http://web.stanford.edu/class/stats214/

经典学习理论 + 最新深度学习理论，非常硬核。授课老师之前是 Percy Liang，现在是 Tengyu Ma。

May 21, 2024

# 后记

从最初的想法开始，到断断续续完成这本书，再到树洞的热烈反响，我很激动，但也五味杂陈。原来在北大这个园子里，也有那么多人，对自己的本科生涯并不满意。而这里，可是囊括了中国非常优秀的一帮年轻人。所以问题出在哪里？我不知道。

我只是个籍籍无名的本科生呀，只是一个单纯的求学者，我的目标只是想快乐地、自由地、高质量地掌握那些专业知识，我想，正在看这本书的大多数本科生也是如此，谁想付出时间但却收效甚微呢？又是谁迫使大家带着痛苦去应付呢？我不知道。

我写这本书绝不是为了鼓励大家翘课自学，试问谁不想在课堂上和那么多优秀的同学济济一堂，热烈讨论呢？谁不想遇到问题直接找老师答疑解惑呢？谁不想辛苦学习的成果可以直接化作学校承认的学分绩点呢？可如果一个兢兢业业、按时到堂的学生收获的却是痛苦，而那个一学期只有考试会出席的学生却学得自得其乐，这公平吗？我不知道。

我只是不甘，不甘心这些通过高考战胜无数人进入高校的学子本可以收获一个更快乐的本科生涯，但现实却留给了他们遗憾。我反问自己，本科教育究竟应该带给我们什么呢？是学完所有这些课程吗？倒也未必，它也许只适合我这种nerd。但我觉得，本科教育至少得展现它应有的诚意，一种分享知识的诚意，一种以人为本的诚意，一种注重学生体验的诚意。它至少不应该是一种恶意，一种拼比知识的恶意，一种胜者为王的恶意，一种让人学无所得的恶意。但这一切能改变吗？我不知道。

我只知道我做了应该做的事情，学生们会用脚投票，树洞的关注量和回帖数证明了这样一份资料是有价值的，也道出了国内CS本科教育和国外的差距。也许这样的改变是微乎其微的，但别忘了我只是一个籍籍无名的本科生，是北大信科一千多名本科生中的普通一员，是中国几百万在读本科生中的一分子，如果有更多的人站出来，每个人做一点点，也许是分享一个帖子，也许是当一门课的助教，也许是精心设计一门课的lab，更或许是将来获得教职之后开设一门高质量的课程，出版一本经典的教材。本科教育真的有什么技术壁垒吗？我看未必，教育靠的是诚意，靠的是育人之心。

今天是2021年12月12日，我期待在不久的将来这个帖子会被遗忘，大家可以满心欢喜地选着自己培养方案上的课程，做着学校自行设计的各类编程实验，课堂没有签到也能济济一堂，学生踊跃地发言互动，大家的收获可以和努力成正比，那些曾经的遗憾和痛苦可以永远成为历史。我真的很期待那一天，真的真的真的很期待。

PKUFlyingPig

2021年12月12日写于燕园

May 21, 2024

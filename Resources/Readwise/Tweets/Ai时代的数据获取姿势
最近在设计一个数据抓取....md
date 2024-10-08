# Ai时代的数据获取姿势
最近在设计一个数据抓取...

![rw-book-cover](https://pbs.twimg.com/profile_images/1511108233695432707/TOvN835h.jpg)

## Metadata
- Author: [[@StephanCptMax on Twitter]]
- Full Title: Ai时代的数据获取姿势
最近在设计一个数据抓取...
- Category: #tweets
- URL: https://twitter.com/StephanCptMax/status/1640024916274872320

## Highlights
- AI时代的数据获取姿势
  最近在设计一个数据抓取的模块，意识到其实传统的结构化数据抓取方式，在AI时代已经不太需要了。这可能也是AI给程序员带来的一大效率提升👇🧵 
  ![](https://pbs.twimg.com/media/FsJ0eRSagAMIPC_.jpg) ([View Tweet](https://twitter.com/StephanCptMax/status/1640024916274872320))
- 传统的抓取方法，一般要考虑网站的结构、元素的位置，正则、xpath、DOM树解析这种都是需要考虑网站结构的。这种抓取的一大缺点就是需要定制化和大量的数据清洗工作。网站结构稍微一变就抓不到数据了，而且不同网站的结构千差万别，维护工作就变得异常复杂和无聊。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024919013748738))
- 现在AI时代就完全不需要这样抓数据了，爬虫只需要设计两部分：
  1. 整站链接的递归抓取，这个跟网站内容无关，只需要把同域名下的url全部抓下来，做成一个树状结构保存下来（如果网站有提供完整的sitemap的话这一步都可以省掉）。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024921001832448))
- 2. 针对每个url，用NLP语义抽取的方式，把网页中所有正文内容抓下来。因为是NLP语义的角度去抓取正文，所以这个过程我不需要考虑网页的元素位置。抓下来的内容就直接是正文内容，NLP会帮你把所有图片、导航、广告等跟正文无关的信息全部过滤掉。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024922901843974))
- 其中，NLP语义抽取引擎选型上，我问了GPT4给出如下几个建议： 
  ![](https://pbs.twimg.com/media/FsJ9MSPacAEsTag.jpg) ([View Tweet](https://twitter.com/StephanCptMax/status/1640024924940304384))
- 我尝试用了下Dragnet，效果看起来还不错。但要注意它只能支持到最高python3.7的版本，再高版本的话安装会报错。
  以下是原网页的部分内容和他提取的内容： 
  ![](https://pbs.twimg.com/media/FsKBxgwaYAApe7p.jpg) 
  ![](https://pbs.twimg.com/media/FsKCN6baUAA8sWv.png) ([View Tweet](https://twitter.com/StephanCptMax/status/1640024927708368903))
- 其实这种NLP的抓取方式，好多年前就有。那么为什么以前用的不是很多呢（至少没有大规模流行起来）？
  是因为以前的人机交互方式，决定了数据必须是结构化的，而未来的人机交互方式变了。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024932561354753))
- AI时代到来后，人与机器沟通的方式已经从繁琐的点击、筛选、下达指令的方式，变为直接可以下达指令的方式了。现有的UI交互形式也会跟着变，数据也不再需要结构化良好的数据，半结构化甚至非结构化的数据，扔给AI就行。它能读懂，并根据你的需求筛选、推理、给出结果。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024934473924609))
- 这样一来，获取数据的成本下降，效率大幅提升。而且这还只是我昨晚刚做的一个最简单的尝试，试想一下，完全可以用AI来进一步辅助信息的抽取和预处理过程，比如文本聚类、情感分析、关键词提取、摘要总结等等。等到多模态成熟后，图文视频声音这些语料信息，直接扔给AI让它来整理就好。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024936378167296))
- 附上上文中例子的源码，跟NLP信息抽取相关的，只需要一行代码😆 
  ![](https://pbs.twimg.com/media/FsKKywqaYAEyTFu.jpg) ([View Tweet](https://twitter.com/StephanCptMax/status/1640026171713929217))
- 再来一个表格比较一下同类的各种库，数据仅供参考（GPT4的数据较老），实际使用还是要自己调研清楚哈： 
  ![](https://pbs.twimg.com/media/FsLHNkvaEAANhDU.jpg) ([View Tweet](https://twitter.com/StephanCptMax/status/1640092280290963456))
# Ai时代的数据获取姿势
最近在设计一个数据抓取...

![rw-book-cover](https://pbs.twimg.com/profile_images/1511108233695432707/TOvN835h.jpg)

## Metadata
- Author: [[@StephanCptMax on Twitter]]
- Full Title: Ai时代的数据获取姿势
最近在设计一个数据抓取...
- Category: #tweets
- URL: https://twitter.com/StephanCptMax/status/1640024916274872320

## Highlights
- AI时代的数据获取姿势
  最近在设计一个数据抓取的模块，意识到其实传统的结构化数据抓取方式，在AI时代已经不太需要了。这可能也是AI给程序员带来的一大效率提升👇🧵 
  ![](https://pbs.twimg.com/media/FsJ0eRSagAMIPC_.jpg) ([View Tweet](https://twitter.com/StephanCptMax/status/1640024916274872320))
- 传统的抓取方法，一般要考虑网站的结构、元素的位置，正则、xpath、DOM树解析这种都是需要考虑网站结构的。这种抓取的一大缺点就是需要定制化和大量的数据清洗工作。网站结构稍微一变就抓不到数据了，而且不同网站的结构千差万别，维护工作就变得异常复杂和无聊。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024919013748738))
- 现在AI时代就完全不需要这样抓数据了，爬虫只需要设计两部分：
  1. 整站链接的递归抓取，这个跟网站内容无关，只需要把同域名下的url全部抓下来，做成一个树状结构保存下来（如果网站有提供完整的sitemap的话这一步都可以省掉）。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024921001832448))
- 2. 针对每个url，用NLP语义抽取的方式，把网页中所有正文内容抓下来。因为是NLP语义的角度去抓取正文，所以这个过程我不需要考虑网页的元素位置。抓下来的内容就直接是正文内容，NLP会帮你把所有图片、导航、广告等跟正文无关的信息全部过滤掉。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024922901843974))
- 其中，NLP语义抽取引擎选型上，我问了GPT4给出如下几个建议： 
  ![](https://pbs.twimg.com/media/FsJ9MSPacAEsTag.jpg) ([View Tweet](https://twitter.com/StephanCptMax/status/1640024924940304384))
- 我尝试用了下Dragnet，效果看起来还不错。但要注意它只能支持到最高python3.7的版本，再高版本的话安装会报错。
  以下是原网页的部分内容和他提取的内容： 
  ![](https://pbs.twimg.com/media/FsKBxgwaYAApe7p.jpg) 
  ![](https://pbs.twimg.com/media/FsKCN6baUAA8sWv.png) ([View Tweet](https://twitter.com/StephanCptMax/status/1640024927708368903))
- 其实这种NLP的抓取方式，好多年前就有。那么为什么以前用的不是很多呢（至少没有大规模流行起来）？
  是因为以前的人机交互方式，决定了数据必须是结构化的，而未来的人机交互方式变了。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024932561354753))
- AI时代到来后，人与机器沟通的方式已经从繁琐的点击、筛选、下达指令的方式，变为直接可以下达指令的方式了。现有的UI交互形式也会跟着变，数据也不再需要结构化良好的数据，半结构化甚至非结构化的数据，扔给AI就行。它能读懂，并根据你的需求筛选、推理、给出结果。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024934473924609))
- 这样一来，获取数据的成本下降，效率大幅提升。而且这还只是我昨晚刚做的一个最简单的尝试，试想一下，完全可以用AI来进一步辅助信息的抽取和预处理过程，比如文本聚类、情感分析、关键词提取、摘要总结等等。等到多模态成熟后，图文视频声音这些语料信息，直接扔给AI让它来整理就好。 ([View Tweet](https://twitter.com/StephanCptMax/status/1640024936378167296))
- 附上上文中例子的源码，跟NLP信息抽取相关的，只需要一行代码😆 
  ![](https://pbs.twimg.com/media/FsKKywqaYAEyTFu.jpg) ([View Tweet](https://twitter.com/StephanCptMax/status/1640026171713929217))
- 再来一个表格比较一下同类的各种库，数据仅供参考（GPT4的数据较老），实际使用还是要自己调研清楚哈： 
  ![](https://pbs.twimg.com/media/FsLHNkvaEAANhDU.jpg) ([View Tweet](https://twitter.com/StephanCptMax/status/1640092280290963456))

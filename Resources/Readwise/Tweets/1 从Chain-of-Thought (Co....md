# 1/ 从Chain-of-Thought (Co...

![rw-book-cover](https://pbs.twimg.com/profile_images/1555109458073747457/JANhY5Zh.jpg)

## Metadata
- Author: [[@realrenmin on Twitter]]
- Full Title: 1/ 从Chain-of-Thought (Co...
- Category: #tweets
- URL: https://twitter.com/realrenmin/status/1643241565031366657

## Highlights
- 1/ 从Chain-of-Thought (CoT) 到 Let's think step by step
  最近每天都可以看到大语言模型进展的文章，LLM的能力从简单文字的处理，逐步演化到复杂的reasoning推断，甚至可以做decision making来完成api调用及tool的使用。
  此条thread回顾了两篇重要的CoT文章作为读书笔记。
  🧵👇 
  ![](https://pbs.twimg.com/media/Fs33flTaYAIrmjF.png) ([View Tweet](https://twitter.com/realrenmin/status/1643241565031366657))
- 2/ Paper 1: Chain-of-Thought Prompting Elicits Reasoning in Large Language Models
  此文是CoT的开山之作，作者Jason Wei当时就职于google brain，如今在openAI，同时也是ChatGPT的重要作者。
  CoT是解锁LLM 推理能力的重要钥匙，一举开启了挖掘LLM隐藏技能的新的paradigm 
  ![](https://pbs.twimg.com/media/Fs33f-MagAIo5zq.jpg) ([View Tweet](https://twitter.com/realrenmin/status/1643241573331894279))
- 3/ 在CoT出现之前, LLM的发展遇到了尴尬的瓶颈，模型越来越大，处理文字能力越来越强，但却似乎没有涌现出接近人类的推理能力，包括算术（e.g. 8只鸡4只兔同笼，一共多少只脚），常识（e.g. 鸭梨能漂在水中么？）以及符号（e.g. 抛硬币若干次，到底哪面朝上）的推理。 ([View Tweet](https://twitter.com/realrenmin/status/1643241576557338625))
- 4/ 作者Jason发现，传统的prompting中，总是让模型一步到位地解决一个复杂multi-step问题，而我们人类的认知方式则是分步骤解决复杂推理问题。
  所以，他提出了一个简单有效的prompting方法，把人类思考问题的过程，所谓chain of thought，用自然语言的形式，显性的放在prompt message中。 
  ![](https://pbs.twimg.com/media/Fs33gkcakAAb8yZ.jpg) ([View Tweet](https://twitter.com/realrenmin/status/1643241583150792707))
- 5/ 这样以来，prompt的message形式由
  <input, output>
  转化为：
  <input, chain of thought, output> ([View Tweet](https://twitter.com/realrenmin/status/1643241586330058754))
- 6/ 之前的thread讲过language modeling，而CoT的思想与之呼应。当chain of thought被放在prompt中时，就会强制LLM在给出答案前， 把chain of thought输出。
  从条件概率分布的角度来讲，答案在chain of thought后，其准确的可能性更大。
  这也反应了一个问题，即LLM或许没有思考，它只在乎输出。 ([View Tweet](https://twitter.com/realrenmin/status/1643241588896964608))
- 7/ 作者经过实验，发现这种简单的prompting方式在超过1000亿的大模型上非常有效，而在小模型上效果不明显。
  如果将‘涌现’定义为：
  “由量变引起的质变”
  那么虽然作者没有直接证明大模型可以推理，但直接证明了经过CoT, 大模型的推理能力可以被解锁，并且这种能力在超过1000亿的超大模型上得以涌现。 ([View Tweet](https://twitter.com/realrenmin/status/1643241591623274497))
- 8/ 题外话，ChatGPT一种涌现的工具，其强大的涌现能力与作者Jason有直接的联系，我们有理由怀疑，不开源的ChatGPT下，或针对用户的输入和任务，有着隐含的CoT，来引导大模型获得更加突出的表现。 ([View Tweet](https://twitter.com/realrenmin/status/1643241594244722688))
- 9/ Paper 2: Large Language Models are Zero-Shot Reasoners
  Jason的文章中，所用的CoT是手动设计的，所以隶属于few-shot-CoT, 需要一定的人工成本。
  此文作者小岛武，进一步简化了CoT的过程，简单的将 ‘Let's think step by step’ 放进prompt message， 让LLM自动生成CoT, 所谓的zero-shot-CoT. 
  ![](https://pbs.twimg.com/media/Fs33hl5acAAfsXL.png) ([View Tweet](https://twitter.com/realrenmin/status/1643241600636833793))
- 10/ ‘Let's think step by step’这句神奇的话，仿佛咒语，将解锁LLM的能力的过程一步简化！
  具体来说，完成逻辑推理任务，只需要两步：
  1) 念咒语‘Let's think step by step’， 生成CoT
  2）将CoT再此嵌入prompt message，完成任务。 
  ![](https://pbs.twimg.com/media/Fs33iBBakAEQOrZ.jpg) ([View Tweet](https://twitter.com/realrenmin/status/1643241608606019585))
- 11/ 下面给出一个在@LangChainAI 中使用 chain-of-thought 来完成SQL query generation的例子 
  ![](https://pbs.twimg.com/media/Fr2bmeJXsAEskN6.png) ([View Tweet](https://twitter.com/realrenmin/status/1643241611546206209))
- 12 /
  Paper 1 链接：https://t.co/YFflHnNak3
  Paper 2 链接：https://t.co/y1G7RRop8u ([View Tweet](https://twitter.com/realrenmin/status/1643241614226382849))
- 13/ 下一个thread，将记录用CoT完成api和工具使用的paper读书笔记，如果你喜欢我的读书笔记，请关注我 @realrenmin ，每周会写一到两个长thread跟大家分享NLP的知识。 ([View Tweet](https://twitter.com/realrenmin/status/1643241616881385472))
# 1/ 从Chain-of-Thought (Co...

![rw-book-cover](https://pbs.twimg.com/profile_images/1555109458073747457/JANhY5Zh.jpg)

## Metadata
- Author: [[@realrenmin on Twitter]]
- Full Title: 1/ 从Chain-of-Thought (Co...
- Category: #tweets
- URL: https://twitter.com/realrenmin/status/1643241565031366657

## Highlights
- 1/ 从Chain-of-Thought (CoT) 到 Let's think step by step
  最近每天都可以看到大语言模型进展的文章，LLM的能力从简单文字的处理，逐步演化到复杂的reasoning推断，甚至可以做decision making来完成api调用及tool的使用。
  此条thread回顾了两篇重要的CoT文章作为读书笔记。
  🧵👇 
  ![](https://pbs.twimg.com/media/Fs33flTaYAIrmjF.png) ([View Tweet](https://twitter.com/realrenmin/status/1643241565031366657))
- 2/ Paper 1: Chain-of-Thought Prompting Elicits Reasoning in Large Language Models
  此文是CoT的开山之作，作者Jason Wei当时就职于google brain，如今在openAI，同时也是ChatGPT的重要作者。
  CoT是解锁LLM 推理能力的重要钥匙，一举开启了挖掘LLM隐藏技能的新的paradigm 
  ![](https://pbs.twimg.com/media/Fs33f-MagAIo5zq.jpg) ([View Tweet](https://twitter.com/realrenmin/status/1643241573331894279))
- 3/ 在CoT出现之前, LLM的发展遇到了尴尬的瓶颈，模型越来越大，处理文字能力越来越强，但却似乎没有涌现出接近人类的推理能力，包括算术（e.g. 8只鸡4只兔同笼，一共多少只脚），常识（e.g. 鸭梨能漂在水中么？）以及符号（e.g. 抛硬币若干次，到底哪面朝上）的推理。 ([View Tweet](https://twitter.com/realrenmin/status/1643241576557338625))
- 4/ 作者Jason发现，传统的prompting中，总是让模型一步到位地解决一个复杂multi-step问题，而我们人类的认知方式则是分步骤解决复杂推理问题。
  所以，他提出了一个简单有效的prompting方法，把人类思考问题的过程，所谓chain of thought，用自然语言的形式，显性的放在prompt message中。 
  ![](https://pbs.twimg.com/media/Fs33gkcakAAb8yZ.jpg) ([View Tweet](https://twitter.com/realrenmin/status/1643241583150792707))
- 5/ 这样以来，prompt的message形式由
  <input, output>
  转化为：
  <input, chain of thought, output> ([View Tweet](https://twitter.com/realrenmin/status/1643241586330058754))
- 6/ 之前的thread讲过language modeling，而CoT的思想与之呼应。当chain of thought被放在prompt中时，就会强制LLM在给出答案前， 把chain of thought输出。
  从条件概率分布的角度来讲，答案在chain of thought后，其准确的可能性更大。
  这也反应了一个问题，即LLM或许没有思考，它只在乎输出。 ([View Tweet](https://twitter.com/realrenmin/status/1643241588896964608))
- 7/ 作者经过实验，发现这种简单的prompting方式在超过1000亿的大模型上非常有效，而在小模型上效果不明显。
  如果将‘涌现’定义为：
  “由量变引起的质变”
  那么虽然作者没有直接证明大模型可以推理，但直接证明了经过CoT, 大模型的推理能力可以被解锁，并且这种能力在超过1000亿的超大模型上得以涌现。 ([View Tweet](https://twitter.com/realrenmin/status/1643241591623274497))
- 8/ 题外话，ChatGPT一种涌现的工具，其强大的涌现能力与作者Jason有直接的联系，我们有理由怀疑，不开源的ChatGPT下，或针对用户的输入和任务，有着隐含的CoT，来引导大模型获得更加突出的表现。 ([View Tweet](https://twitter.com/realrenmin/status/1643241594244722688))
- 9/ Paper 2: Large Language Models are Zero-Shot Reasoners
  Jason的文章中，所用的CoT是手动设计的，所以隶属于few-shot-CoT, 需要一定的人工成本。
  此文作者小岛武，进一步简化了CoT的过程，简单的将 ‘Let's think step by step’ 放进prompt message， 让LLM自动生成CoT, 所谓的zero-shot-CoT. 
  ![](https://pbs.twimg.com/media/Fs33hl5acAAfsXL.png) ([View Tweet](https://twitter.com/realrenmin/status/1643241600636833793))
- 10/ ‘Let's think step by step’这句神奇的话，仿佛咒语，将解锁LLM的能力的过程一步简化！
  具体来说，完成逻辑推理任务，只需要两步：
  1) 念咒语‘Let's think step by step’， 生成CoT
  2）将CoT再此嵌入prompt message，完成任务。 
  ![](https://pbs.twimg.com/media/Fs33iBBakAEQOrZ.jpg) ([View Tweet](https://twitter.com/realrenmin/status/1643241608606019585))
- 11/ 下面给出一个在@LangChainAI 中使用 chain-of-thought 来完成SQL query generation的例子 
  ![](https://pbs.twimg.com/media/Fr2bmeJXsAEskN6.png) ([View Tweet](https://twitter.com/realrenmin/status/1643241611546206209))
- 12 /
  Paper 1 链接：https://t.co/YFflHnNak3
  Paper 2 链接：https://t.co/y1G7RRop8u ([View Tweet](https://twitter.com/realrenmin/status/1643241614226382849))
- 13/ 下一个thread，将记录用CoT完成api和工具使用的paper读书笔记，如果你喜欢我的读书笔记，请关注我 @realrenmin ，每周会写一到两个长thread跟大家分享NLP的知识。 ([View Tweet](https://twitter.com/realrenmin/status/1643241616881385472))

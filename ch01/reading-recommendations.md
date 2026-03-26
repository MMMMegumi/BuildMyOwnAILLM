# Recommendations for Getting the Most Out of a Technical Book

Below are a few notes I previously shared when readers ask how to get the most out of my building large language model from scratch book(s).


I follow a similar approach when I read technical books myself. It is not meant as a universal recipe, but it may be a helpful starting point.

For this particular book, I strongly suggest reading it in order since each chapter depends on the previous one. And for each chapter, I recommend the following steps.

&nbsp;
### 1) First read (offline)

I recommend reading the chapter from start to finish without any coding, yet.
The goal of this first read-through is to get the big picture first.

Ideally, I recommend reading the chapter away from the computer. A physical copy works
well, but a digital device without distractions (no browser, social media, or
email) works, too.

Personally, I read both on paper and on an e-ink tablet. While I have used
e-ink tablets since 2018, and always try to read more on e-ink, I still notice
that physical copies help me focus better. That is also why I sometimes print
research papers that are challenging or that I really want to understand in
detail.

My recommendation is to make the first read-through a short, focused 20-minute reading
session with minimal distractions and without overthinking it or getting stuck
with details.

Highlighting or annotating confusing or interesting parts is
fine, but I would not look things up at this stage. I just suggest reading, but
not running any code yet. This first pass is meant to understand the bigger picture.

&nbsp;
### 2) Second read (with code)

On the second read-through, I recommend typing up and running the code from the chapter. Copying code is tempting because retyping is a lot of work, but when I read other technical books, it usually helps me to think about the code a bit more (versus just glancing over it). 

If I get different results than in the book, I would check the book's GitHub repo and try the code from there. If I still get different results, I would try to see if it's due to different package versions, random seeds, CPU/CUDA, etc. If I then still can't figure it out, asking the author would not be a bad idea (via the book forum, public GitHub repo issues or discussions, and as a last resort, email).

&nbsp;
### 3) Exercises

After the second read-through, retyping and running the code, it's usually a good time to try the exercises. It's great for solidifying one's understanding or tinkering with a problem in a semi-structured way. If the exercise is too challenging, it's okay to look at the solution. However, I would still recommend giving it a solid try first.

&nbsp;
### 4) Review notes and explore further

Now, after reading the chapter, running the code, and doing the exercises, I recommend going back to highlights and annotations from the previous two read-throughs and seeing if there's still something unclear.

This is also a good time to look up additional references or do a quick search to clarify anything that still feels unresolved. But even if everything makes sense, reading more about a topic of interest is not a bad idea.

At this stage, it also makes sense to write down or transfer useful insights, code snippets, etc., to your favorite note-taking app. 

&nbsp;
### 5) Use the ideas in a project

The previous steps were all about soaking up knowledge. Now, see if you can use certain aspects of a chapter in your own project. Or maybe build a small project using the code from the book as a starting point. For inspiration, check out the bonus materials, which are basically mini-projects I did to satisfy my own curiosity.

For example, after reading about the multi-head attention mechanisms and implementing the LLM, you may wonder how well a model with grouped-query attention performs, or how much of a difference RMSNorm vs LayerNorm really makes. And so forth.

There could also be smaller aspects that could be useful in your own projects. For example, sometimes it is a tiny detail that ends up being useful, like testing whether
explicitly calling `torch.mps.manual_seed(seed)` changes anything
compared to using `torch.manual_seed(seed)` alone.

Eventually, though, I somehow want to use that knowledge. This could involve using the main concept from the chapter, but also sometimes minor tidbits I learned along the way, e.g., even trivial things like whether it actually makes a difference in my project to explicitly call 
`torch.mps.manual_seed(seed)` instead of just `torch.manual_seed(seed)`.

&nbsp;
### Additional thoughts

Of course, none of the above is set in stone. If the topic is overall very familiar or easy, and I am primarily reading the book to get some information in later chapters, skimming a chapter is ok (to not waste my time).

Also, for chapters that don't have any code (for example, the introductory chapter 1), it makes of course sense to skip the code-related steps.

Anyway, I hope this is useful. And happy reading and learning!

以下是我之前分享的一些笔记，供读者参考如何最大化地利用我的《从零开始构建大语言模型》这本书。

我自己阅读技术书籍时也遵循类似的方法。这并不是一个放之四海而皆准的万能公式，但或许能作为一个有用的起点。

对于这本书，我强烈建议按顺序阅读，因为每一章都建立在上一章的基础上。对于每一章，我建议按以下步骤进行。

 
1）第一遍阅读（离线）

我建议先把一章从头到尾读一遍，暂时不写任何代码。
第一遍阅读的目标是先把握整体框架。

理想情况下，我建议远离电脑来阅读这一章。纸质书效果很好，使用没有干扰（不打开浏览器、社交媒体或邮件）的电子设备阅读也可以。

就我个人而言，纸质书和墨水屏阅读器我都会用。虽然我从2018年就开始使用墨水屏阅读器，并一直尽量在它上面阅读，但我仍然觉得纸质书能让我更专注。这也是为什么我有时会把那些很有挑战性、或者想深入理解的研究论文打印出来看。

我的建议是，让第一遍阅读成为一次短小、专注的20分钟阅读，尽量减少干扰，不要过度思考或纠结于细节。

标记或批注感到困惑或有趣的部分没问题，但在这个阶段不要去查阅资料。我建议只是读，暂时不要运行任何代码。这第一遍的目的是理解整体框架。

 
2）第二遍阅读（结合代码）

第二遍阅读时，我建议亲手敲一遍并运行本章的代码。复制粘贴代码很诱人，因为重新敲一遍工作量不小，但在我阅读其他技术书籍时，这通常能帮助我更深入地思考代码（而不是仅仅扫一眼）。

如果我得到的结果和书中不同，我会先查看本书的 GitHub 仓库，尝试那里的代码。如果结果还是不一样，我会尝试排查是否是因为包版本、随机种子、CPU/CUDA 等因素导致的。如果仍然无法解决，那么向作者提问是个不错的办法（可以通过本书论坛、公开的 GitHub 仓库 issues 或 discussions 提问，最后的选择是发邮件）。

 
3）做练习

在第二遍阅读、重新敲代码并运行之后，通常是尝试做练习的好时机。这对于巩固理解，或以半结构化的方式钻研问题非常有帮助。如果练习太难，看答案也没关系，但我还是建议自己先认真尝试一下。

 
4）回顾笔记并进一步探索

现在，在读完一章、运行代码并做完练习之后，我建议回过头看看前两遍阅读时做的标记和批注，检查一下是否还有不清楚的地方。

这也是一个查漏补缺的好时机，可以查阅额外的参考资料或快速搜索，以澄清任何仍未解决的问题。但即使一切都理解了，多读一些自己感兴趣的、相关的主题也不是坏事。

在这个阶段，把有用的见解、代码片段等记录下来或转移到你喜欢的笔记应用中也是很有意义的。

 
5）在项目中应用这些想法

前面的步骤都是为了吸收知识。现在，看看你是否能将自己项目中的某些方面与本章的内容结合起来。或者，以本书的代码为起点，构建一个小项目来获取灵感。可以参考一下本书的补充材料，那基本上是我为了满足自己的好奇心而做的一些迷你项目。

例如，在阅读了关于多头注意力机制并实现了 LLM 之后，你可能会好奇使用分组查询注意力（Grouped-Query Attention）的模型表现如何，或者 RMSNorm 与 LayerNorm 到底有多大的区别，等等。

有时，一些很小的细节最终可能会在你的项目中派上用场。例如，测试显式调用 torch.mps.manual_seed(seed) 与单独使用 torch.manual_seed(seed) 相比是否会有什么不同。

最终，无论如何我都希望能把这些知识用起来。这可能是用到本章的主要概念，但有时也可能只是顺便学到的一些小技巧，甚至是一些微不足道的事情，比如在我的项目里，显式调用 torch.mps.manual_seed(seed) 而不是只调用 torch.manual_seed(seed) 是否真的有区别。

 
补充想法

当然，以上都不是一成不变的。如果某个主题我总体上非常熟悉或觉得简单，我读书主要是为了获取后面章节的一些信息，那么快速浏览一章是可以的（为了不浪费时间）。

另外，对于没有代码的章节（例如介绍性的第1章），跳过与代码相关的步骤当然也是合理的。

总之，希望这些对你有用。祝阅读和学习愉快！
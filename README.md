# 从零开始构建大型语言模型

本仓库包含开发、预训练和微调类GPT大型语言模型（LLM）的代码，是《从零开始构建大型语言模型》一书的官方代码仓库。

在《从零开始构建大型语言模型》一书中，你将通过从零开始、一步步编码的方式，从内到外地理解大型语言模型（LLM）的工作原理。在本书中，我将通过清晰的文字、图表和示例，引导你创建自己的LLM，并对每个阶段进行解释。

本书中描述的用于训练和开发自己的、用于教育目的小型但功能齐全的模型的方法，与创建像ChatGPT背后那样的大规模基础模型的方法相呼应。此外，本书还包含了用于加载更大预训练模型权重以进行微调的代码。

*   [官方源代码仓库链接](https://github.com/rasbt/LLMs-from-scratch)
*   [Manning（出版社网站）上的图书链接](https://www.manning.com/books/build-a-large-language-model-from-scratch)
*   [Amazon.com上的图书页面链接](https://www.amazon.com/Build-Large-Language-Model-Scratch/dp/1633437167)
*   ISBN 9781633437166

要下载本仓库的副本，请点击“Download ZIP”按钮，或在终端中执行以下命令：

```bash
git clone --depth 1 https://github.com/rasbt/LLMs-from-scratch.git
```

（如果你是从Manning网站下载的代码包，请考虑访问GitHub上的官方代码仓库 https://github.com/rasbt/LLMs-from-scratch 以获取最新更新。）

## 目录

请注意，本 README.md 文件是一个 Markdown（.md）文件。如果你是从Manning网站下载的代码包并在本地计算机上查看，建议使用Markdown编辑器或预览器以获得正确的查看效果。如果你尚未安装Markdown编辑器，[Ghostwriter](https://ghostwriter.kde.org/) 是一个不错的免费选择。

你也可以在浏览器中通过 GitHub 访问 https://github.com/rasbt/LLMs-from-scratch 来查看此文件及其他文件，GitHub会自动渲染Markdown。

> **提示：** 如果你需要关于安装Python和Python包以及设置代码环境的指导，建议阅读 `setup` 目录中的 README.md 文件。

| 代码测试 Linux | 代码测试 Windows | 代码测试 macOS |
|---|---|---|

| 章节标题 | 主要代码（快速访问） | 全部代码 + 补充材料 |
|---|---|---|
| [环境设置建议](setup/README.md) | - | - |
| [如何最好地阅读本书](https://sebastianraschka.com/blog/2025/reading-books.html) | - | - |
| [**第1章：理解大型语言模型**](ch01/README.md) | 无代码 | [`./ch01`](ch01/) |
| [**第2章：处理文本数据**](ch02/README.md) | • [ch02.ipynb](ch02/01_main-chapter-code/ch02.ipynb)<br>• [dataloader.ipynb (总结)](ch02/01_main-chapter-code/dataloader.ipynb)<br>• [exercise-solutions.ipynb](ch02/01_main-chapter-code/exercise-solutions.ipynb) | [`./ch02`](ch02/) |
| [**第3章：编码注意力机制**](ch03/README.md) | • [ch03.ipynb](ch03/01_main-chapter-code/ch03.ipynb)<br>• [multihead-attention.ipynb (总结)](ch03/01_main-chapter-code/multihead-attention.ipynb)<br>• [exercise-solutions.ipynb](ch03/01_main-chapter-code/exercise-solutions.ipynb) | [`./ch03`](ch03/) |
| [**第4章：从零实现一个GPT模型**](ch04/README.md) | • [ch04.ipynb](ch04/01_main-chapter-code/ch04.ipynb)<br>• [gpt.py (总结)](ch04/01_main-chapter-code/gpt.py)<br>• [exercise-solutions.ipynb](ch04/01_main-chapter-code/exercise-solutions.ipynb) | [`./ch04`](ch04/) |
| [**第5章：在无标签数据上预训练**](ch05/README.md) | • [ch05.ipynb](ch05/01_main-chapter-code/ch05.ipynb)<br>• [gpt_train.py (总结)](ch05/01_main-chapter-code/gpt_train.py)<br>• [gpt_generate.py (总结)](ch05/01_main-chapter-code/gpt_generate.py)<br>• [exercise-solutions.ipynb](ch05/01_main-chapter-code/exercise-solutions.ipynb) | [`./ch05`](ch05/) |
| [**第6章：为文本分类进行微调**](ch06/README.md) | • [ch06.ipynb](ch06/01_main-chapter-code/ch06.ipynb)<br>• [gpt_class_finetune.py](ch06/01_main-chapter-code/gpt_class_finetune.py)<br>• [exercise-solutions.ipynb](ch06/01_main-chapter-code/exercise-solutions.ipynb) | [`./ch06`](ch06/) |
| [**第7章：微调以遵循指令**](ch07/README.md) | • [ch07.ipynb](ch07/01_main-chapter-code/ch07.ipynb)<br>• [gpt_instruction_finetuning.py (总结)](ch07/01_main-chapter-code/gpt_instruction_finetuning.py)<br>• [ollama_evaluate.py (总结)](ch07/01_main-chapter-code/ollama_evaluate.py)<br>• [exercise-solutions.ipynb](ch07/01_main-chapter-code/exercise-solutions.ipynb) | [`./ch07`](ch07/) |
| [**附录A：PyTorch简介**](appendix-A/01_main-chapter-code/README.md) | • [code-part1.ipynb](appendix-A/01_main-chapter-code/code-part1.ipynb)<br>• [code-part2.ipynb](appendix-A/01_main-chapter-code/code-part2.ipynb)<br>• [DDP-script.py](appendix-A/01_main-chapter-code/DDP-script.py)<br>• [exercise-solutions.ipynb](appendix-A/01_main-chapter-code/exercise-solutions.ipynb) | [`./appendix-A`](appendix-A/) |
| [**附录B：参考文献与延伸阅读**](appendix-B/README.md) | 无代码 | [`./appendix-B`](appendix-B/) |
| [**附录C：练习解答**](appendix-C/README.md) | • [练习解答列表](appendix-C/) | [`./appendix-C`](appendix-C/) |
| [**附录D：为训练循环锦上添花**](appendix-D/01_main-chapter-code/README.md) | • [appendix-D.ipynb](appendix-D/01_main-chapter-code/appendix-D.ipynb) | [`./appendix-D`](appendix-D/) |
| [**附录E：使用LoRA进行参数高效微调**](appendix-E/01_main-chapter-code/README.md) | • [appendix-E.ipynb](appendix-E/01_main-chapter-code/appendix-E.ipynb) | [`./appendix-E`](appendix-E/) |

下方的思维导图总结了本书涵盖的内容。

<img src="https://sebastianraschka.com/images/LLMs-from-scratch-images/mental-model.jpg" width="650px">

## 先决条件

最重要的先决条件是扎实的Python编程基础。有了这些知识，你将能很好地为探索迷人的LLM世界并理解本书中展示的概念和代码示例做好准备。

如果你对深度神经网络有一些经验，你可能会发现某些概念更熟悉，因为LLM正是构建在这些架构之上的。

本书使用PyTorch从零实现代码，不使用任何外部LLM库。虽然不要求精通PyTorch，但熟悉PyTorch基础知识当然会有所帮助。如果你是PyTorch新手，附录A提供了PyTorch的简明介绍。或者，你可能会发现我的书《一小时入门PyTorch：从张量到多GPU训练神经网络》对学习基础知识很有帮助。

## 硬件要求

本书主要章节中的代码设计为在常规笔记本电脑上合理的时间内运行，**不需要专门的硬件**。这种方法确保了广大读者都能使用这些材料。此外，如果GPU可用，代码会自动利用它们。（更多建议请参阅[环境设置文档](setup/README.md)。）

## 视频课程

一个**17小时15分钟**的配套视频课程，我将逐章讲解本书的代码。该课程按章节和部分组织，与本书结构相对应，既可以作为本书的独立替代品，也可以作为配套的代码实战资源。

[![视频课程链接](https://img.youtube.com/vi/7xTGNNPKy3c/0.jpg)](https://www.youtube.com/watch?v=7xTGNNPKy3c)

## 配套书籍 / 续作

**《从零构建推理模型》** 虽然是一本独立的书，但可以被视为《从零构建大型语言模型》的续作。

它从一个预训练模型开始，实现了不同的推理方法，包括推理时扩展、强化学习和蒸馏，以提高模型的推理能力。

与《从零构建大型语言模型》类似，《从零构建推理模型》也采用从零开始实现这些方法的实践方法。

*   [Amazon链接（待定）]()
*   [Manning链接](https://www.manning.com/books/build-a-reasoning-model-from-scratch)
*   [GitHub仓库](https://github.com/rasbt/Reasoning-From-Scratch)

## 练习

本书的每一章都包含几个练习。解答总结在**附录C**中，相应的代码笔记本可在本仓库的主要章节文件夹中找到（例如，`./ch02/01_main-chapter-code/exercise-solutions.ipynb`）。

除了代码练习，你还可以从Manning网站下载一份免费的**170页PDF**，名为**《自测：从零构建大型语言模型》**。它每章包含约30道测验题和解答，帮助你检验理解。

[![自测题预览](images/quiz-preview-small.png)](https://www.manning.com/books/build-a-large-language-model-from-scratch)

## 补充材料

几个文件夹包含了为感兴趣的读者提供的可选材料：

*   **环境设置**
    *   [Python设置技巧](setup/01_python-setup指南.md)
    *   [安装本书使用的Python包和库](setup/02_installing-python-libraries.md)
    *   [Docker环境设置指南](setup/03_docker-environment.md)
*   **第2章：处理文本数据**
    *   [从头开始的字节对编码（BPE）分词器](ch02/05_bpe-from-scratch/README.md)
    *   [比较各种字节对编码（BPE）实现](ch02/02_bonus_bytepair-encoder/README.md)
    *   [理解嵌入层和线性层之间的区别](ch02/03_bonus_embedding-vs-matmul/README.md)
    *   [用简单数字直观理解数据加载器](ch02/04_bonus_dataloader-intuition/README.md)
*   **第3章：编码注意力机制**
    *   [比较高效的多头注意力实现](ch03/02_bonus_efficient-multihead-attention/README.md)
    *   [理解PyTorch Buffers](ch03/03_bonus_pytorch-buffers/README.md)
*   **第4章：从零实现一个GPT模型**
    *   [FLOPs分析](ch04/02_bonus_flops-analysis/README.md)
    *   [KV缓存](ch04/03_bonus_kv-cache/README.md)
    *   [注意力机制的替代方案](ch04/04_bonus_attention-alternatives/README.md)
        *   [分组查询注意力（Grouped-Query Attention）](ch04/04_bonus_attention-alternatives/grouped-query-attention.ipynb)
        *   [多查询潜在注意力（Multi-Head Latent Attention）](ch04/04_bonus_attention-alternatives/multi-head-latent-attention.ipynb)
        *   [滑动窗口注意力（Sliding Window Attention）](ch04/04_bonus_attention-alternatives/sliding-window-attention.ipynb)
        *   [门控DeltaNet](ch04/04_bonus_attention-alternatives/gated-deltanet.ipynb)
        *   [混合专家（Mixture-of-Experts, MoE）](ch04/04_bonus_attention-alternatives/moe-from-scratch.ipynb)
*   **第5章：在无标签数据上预训练**
    *   [备选权重加载方法](ch05/02_alternative-weight-loading/README.md)
    *   [在Project Gutenberg数据集上预训练GPT](ch05/03_pretraining-gpt-on-gutenberg/README.md)
    *   [为训练循环锦上添花](ch05/04_bells-and-whistles/README.md)
    *   [为预训练优化超参数](ch05/05_hyperparameter-optimization/README.md)
    *   [构建用户界面与预训练LLM交互](ch05/06_user-interface/README.md)
    *   [将GPT转换为Llama](ch05/07_gpt-to-llama/README.md)
    *   [内存高效的模型权重加载](ch05/08_memory-efficient-weight-loading/README.md)
    *   [使用新标记扩展Tiktoken BPE分词器](ch05/09_extending-tiktoken/README.md)
    *   [PyTorch性能技巧：加速LLM训练](ch05/10_pytorch-performance/README.md)
    *   [**LLM架构**](ch05/11_llm-architectures/README.md)
        *   [从零实现Llama 3.2](ch05/11_llm-architectures/llama3-from-scratch.ipynb)
        *   [从零实现Qwen3（密集型和混合专家MoE）](ch05/11_llm-architectures/qwen3-from-scratch.ipynb)
        *   [从零实现Gemma 3](ch05/11_llm-architectures/gemma3-from-scratch.ipynb)
        *   [从零实现Olmo 3](ch05/11_llm-architectures/olmo3-from-scratch.ipynb)
        *   [从零实现Tiny Aya](ch05/11_llm-architectures/tiny-aya-from-scratch.ipynb)
        *   [从零实现Qwen3.5](ch05/11_llm-architectures/qwen3.5-from-scratch.ipynb)
    *   [**第5章：使用其他LLM作为替代（例如，Llama 3, Qwen 3）**](ch05/12_llm-tutorials/README.md)
*   **第6章：为分类进行微调**
    *   [关于微调不同层和使用更大模型的补充实验](ch06/02_bonus_additional-experiments/README.md)
    *   [在5万条IMDb电影评论数据集上微调不同模型](ch06/03_bonus_imdb-classification/README.md)
    *   [构建用户界面与基于GPT的垃圾邮件分类器交互](ch06/04_bonus_user-interface/README.md)
*   **第7章：微调以遵循指令**
    *   [用于查找近乎重复项和创建被动语态条目的数据集工具](ch07/02_dataset-utilities/README.md)
    *   [使用OpenAI API和Ollama评估指令响应](ch07/03_model-evaluation/README.md)
    *   [为指令微调生成数据集](ch07/04_preference-tuning/01_generate-preference-data-llama-ollama/README.md)
    *   [改进用于指令微调的数据集](ch07/04_preference-tuning/02_dataset-hardening/README.md)
    *   [使用Llama 3.1 70B和Ollama生成偏好数据集](ch07/04_preference-tuning/01_generate-preference-data-llama-ollama/README.md)
    *   [用于LLM对齐的直接偏好优化（DPO）](ch07/04_preference-tuning/03_dpo-from-scratch/README.md)
    *   [构建用户界面与指令微调后的GPT模型交互](ch07/05_user-interface/README.md)
*   **来自《从零构建推理模型》仓库的更多补充材料**：[`Reasoning-From-Scratch`](https://github.com/rasbt/Reasoning-From-Scratch)
    *   **Qwen3（从零）基础**
        *   [Qwen3源代码走读](https://github.com/rasbt/Reasoning-From-Scratch/blob/main/qwen3/01_bonus_notebooks/00_qwen3-walkthrough.ipynb)
        *   [优化的Qwen3](https://github.com/rasbt/Reasoning-From-Scratch/blob/main/qwen3/01_bonus_notebooks/01_qwen3-optimized.ipynb)
    *   **评估**
        *   [基于验证器的评估（MATH-500）](https://github.com/rasbt/Reasoning-From-Scratch/blob/main/eval/01_math-eval/README.md)
        *   [多项选择评估（MMLU）](https://github.com/rasbt/Reasoning-From-Scratch/blob/main/eval/02_multiple-choice-eval/README.md)
        *   [LLM排行榜评估](https://github.com/rasbt/Reasoning-From-Scratch/blob/main/eval/03_llm-leaderboard-eval/README.md)
        *   [LLM作为评判者的评估](https://github.com/rasbt/Reasoning-From-Scratch/blob/main/eval/04_llm-as-a-judge/README.md)
    *   **推理时扩展**
        *   [自洽性（Self-Consistency）](https://github.com/rasbt/Reasoning-From-Scratch/blob/main/inference-scaling/01_self-consistency/README.md)
        *   [自我优化（Self-Refinement）](https://github.com/rasbt/Reasoning-From-Scratch/blob/main/inference-scaling/02_self-refinement/README.md)
    *   **强化学习（RL）**
        *   [使用GRPO从零实现RLVR](https://github.com/rasbt/Reasoning-From-Scratch/tree/main/rl/01_grpo-from-scratch)

## 问题、反馈及对本仓库的贡献

我欢迎各种形式的反馈，最好通过 [Manning论坛](https://livebook.manning.com/forum?product=raschka&book=raschka) 或 [GitHub Discussions](https://github.com/rasbt/LLMs-from-scratch/discussions) 分享。同样，如果你有任何问题或只是想和别人交流想法，也请随时在论坛上发帖。

请注意，由于本仓库对应的是纸质书的代码，我目前**无法接受**会扩展主要章节代码内容的贡献，因为这会引入与实体书的偏差。保持一致有助于确保大家都有顺畅的体验。

## 引用

如果你觉得本书或代码对你的研究有用，请考虑引用它。

**芝加哥格式引用：**

Raschka, Sebastian. *Build A Large Language Model (From Scratch)*. Manning, 2024. ISBN: 978-1633437166.

**BibTeX条目：**

```bibtex
@book{build-llms-from-scratch-book,
  author       = {Sebastian Raschka},
  title        = {Build A Large Language Model (From Scratch)},
  publisher    = {Manning},
  year         = {2024},
  isbn         = {978-1633437166},
  url          = {https://www.manning.com/books/build-a-large-language-model-from-scratch},
  github       = {https://github.com/rasbt/LLMs-from-scratch}
}
```

# Build a Large Language Model (From Scratch)

This repository contains the code for developing, pretraining, and finetuning a GPT-like LLM and is the official code repository for the book [Build a Large Language Model (From Scratch)](https://amzn.to/4fqvn0D).

<br>
<br>

<a href="https://amzn.to/4fqvn0D"><img src="https://sebastianraschka.com/images/LLMs-from-scratch-images/cover.jpg?123" width="250px"></a>

<br>

In [*Build a Large Language Model (From Scratch)*](http://mng.bz/orYv), you'll learn and understand how large language models (LLMs) work from the inside out by coding them from the ground up, step by step. In this book, I'll guide you through creating your own LLM, explaining each stage with clear text, diagrams, and examples.

The method described in this book for training and developing your own small-but-functional model for educational purposes mirrors the approach used in creating large-scale foundational models such as those behind ChatGPT. In addition, this book includes code for loading the weights of larger pretrained models for finetuning.

- Link to the official [source code repository](https://github.com/rasbt/LLMs-from-scratch)
- [Link to the book at Manning (the publisher's website)](http://mng.bz/orYv)
- [Link to the book page on Amazon.com](https://www.amazon.com/gp/product/1633437167)
- ISBN 9781633437166

<a href="http://mng.bz/orYv#reviews"><img src="https://sebastianraschka.com//images/LLMs-from-scratch-images/other/reviews.png" width="220px"></a>


<br>
<br>

To download a copy of this repository, click on the [Download ZIP](https://github.com/rasbt/LLMs-from-scratch/archive/refs/heads/main.zip) button or execute the following command in your terminal:

```bash
git clone --depth 1 https://github.com/rasbt/LLMs-from-scratch.git
```

<br>

(If you downloaded the code bundle from the Manning website, please consider visiting the official code repository on GitHub at [https://github.com/rasbt/LLMs-from-scratch](https://github.com/rasbt/LLMs-from-scratch) for the latest updates.)

<br>
<br>


# Table of Contents

Please note that this `README.md` file is a Markdown (`.md`) file. If you have downloaded this code bundle from the Manning website and are viewing it on your local computer, I recommend using a Markdown editor or previewer for proper viewing. If you haven't installed a Markdown editor yet, [Ghostwriter](https://ghostwriter.kde.org) is a good free option.

You can alternatively view this and other files on GitHub at [https://github.com/rasbt/LLMs-from-scratch](https://github.com/rasbt/LLMs-from-scratch) in your browser, which renders Markdown automatically.

<br>
<br>


> **Tip:**
> If you're seeking guidance on installing Python and Python packages and setting up your code environment, I suggest reading the [README.md](setup/README.md) file located in the [setup](setup) directory.

<br>
<br>

[![Code tests Linux](https://github.com/rasbt/LLMs-from-scratch/actions/workflows/basic-tests-linux-uv.yml/badge.svg)](https://github.com/rasbt/LLMs-from-scratch/actions/workflows/basic-tests-linux-uv.yml)
[![Code tests Windows](https://github.com/rasbt/LLMs-from-scratch/actions/workflows/basic-tests-windows-uv-pip.yml/badge.svg)](https://github.com/rasbt/LLMs-from-scratch/actions/workflows/basic-tests-windows-uv-pip.yml)
[![Code tests macOS](https://github.com/rasbt/LLMs-from-scratch/actions/workflows/basic-tests-macos-uv.yml/badge.svg)](https://github.com/rasbt/LLMs-from-scratch/actions/workflows/basic-tests-macos-uv.yml)



| Chapter Title                                              | Main Code (for Quick Access)                                                                                                    | All Code + Supplementary      |
|------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|-------------------------------|
| [Setup recommendations](setup) <br/>[How to best read this book](https://sebastianraschka.com/blog/2025/reading-books.html)                            | -                                                                                                                               | -                             |
| Ch 1: Understanding Large Language Models                  | No code                                                                                                                         | -                             |
| Ch 2: Working with Text Data                               | - [ch02.ipynb](ch02/01_main-chapter-code/ch02.ipynb)<br/>- [dataloader.ipynb](ch02/01_main-chapter-code/dataloader.ipynb) (summary)<br/>- [exercise-solutions.ipynb](ch02/01_main-chapter-code/exercise-solutions.ipynb)               | [./ch02](./ch02)            |
| Ch 3: Coding Attention Mechanisms                          | - [ch03.ipynb](ch03/01_main-chapter-code/ch03.ipynb)<br/>- [multihead-attention.ipynb](ch03/01_main-chapter-code/multihead-attention.ipynb) (summary) <br/>- [exercise-solutions.ipynb](ch03/01_main-chapter-code/exercise-solutions.ipynb)| [./ch03](./ch03)             |
| Ch 4: Implementing a GPT Model from Scratch                | - [ch04.ipynb](ch04/01_main-chapter-code/ch04.ipynb)<br/>- [gpt.py](ch04/01_main-chapter-code/gpt.py) (summary)<br/>- [exercise-solutions.ipynb](ch04/01_main-chapter-code/exercise-solutions.ipynb) | [./ch04](./ch04)           |
| Ch 5: Pretraining on Unlabeled Data                        | - [ch05.ipynb](ch05/01_main-chapter-code/ch05.ipynb)<br/>- [gpt_train.py](ch05/01_main-chapter-code/gpt_train.py) (summary) <br/>- [gpt_generate.py](ch05/01_main-chapter-code/gpt_generate.py) (summary) <br/>- [exercise-solutions.ipynb](ch05/01_main-chapter-code/exercise-solutions.ipynb) | [./ch05](./ch05)              |
| Ch 6: Finetuning for Text Classification                   | - [ch06.ipynb](ch06/01_main-chapter-code/ch06.ipynb)  <br/>- [gpt_class_finetune.py](ch06/01_main-chapter-code/gpt_class_finetune.py)  <br/>- [exercise-solutions.ipynb](ch06/01_main-chapter-code/exercise-solutions.ipynb) | [./ch06](./ch06)              |
| Ch 7: Finetuning to Follow Instructions                    | - [ch07.ipynb](ch07/01_main-chapter-code/ch07.ipynb)<br/>- [gpt_instruction_finetuning.py](ch07/01_main-chapter-code/gpt_instruction_finetuning.py) (summary)<br/>- [ollama_evaluate.py](ch07/01_main-chapter-code/ollama_evaluate.py) (summary)<br/>- [exercise-solutions.ipynb](ch07/01_main-chapter-code/exercise-solutions.ipynb) | [./ch07](./ch07)  |
| Appendix A: Introduction to PyTorch                        | - [code-part1.ipynb](appendix-A/01_main-chapter-code/code-part1.ipynb)<br/>- [code-part2.ipynb](appendix-A/01_main-chapter-code/code-part2.ipynb)<br/>- [DDP-script.py](appendix-A/01_main-chapter-code/DDP-script.py)<br/>- [exercise-solutions.ipynb](appendix-A/01_main-chapter-code/exercise-solutions.ipynb) | [./appendix-A](./appendix-A) |
| Appendix B: References and Further Reading                 | No code                                                                                                                         | [./appendix-B](./appendix-B) |
| Appendix C: Exercise Solutions                             | - [list of exercise solutions](appendix-C)                                                                 | [./appendix-C](./appendix-C) |
| Appendix D: Adding Bells and Whistles to the Training Loop | - [appendix-D.ipynb](appendix-D/01_main-chapter-code/appendix-D.ipynb)                                                          | [./appendix-D](./appendix-D)  |
| Appendix E: Parameter-efficient Finetuning with LoRA       | - [appendix-E.ipynb](appendix-E/01_main-chapter-code/appendix-E.ipynb)                                                          | [./appendix-E](./appendix-E) |

<br>
&nbsp;

The mental model below summarizes the contents covered in this book.

<img src="https://sebastianraschka.com/images/LLMs-from-scratch-images/mental-model.jpg" width="650px">


<br>
&nbsp;

## Prerequisites

The most important prerequisite is a strong foundation in Python programming.
With this knowledge, you will be well prepared to explore the fascinating world of LLMs
and understand the concepts and code examples presented in this book.

If you have some experience with deep neural networks, you may find certain concepts more familiar, as LLMs are built upon these architectures.

This book uses PyTorch to implement the code from scratch without using any external LLM libraries. While proficiency in PyTorch is not a prerequisite, familiarity with PyTorch basics is certainly useful. If you are new to PyTorch, Appendix A provides a concise introduction to PyTorch. Alternatively, you may find my book, [PyTorch in One Hour: From Tensors to Training Neural Networks on Multiple GPUs](https://sebastianraschka.com/teaching/pytorch-1h/), helpful for learning about the essentials.



<br>
&nbsp;

## Hardware Requirements

The code in the main chapters of this book is designed to run on conventional laptops within a reasonable timeframe and does not require specialized hardware. This approach ensures that a wide audience can engage with the material. Additionally, the code automatically utilizes GPUs if they are available. (Please see the [setup](https://github.com/rasbt/LLMs-from-scratch/blob/main/setup/README.md) doc for additional recommendations.)


&nbsp;
## Video Course

[A 17-hour and 15-minute companion video course](https://www.manning.com/livevideo/master-and-build-large-language-models) where I code through each chapter of the book. The course is organized into chapters and sections that mirror the book's structure so that it can be used as a standalone alternative to the book or complementary code-along resource.

<a href="https://www.manning.com/livevideo/master-and-build-large-language-models"><img src="https://sebastianraschka.com/images/LLMs-from-scratch-images/video-screenshot.webp?123" width="350px"></a>


&nbsp;


## Companion Book / Sequel

[*Build A Reasoning Model (From Scratch)*](https://mng.bz/lZ5B), while a standalone book, can be considered as a sequel to *Build A Large Language Model (From Scratch)*.

It starts with a pretrained model and implements different reasoning approaches, including inference-time scaling, reinforcement learning, and distillation, to improve the model's reasoning capabilities.

Similar to *Build A Large Language Model (From Scratch)*, [*Build A Reasoning Model (From Scratch)*](https://mng.bz/lZ5B) takes a hands-on approach implementing these methods from scratch.

<a href="https://mng.bz/lZ5B"><img src="https://sebastianraschka.com/images/reasoning-from-scratch-images/cover.webp?123" width="120px"></a>

- Amazon link (TBD)
- [Manning link](https://mng.bz/lZ5B)
- [GitHub repository](https://github.com/rasbt/reasoning-from-scratch)

<br>

&nbsp;
## Exercises

Each chapter of the book includes several exercises. The solutions are summarized in Appendix C, and the corresponding code notebooks are available in the main chapter folders of this repository (for example,  [./ch02/01_main-chapter-code/exercise-solutions.ipynb](./ch02/01_main-chapter-code/exercise-solutions.ipynb).

In addition to the code exercises, you can download a free 170-page PDF titled  [Test Yourself On Build a Large Language Model (From Scratch)](https://www.manning.com/books/test-yourself-on-build-a-large-language-model-from-scratch) from the Manning website. It contains approximately 30 quiz questions and solutions per chapter to help you test your understanding.

<a href="https://www.manning.com/books/test-yourself-on-build-a-large-language-model-from-scratch"><img src="https://sebastianraschka.com/images/LLMs-from-scratch-images/test-yourself-cover.jpg?123" width="150px"></a>

&nbsp;
## Bonus Material

Several folders contain optional materials as a bonus for interested readers:
- **Setup**
  - [Python Setup Tips](setup/01_optional-python-setup-preferences)
  - [Installing Python Packages and Libraries Used in This Book](setup/02_installing-python-libraries)
  - [Docker Environment Setup Guide](setup/03_optional-docker-environment)

- **Chapter 2: Working With Text Data**
  - [Byte Pair Encoding (BPE) Tokenizer From Scratch](ch02/05_bpe-from-scratch/bpe-from-scratch-simple.ipynb)
  - [Comparing Various Byte Pair Encoding (BPE) Implementations](ch02/02_bonus_bytepair-encoder)
  - [Understanding the Difference Between Embedding Layers and Linear Layers](ch02/03_bonus_embedding-vs-matmul)
  - [Dataloader Intuition With Simple Numbers](ch02/04_bonus_dataloader-intuition)

- **Chapter 3: Coding Attention Mechanisms**
  - [Comparing Efficient Multi-Head Attention Implementations](ch03/02_bonus_efficient-multihead-attention/mha-implementations.ipynb)
  - [Understanding PyTorch Buffers](ch03/03_understanding-buffers/understanding-buffers.ipynb)

- **Chapter 4: Implementing a GPT Model From Scratch**
  - [FLOPs Analysis](ch04/02_performance-analysis/flops-analysis.ipynb)
  - [KV Cache](ch04/03_kv-cache)
  - [Attention Alternatives](ch04/#attention-alternatives)
    - [Grouped-Query Attention](ch04/04_gqa)
    - [Multi-Head Latent Attention](ch04/05_mla)
    - [Sliding Window Attention](ch04/06_swa)
    - [Gated DeltaNet](ch04/08_deltanet)
  - [Mixture-of-Experts (MoE)](ch04/07_moe)

- **Chapter 5: Pretraining on Unlabeled Data**
  - [Alternative Weight Loading Methods](ch05/02_alternative_weight_loading/)
  - [Pretraining GPT on the Project Gutenberg Dataset](ch05/03_bonus_pretraining_on_gutenberg)
  - [Adding Bells and Whistles to the Training Loop](ch05/04_learning_rate_schedulers)
  - [Optimizing Hyperparameters for Pretraining](ch05/05_bonus_hparam_tuning)
  - [Building a User Interface to Interact With the Pretrained LLM](ch05/06_user_interface)
  - [Converting GPT to Llama](ch05/07_gpt_to_llama)
  - [Memory-efficient Model Weight Loading](ch05/08_memory_efficient_weight_loading/memory-efficient-state-dict.ipynb)
  - [Extending the Tiktoken BPE Tokenizer with New Tokens](ch05/09_extending-tokenizers/extend-tiktoken.ipynb)
  - [PyTorch Performance Tips for Faster LLM Training](ch05/10_llm-training-speed)
  - [LLM Architectures](ch05/#llm-architectures-from-scratch)
    - [Llama 3.2 From Scratch](ch05/07_gpt_to_llama/standalone-llama32.ipynb)
    - [Qwen3 Dense and Mixture-of-Experts (MoE) From Scratch](ch05/11_qwen3/)
    - [Gemma 3 From Scratch](ch05/12_gemma3/)
    - [Olmo 3 From Scratch](ch05/13_olmo3/)
    - [Tiny Aya From Scratch](ch05/15_tiny-aya/)
    - [Qwen3.5 From Scratch](ch05/16_qwen3.5/)
  - [Chapter 5 with other LLMs as Drop-In Replacement (e.g., Llama 3, Qwen 3)](ch05/14_ch05_with_other_llms/)
- **Chapter 6: Finetuning for classification**
  - [Additional Experiments Finetuning Different Layers and Using Larger Models](ch06/02_bonus_additional-experiments)
  - [Finetuning Different Models on the 50k IMDb Movie Review Dataset](ch06/03_bonus_imdb-classification)
  - [Building a User Interface to Interact With the GPT-based Spam Classifier](ch06/04_user_interface)
- **Chapter 7: Finetuning to follow instructions**
  - [Dataset Utilities for Finding Near Duplicates and Creating Passive Voice Entries](ch07/02_dataset-utilities)
  - [Evaluating Instruction Responses Using the OpenAI API and Ollama](ch07/03_model-evaluation)
  - [Generating a Dataset for Instruction Finetuning](ch07/05_dataset-generation/llama3-ollama.ipynb)
  - [Improving a Dataset for Instruction Finetuning](ch07/05_dataset-generation/reflection-gpt4.ipynb)
  - [Generating a Preference Dataset With Llama 3.1 70B and Ollama](ch07/04_preference-tuning-with-dpo/create-preference-data-ollama.ipynb)
  - [Direct Preference Optimization (DPO) for LLM Alignment](ch07/04_preference-tuning-with-dpo/dpo-from-scratch.ipynb)
  - [Building a User Interface to Interact With the Instruction-Finetuned GPT Model](ch07/06_user_interface)

More bonus material from the [Reasoning From Scratch](https://github.com/rasbt/reasoning-from-scratch) repository:

- **Qwen3 (From Scratch) Basics**
  - [Qwen3 Source Code Walkthrough](https://github.com/rasbt/reasoning-from-scratch/blob/main/chC/01_main-chapter-code/chC_main.ipynb)
  - [Optimized Qwen3](https://github.com/rasbt/reasoning-from-scratch/tree/main/ch02/03_optimized-LLM)

- **Evaluation**
  - [Verifier-Based Evaluation (MATH-500)](https://github.com/rasbt/reasoning-from-scratch/tree/main/ch03)
  - [Multiple-Choice Evaluation (MMLU)](https://github.com/rasbt/reasoning-from-scratch/blob/main/chF/02_mmlu)
  - [LLM Leaderboard Evaluation](https://github.com/rasbt/reasoning-from-scratch/blob/main/chF/03_leaderboards)
  - [LLM-as-a-Judge Evaluation](https://github.com/rasbt/reasoning-from-scratch/blob/main/chF/04_llm-judge)
- **Inference Scaling**
  - [Self-Consistency](https://github.com/rasbt/reasoning-from-scratch/blob/main/ch04/01_main-chapter-code/ch04_main.ipynb)
  - [Self-Refinement](https://github.com/rasbt/reasoning-from-scratch/blob/main/ch05/01_main-chapter-code/ch05_main.ipynb)

- **Reinforcement Learning** (RL)
  - [RLVR with GRPO From Scratch](https://github.com/rasbt/reasoning-from-scratch/blob/main/ch06/01_main-chapter-code/ch06_main.ipynb)


<br>
&nbsp;

## Questions, Feedback, and Contributing to This Repository


I welcome all sorts of feedback, best shared via the [Manning Forum](https://livebook.manning.com/forum?product=raschka&page=1) or [GitHub Discussions](https://github.com/rasbt/LLMs-from-scratch/discussions). Likewise, if you have any questions or just want to bounce ideas off others, please don't hesitate to post these in the forum as well.

Please note that since this repository contains the code corresponding to a print book, I currently cannot accept contributions that would extend the contents of the main chapter code, as it would introduce deviations from the physical book. Keeping it consistent helps ensure a smooth experience for everyone.


&nbsp;
## Citation

If you find this book or code useful for your research, please consider citing it.

Chicago-style citation:

> Raschka, Sebastian. *Build A Large Language Model (From Scratch)*. Manning, 2024. ISBN: 978-1633437166.

BibTeX entry:

```
@book{build-llms-from-scratch-book,
  author       = {Sebastian Raschka},
  title        = {Build A Large Language Model (From Scratch)},
  publisher    = {Manning},
  year         = {2024},
  isbn         = {978-1633437166},
  url          = {https://www.manning.com/books/build-a-large-language-model-from-scratch},
  github       = {https://github.com/rasbt/LLMs-from-scratch}
}
```

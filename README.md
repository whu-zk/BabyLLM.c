<h1 align="center">  🚀 5天徒手拆解 GPT：纯 C 语言推理引擎挑战赛（⚠️ Alpha内测版 ） </h1>

> [!CAUTION]
> ⚠️ Alpha内测版本警告：此为早期内部构建版本，尚不完整且可能存在错误，欢迎大家提Issue反馈问题或建议。

> **“What I cannot create, I do not understand.” — Richard Feynman**

*在这个到处是 PyTorch 和庞大显卡的时代，我们要反其道而行之。我们将剥离所有复杂的框架，只用**最原始的 C 语言**，在你的笔记本 CPU 上唤醒一个拥有 1500 万参数的大模型。*

*我们将实现一个精简版的 Transformer Decoder 推理内核，让它在你的终端里一字一句地为你写故事。*

---

## 🌟 为什么参加这个挑战？

1.  **击碎黑盒焦虑**：不再满足于调用 `openai.Chat` API。你会亲手写下矩阵乘法的每一行循环，理解 LLM 到底是如何“思考”的。
2.  **极简主义的胜利**：不需要 GPU，不需要安装几 GB 的 CUDA 环境。一个 `gcc` 编译器，就是你全部的武器。
3.  **底层思维重构**：学习内存映射 (mmap)、缓存局部性 (Cache Locality) 以及 KV Cache 优化，这些是顶尖 AI 工程师的必备直觉。

---

## 项目受众

*注：这里写你的项目所面向的受众，本项目能给他们带来什么，对他们的基础能力要求有哪些*

## 在线阅读
https://datawhalechina.github.io/repo-template

## 目录
|  章节名   | 简介 | 状态 |
|  ----  | ---- | ---- |
| [第1章  **加载大脑**](https://github.com/datawhalechina/repo-template/blob/main/docs/chapter1)  | 实现权重文件的 `mmap` 与 Header 解析，成功打印出模型超参数 | ✅ |
| [第2章 **算力的心脏**](https://github.com/datawhalechina/repo-template/blob/main/docs/chapter2)  | 编写 `MatMul` (矩阵乘法) 与 `RMSNorm`，通过算子精度验证测试 | 🚧 |
| [第3章 **灵魂的连接** ](https://github.com/datawhalechina/repo-template/blob/main/docs/chapter3)  | 实现 `Multi-Head Attention` (多头注意力)，理解 Q,K,V 向量的交织 | 🚧 |
| [第4章 **记忆与循环**] | 编写 `Inference Loop` 并加入 `KV Cache`,推理速度提升 5x 以上 | 🚧 |
| [第5章 **对话与采样**] | 实现 `Top-p` 采样，让模型开始讲故事,**[最终作品]** 笔记本流畅跑通 AI | 🚧 |

## 贡献者名单

| 姓名 | 职责 | 简介 |
| :----| :---- | :---- |
| 小明 | 项目负责人 | 一个理想主义者 |
| 小红 | 第1章贡献者 | 小明的朋友 |
| 小强 | 第2章贡献者 | 小明的朋友 |

*注：表头可自定义，但必须在名单中标明项目负责人*

## 参与贡献

- 如果你发现了一些问题，可以提Issue进行反馈，如果提完没有人回复你可以联系[保姆团队](https://github.com/datawhalechina/DOPMC/blob/main/OP.md)的同学进行反馈跟进~
- 如果你想参与贡献本项目，可以提Pull Request，如果提完没有人回复你可以联系[保姆团队](https://github.com/datawhalechina/DOPMC/blob/main/OP.md)的同学进行反馈跟进~
- 如果你对 Datawhale 很感兴趣并想要发起一个新的项目，请按照[Datawhale开源项目指南](https://github.com/datawhalechina/DOPMC/blob/main/GUIDE.md)进行操作即可~

## 关注我们

<div align=center>
<p>扫描下方二维码关注公众号：Datawhale</p>
<img src="https://raw.githubusercontent.com/datawhalechina/pumpkin-book/master/res/qrcode.jpeg" width = "180" height = "180">
</div>

## LICENSE

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。

*注：默认使用CC 4.0协议，也可根据自身项目情况选用其他协议*

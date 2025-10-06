---
title: 认知科学笔记#5：深度学习，更深刻的解答还是更深刻的疑问
date: 2025-01-30 18:25:12
tags:
---

物理符号系统虽然理论上简洁优美、十分诱人，但在比如模式识别、自然语言处理、计算机视觉等传统上认为的智能工作，实践上取得空前成功却是人工神经网络，学习模式由算法给出，诸如监督学习、深度学习（无监督学习）、强化学习。

监督学习利用后向传播，从监督者的反馈信号向后调整网络的参数。这种算法可以在已经结构化的数据中提取模式。

深度学习模拟的是哺乳动物的视觉系统。视觉系统从外侧膝状体LGN开始，到初级视觉皮层V1再到五级视觉皮层V5，不同的层级处理不同层次的视觉信号，比如从下层信号中判断中央野中是否存在拐角。这种多层次处理使得学习非结构化的数据特别有效，比如 feature engineering 使用 autoencoder 

//我不是搞技术的我真的不想写了

强化学习既不是监督学习，也不是非监督学习；它模拟多巴胺回路，对应接受的反馈信号不是对或者错，而是最大化反馈给予的收益。

//CNN, LLM


</br></br>

深度学习在时间上的成功，让人感到人工智能的实现似乎胜利在望。但其实在一些关键方面，目前的人工智能仍然表现出低于人类的能力。我们来讨论这其中的一些理论和哲学问题。

首先是实践上的问题。 Rosenfeld, et al* 发现目前最好的的深度学习计算机视觉系统一旦遇到场景中有反常物体就会失败。在语境感知方面，人类擅长在场景中合并新的数据并且知道新物品带来新问题。但这些实践上的问题也不能过分鼓吹，人类也经常做一些类似机器的不太聪明的事。

---

\* https://www.quantamagazine.org/machine-learning-confronts-the-elephant-in-the-room-20180920/
https://arxiv.org/abs/1808.03305


其次，人工智能的感觉问题。正如 Turing 引用的反对所说，

>Not until a machine can write a sonnet or compose a concerto because of thoughts and emotions felt … No mechanism could feel (and not merely artificially signal) pleasure at its successes, grief when its valves fuse …*

但是我们可以回应，就算感觉问题得到认可，对于智能来说也是无关的。智能和感觉是完全不同的方面，完全可以有智能但没有情感。比如对反社会者(sociopath)的标准解读即是有智能但缺乏同情心。

哲学上区分两种意识，一是作为觉察的意识，指接触到信息，二是作为现象质的经验的意识，比如疼痛的感觉，一副绿色图像的经验，Block N. **将此称为现象意识。机器可能缺乏第二种意识，但第一种意识很可能是没问题的。

---

\* Turing. Computing machinery and intelligence. Mind 59 (1950), 433-460. [Objection #4, from Professor Jefferson Lister]

** Block. On a Confusion about a Function of Consciousness. Behavior and Brain Science 18 (1995).

再次，意识难题。一个信息处理机器如何出现现象意识，或者现象意识的性质如何用脑的物理性质描述被称为意识难题。计算一般是没有意识的，我们可以想象一台机器人有一个痛觉程序，能在检测到手臂受伤后大叫一声，却没有任何感觉。人类身上也有被称作「盲视」的例子*。盲视主体的视觉皮层有损伤，主体报告没有任何视觉经验，但却在视觉识别任务中表现得比随机更好。研究者猜测这是因为存在没有意识的视觉信息处理，即有数据的表征，但没有对之有意识的觉察。

现象意识的视角不仅面临死局而且似乎过于粗糙，当代其他的理论视角试图给出新的希望。

---

\* Weisenkrantz. Blindsight: A Case Study & Implications (1989). 又见 De Gelder, Vroomen, Pourtois, Weiskrantz. Nonconscious recognition of affect in the absense of striate cortex. Neuroreport 10 (1999):3759-63.

又次，Searle 中文房间。


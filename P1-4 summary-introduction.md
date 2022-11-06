# summary

- 将神经元插入到电路系统里可能比纯硅电路有提升

- 使用 active inference via the free evergy principle(FEP), 观察到了学习过程

- 实验表示了 closed-loop structured feedback in eliciting learning over time 的重要性
- ![img](/img/feedbackSystems.png)

- 培养组织 接收少量自己对外界影响结果的回馈信号后 有自我组织能力



# Introduction

- 生物计算的优越性 被研究了很多 （kumar et al. 2020）

- 但体外没有支持third-order complexity 的人工系统。所以没法重现BNN的复杂
- 这个文章培养的神经组织可以通过 内部适应过程 来 回应外部sensory impression　

- Instantiating SBIs (synthetic biological intelligence) 有关于
  - 药物筛选 
  - 单细胞到多细胞的神经活动
  - 神经元-硅 计算平台
  - BNN（a biological neuronal network）表现的机器学习方法
- 一个智能系统的sentient behaviour （ (goal-directed) ）的形成需要两个过程
  - 能够通过观测 学习 外界如何影响内部。 通过行为 学习 内部如何影响外部
  - 能够通过内部感官状态 推断出 什么时候采取什么行动 和 行动对外界的影响 

- 为解决上面的第一个需求， 做了一个low-latency closed-loop feedback system。来模拟环境与BNN的交流。 前人工作 显示了  电生理学-闭环-反馈-系统的可塑性， 有一个在小鼠体内显示反馈和BNN功能发展的工作。
- 为解决上面的第二个需求， 借鉴了active inference via the free evergy principle (FEP)。这个theory是试图解释智能是如何生成的。智能系统会缩小预期与感知的差距。BNN对外界持有 ’belief‘ ， 学习的过程就是更新这些 ’belief‘ 或者改变外界环境来让探测结果跟符合预期。通过上面的这个说法，可以在神经细胞做出错误行为时，给予随机杂乱的电信号。前人有在体外用fep执行blind-source separation的工作。文章通过通过信号模拟”Pong“游戏，期望BNN会调节内部活动来避免与杂乱反馈有关的行为。
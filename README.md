# Reinforcement Learning for Computer Architecture Security

## AutoCAT: Reinforcement Learning for Automated Exploration of Cache-Timing Attacks

### Mulong Luo*, Wenjie Xiong*, Geunbae Lee, Yueying Li, Xiaomeng Yang, Amy Zhang, Yuandong Tian, Hsien-Hsin S. Lee, and G. Edward Suh


**Abstract** The aggressive performance optimizations in mod- ern microprocessors can result in security vulnerabilities. For example, timing-based attacks in processor caches can steal secret keys or break randomization. So far, finding cache-timing vulnerabilities is mostly performed by human experts, which is inefficient and laborious. There is a need for automatic tools that can explore vulnerabilities given that unreported vulnerabilities leave the systems at risk.
In this paper, we propose AutoCAT, an automated exploration framework that finds cache timing-channel attack sequences using reinforcement learning (RL). Specifically, AutoCAT formu- lates the cache timing-channel attack as a guessing game between an attack program and a victim program holding a secret. This guessing game can thus be solved via modern deep RL techniques. AutoCAT can explore attacks in various cache configurations without knowing design details and under different attack and victim program configurations. AutoCAT can also find attacks to bypass certain detection and defense mechanisms. In particular, AutoCAT discovered StealthyStreamline, a new attack that is able to bypass performance counter-based detection and has up to a 71% higher information leakage rate than the state- of-the-art LRU-based attacks on real processors. AutoCAT is the first of its kind in using RL for crafting microarchitectural timing-channel attack sequences and can accelerate cache timing- channel exploration for secure microprocessor designs.

[\[paper\]](paper/HPCA2023_revision-39.pdf) [\[code\]](https://github.com/facebookresearch/AutoCAT)


## MACTA: A Multi-agent Reinforcement Learning Approach for Cache Timing Attacks and Detection 

### Jiaxun Cui, Xiaomeng Yang*, Mulong Luo*, Geunbae Lee*, Peter Stone, Hsien-Hsin S. Lee, Benjamin Lee, G. Edward Suh, Wenjie Xiong*, Yuandong Tian*

**Abstract** Security vulnerabilities in computer systems raise serious concerns as computers process an unprecedented amount of private and sensitive data today. Cache-timing attacks pose an important practical threat as they have been shown to be able to effectively breach many protection mechanisms in today's system. However, the current detection of cache timing attacks relies heavily on heuristics and expert knowledge, which can lead to brittleness and inability to adapt to new attacks. To mitigate these problems, we develop a two-player environment for cache-timing attacks and detection, and leverage the idea of population-based multi-agent reinforcement learning (MARL) to train both attackers and detectors. Our empirical results indicate that, without any manual input from security experts, the trained attacker is able to act more stealthily while the trained detector can generalize to \emph{unseen} attacks and is less exploitable to high-bandwidth attacks. Furthermore, in this environment, we found that agents equipped with a Transformer encoder substantially outperform agents with multi-layer perceptrons encoders, which has been commonly used in RL tasks, suggesting that Transformer may learn better representations in such real-world tasks. 

[\[paper\]](https://openreview.net/pdf?id=CDlHZ78-Xzi)

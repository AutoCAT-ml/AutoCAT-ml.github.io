# AutoCAT: Reinforcement Learning for Automated Exploration of Cache-Timing Attacks

### Mulong Luo*, Wenjie Xiong*, Geunbae Lee, Yueying Li, Xiaomeng Yang, Amy Zhang, Yuandong Tian, Hsien-Hsin S. Lee, and G. Edward Suh


The aggressive performance optimizations in mod- ern microprocessors can result in security vulnerabilities. For example, timing-based attacks in processor caches can steal secret keys or break randomization. So far, finding cache-timing vulnerabilities is mostly performed by human experts, which is inefficient and laborious. There is a need for automatic tools that can explore vulnerabilities given that unreported vulnerabilities leave the systems at risk.
In this paper, we propose AutoCAT, an automated exploration framework that finds cache timing-channel attack sequences using reinforcement learning (RL). Specifically, AutoCAT formu- lates the cache timing-channel attack as a guessing game between an attack program and a victim program holding a secret. This guessing game can thus be solved via modern deep RL techniques. AutoCAT can explore attacks in various cache configurations without knowing design details and under different attack and victim program configurations. AutoCAT can also find attacks to bypass certain detection and defense mechanisms. In particular, AutoCAT discovered StealthyStreamline, a new attack that is able to bypass performance counter-based detection and has up to a 71% higher information leakage rate than the state- of-the-art LRU-based attacks on real processors. AutoCAT is the first of its kind in using RL for crafting microarchitectural timing-channel attack sequences and can accelerate cache timing- channel exploration for secure microprocessor designs.



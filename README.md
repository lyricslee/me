### 1. Deep Reinforcement Learning
- [0. RL 资料整理](rl/00_RL_course.html)
- [1. RL 强化学习入门](rl/ALL_IntroRL.html)
- [2. DQN all in one](rl/ALL_DQN.html)
- [3. PG all in on](rl/ALL_PG.html)
- [4. DDPG all in one](rl/ALL_DDPG.html)

#### 1.1 UCB RL note(知乎谢天)
- [1. UCB_1-6 Policy Gradient](rl/04_UCB_1-6.html)
- [2. UCB_7-10 Q-learning & Advanced PG](rl/05_UCB_7-10.html)
- [3. UCB_11 Model-Based RL](rl/06_UCB_11.html)
- [4. UCB_16  Inverse Reinforcement Learning](rl/07_UCB_16.html)

### 2. Tools
- [linux shell](linux/01_linux_cmd.html)
- [python tools](linux/02_python_tools.html)
- [tools](linux/03_tools.html)

### 3. Reserch
- [music 合成方法总结](paper/music_papers.html)
- [lyrics generation 歌词生成方法总结](paper/03 lyrics_generation.html)

### 4. Deep Learning
- [1. TCN seq-to-seq model](ml/04_TCN.html)
- [2. tensorflow introduce](ml/02_tensorflow.html)
- [3. NLP 课程笔记](ml/06_NLP_Notebook.html)

### 5. Machine Learning
- [1. KL cross_entry](ml/03_KL_cross_entroy.html)
- [2. UnsupervisedLearning K-mean](ml/unsupervised_learning.html)
- [3. Regression_PCA_PCR](ml/MLRegressionPCAPCR.html)
- [4. kernel _trick](ml/kernel _trick.html)
- [5. Deep Learning](ml/DeepLearning.html)
- [6. Decision Tree](ml/DecisionTree.html)
- [7. PLA: Perceptrons Learning Alogrithm](ml/PLA.html)

### 7. Autonomous System
- [1. BFS_DFS_Heuristics](rl/08_BFS_DFS_Search.html)
- [2. Policy iteration And Value iteration](rl/09_PI_VI.html)

### A: Useful Repository

repository | details
---|---
[cs188](https://github.com/lyricslee/CS188) | answers about homework in CS188 course 
[torndado_demo](https://github.com/lyricslee/torndado_demo) |  simple http server based on the Tornado Web Framework 
[begin_lua](https://github.com/lyricslee/begin_lua)  | a beginners guide to lua programming in chinese
[55000lyrics_rhyme_annotation](https://github.com/lyricslee/55000lyrics_meter_annotation) | Add rhyme and meter annotation into dataset [55000+ Song Lyrics kaggle](https://www.kaggle.com/mousehead/songlyrics), using the python [pronouncing](https://pronouncing.readthedocs.io/en/latest/).

### B: 强化学习算法列表

分类 | 名称 | 说明
---|---|---
DQN | DQN | 记忆池+固定目标网络
DQN | Double DQN | 将动作选择和价值估计分开，避免价值过高估计
DQN | Dueling DQN |将Q值分解为状态价值和优势函数，得到更多有用信息
DQN | Prioritized Replay Buffer | 将经验池中的经验按照优先级进行采样
DQN | Multi-Step Learnin | 多步执行使得目标价值估计更为准确
DQN | Distributional DQN(Categorical DQN) | 得到价值分布
DQN | NoisyNet| 增强模型的探索能力
DQN | Rainbow: all in one | 六种方法进行了一个整合
DQN | Deep Recurrent Q-Learning for Partially Observable MDPs| DQN 和 LSTM 的结合
PG | TNPG | 共轭梯度法 求解自然策略梯度 (NPG) 
PG | ACKTR | 完全正交的Kronecker-factor技术 求解自然策略梯度 (NPG) 
PG | TRPO | 相比TNPG，TRPO由于有了一个检验手段和线搜索，能承受更大的步长。
PG | PPO-clip | 对优势的估计进行一个截断，限制了新策略空间的范围。
PG | GAE | discounted rewards to estimate the advantage
PG | Actor-Critic | 结合了 Policy Gradient (Actor) 和 Function Approximation (Critic) 的方法
PG | A3C | A3C （基于 actor-critic）算法是并行算法，可以有效的利用多核。
DDPG | DDPG | 连续空间 Actor-Critic + DQN 的结合
DDPG | TD3 | 改善 DDPG Q 值 overestimate 导致 policy 在错误的 Q 值 errors 上 exploit 的问题
DDPG | SAC |  entropy regularization(exploration-exploitation trade-off)

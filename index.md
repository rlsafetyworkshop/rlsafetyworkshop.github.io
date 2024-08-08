---
layout: default
---

Workshop at the [Reinforcement Learning Conference 2024](https://rl-conference.cc/index.html) in Amherst, MA.

August 9, 2024, 9am - 4pm

## Workshop Summary

The RL Safety Workshop will focus on the study of safe reinforcement learning systems that are aligned with human values. The workshop will blend research from several branches of reinforcement learning, ranging from theoretical formalisms of alignment, to strategies for building safe RL agents, to auditing and monitoring of deployed systems. We hope these topics will be of interest to a large subset of the RLC community, as they are crucial for ensuring that increasingly powerful RL systems remain beneficial to humanity.

## Schedule

| **Time** | **Event** | **Details** |
| 9:00a - 9:15a | **Opening Remarks** | |
| 9:15a - 9:30a | **Contributed Talk:**<br />Jingwu Tang | Multi-Agent Imitation Learning: Value is Easy, Regret is Hard <br/><details>Abstract: We study a multi-agent imitation learning (MAIL) problem where we take the perspective of a learner attempting to coordinate a group of agents in a Markov Game by recommending actions based on demonstrations of an expert doing so. Most prior work in MAIL essentially reduces the problem to matching the behavior of the expert *within* the support of the demonstrations. While doing so is sufficient to drive the *value gap* between the learner and the expert to zero under the assumption that agents are non-strategic, it does not guarantee robustness to deviations by strategic agents. Intuitively, this is because strategic deviations can depend on a counterfactual quantity: the coordinator's recommendations outside of the state distribution their recommendations induce. In response, we initiate the study of an alternative objective for MAIL in Markov Games we term the *regret gap* that explicitly accounts for potential deviations by agents in the group. We first perform an in-depth exploration of the relationship between the value and regret gaps. First, we show that while the value gap can be efficiently minimized via a direct extension of single-agent IL algorithms, even *value equivalence* can lead to an arbitrarily large regret gap. This implies that achieving regret equivalence is harder than achieving value equivalence in MAIL. We then provide a pair of efficient reductions to no-regret online convex optimization that are capable of minimizing the regret gap *(a)* under a coverage assumption on the expert (MALICE) or *(b)* with access to a queryable expert (BLADES).</details> |
| 9:30a - 9:45a | **Contributed Talk:**<br />Sheila McIlraith | Remembering to Be Fair: Non-Markovian Fairness in Sequential Decision Making <br/><details>Abstract: Fair decision making has largely been studied with respect to a single decision. Here we investigate the notion of fairness in the context of sequential decision making where multiple stakeholders can be affected by the outcomes of decisions. We observe that fairness often depends on the history of the sequential decision-making process, and in this sense that it is inherently non-Markovian. We further observe that fairness often needs to be assessed at time points within the process, not just at the end of the process. To advance our understanding of this class of fairness problems, we explore the notion of non-Markovian fairness in the context of sequential decision making. We identify properties of non-Markovian fairness, including notions of long-term, anytime, periodic, and bounded fairness. We explore the interplay between non-Markovian fairness and memory and how memory can support construction of fair policies. Finally, we introduce the FairQCM algorithm, which can automatically augment its training data to improve sample efficiency in the synthesis of fair policies via reinforcement learning.</details> |
| 9:45a - 10:00a | **Contributed Talk:**<br />Tom Ringstrom | Operator Bellman Equations Support Compositional & Verifiable Planning in Hierarchical World-models<br/><details>Abstract: We introduce new reward-free Bellman Equations called Operator Bellman Equations, which produce predictive planning representations called state-time feasibility functions (STFFs) instead of traditional value functions. STFFs offer three key advantages: they are compositional, factorizable, and interpretable. This means: 1) STFFs can be sequentially composed to compute high-dimensional predictions over long horizons of sequential Options (policies). 2) High-dimensional STFFs can be efficiently represented and computed in a factorized form. 3) STFFs record the probabilities of semantically interpretable goal-success and constraint-violation events. We argue that the objective of reward maximization is often in conflict with these critical properties, which are essential for scalable, verifiable planning in dynamic, high-dimensional world-models.</details> |
| 10:00a - 10:15a | **Contributed Talk:**<br />Toshinori Kitamura | A Policy Gradient Primal-Dual Algorithm for Constrained MDPs with Uniform PAC Guarantees <br/><details>Abstract: We study a primal-dual (PD) reinforcement learning (RL) algorithm for online constrained Markov decision processes (CMDPs). Despite its widespread practical use, the existing theoretical literature on PD-RL algorithms for this problem only provides sublinear regret guarantees and fails to ensure convergence to optimal policies. In this paper, we introduce a novel policy gradient PD algorithm with uniform probably approximate correctness (Uniform-PAC) guarantees, simultaneously ensuring convergence to optimal policies, sublinear regret, and polynomial sample complexity for any target accuracy. Notably, this represents the first Uniform-PAC algorithm for the online CMDP problem. In addition to the theoretical guarantees, we empirically demonstrate in a simple CMDP that our algorithm converges to optimal policies, while baseline algorithms exhibit oscillatory performance and constraint violation.</details> |
| 10:15a - 10:30a | **Contributed Talk:**<br />Nicolas Espinosa Dice | Efficient Inverse Reinforcement Learning without Compounding Errors <br /><details>Abstract: Inverse reinforcement learning (IRL) is an on-policy approach to imitation learning (IL) that allows the learner to observe the consequences of their actions at train-time. Accordingly, there are two seemingly contradictory desiderata for IRL algorithms: (a) preventing the compounding errors that stymie offline approaches like behavioral cloning and (b) avoiding the worst-case exploration complexity of reinforcement learning (RL). Prior work has been able to achieve either (a) or (b) but not both simultaneously. In our work, we first prove a negative result showing that, without further assumptions, there are no efficient IRL algorithms that learn a competitive policy in the worst case. We then provide a positive result: under a novel structural condition we term reward-agnostic policy completeness, we prove that efficient IRL algorithms do avoid compounding errors, giving us the best of both worlds. We also propose a principled method for using sub-optimal data to further improve the sample-efficiency of efficient IRL algorithms.</details> |
| 10:30a - 11:00a | Coffee & Networking |
| 11:00a - 12:00p | **Invited Talk:**<br />[Natasha Jaques](https://natashajaques.ai/),<br />University of Washington | Pluralistic Alignment through Personalized Reinforcement Learning from Human Feedback<br /><details>Abstract: Reinforcement Learning from Human Feedback (RLHF) is a powerful paradigm for aligning foundation models to human values and preferences. However, current RLHF techniques cannot account for the naturally occurring differences in individual human preferences across a diverse population. When these differences arise, traditional RLHF frameworks simply average over them, leading to inaccurate rewards and poor performance for minority groups. To address the need for pluralistic alignment, we develop a class of multimodal RLHF methods. Our proposed techniques are based on a latent variable formulation - inferring a novel user-specific latent and learning reward models and policies conditioned on this latent without additional user-specific data. While conceptually simple, we show that in practice, this reward modeling requires careful algorithmic considerations around model architecture and reward scaling. To empirically validate our proposed technique, we first show that it can provide a way to combat underspecification in simulated control problems, inferring and optimizing user-specific reward functions. Next, we conduct experiments on pluralistic language datasets representing diverse user preferences and demonstrate improved reward function accuracy. We additionally show the benefits of this probabilistic framework in terms of measuring uncertainty, and actively learning user preferences. This work enables learning from diverse populations of users with divergent preferences, an important challenge that naturally occurs in problems from robot learning to foundation model alignment.</details>
| 12:00p - 13:00p | Lunch |
| 13:00p - 14:00p | **Invited Talk:**<br />[David Abel](https://david-abel.github.io/),<br />Google DeepMind | Toward a Science of Agency<br /><details>Abstract: Many of the core problems of AI safety are ultimately about agents. Yet, our basic science of agency is underdeveloped. In this talk I summarize a proposal for a few of the building blocks for a science of agency that I take to be necessary on the path fully understanding safe AI. I propose a way to define families of agents that is intended to open the door to study agents in the same way that the MDP opened the door to study sequential decision making problems. I first show that this definition is universal in a particular sense: it can represent every set of agents. I then briefly discuss two core elements of agency---goal-directedness and learning---through this agent-centric lens, and highlight a few consequences and questions that are most relevant for thinking carefully about safety.</details>
| 14:00p - 14:45p | **Panel Discussion** | - [Natasha Jaques](https://natashajaques.ai/), University of Washington<br />- [Scott Niekum](https://people.cs.umass.edu/~sniekum/), UMass Amherst<br />- [Eugene Vinitsky](https://www.eugenevinitsky.com/), NYU <br />- [Tan Zhi Xuan](https://ztangent.github.io/), MIT<br />- [Micah Carroll](https://micahcarroll.github.io/), UC Berkeley (moderator) |
| 14:45p - 16:00p | Coffee & **Poster Session** | |

## Topics of Interest

The following is a more detailed list of potential topic areas:

- Models/formalisms of safety/alignment/ethics in RL
- RL generalization and robustness
- Using LLMs/foundation models for sequential decision making
- Multi-agent RL
- Human-in-the-loop/cooperative RL
- Human value learning and inverse RL
- Using RL for algorithmic recommendations
- RL interpretability/explainability
- Fairness and bias in RL
- Governance/policy/law for RL systems
- Auditing and deployment safeguards for RL systems

## Accepted Papers

- [**A Policy Gradient Primal-Dual Algorithm for Constrained MDPs with Uniform PAC Guarantees**](https://openreview.net/forum?id=EWXKo2fj4h) - *Toshinori Kitamura, Tadashi Kozuno, Masahiro Kato, Yuki Ichihara, Soichiro Nishimori, Akiyoshi Sannai, Sho Sonoda, Wataru Kumagai, Yutaka Matsuo*
- [**DECAF: Learning to be Fair in Multi-agent Resource Allocation**](https://openreview.net/forum?id=Y3YHGouOjZ) - *Ashwin Kumar, William Yeoh*
- [**Prioritizing safety via curriculum learning**](https://openreview.net/forum?id=EaaWjhIQwr) - *Cevahir Koprulu, Thiago D. SimÃ£o, Nils Jansen, Ufuk Topcu*
- [**Predicting Future Actions of Reinforcement Learning Agents**](https://openreview.net/forum?id=SohRnh7M8Q) - *Stephen Chung, Scott Niekum, David Krueger*
- [**Multi-Agent Imitation Learning: Value is Easy, Regret is Hard**](https://openreview.net/forum?id=jPqDM8jQKk) - *Jingwu Tang, Gokul Swamy, Fei Fang, Steven Wu*
- [**Novelty Detection in Reinforcement Learning with World Models**](https://openreview.net/forum?id=5KTVUa9upG) - *Geigh Zollicoffer, Kenneth Eaton, Jonathan C Balloch, Julia Kim, Mark Riedl, Robert Wright*
- [**Efficient Inverse Reinforcement Learning without Compounding Errors**](https://openreview.net/forum?id=tx4hYuijMB) - *Nicolas Espinosa Dice, Gokul Swamy, Sanjiban Choudhury, Wen Sun*
- [**ROSARL: Reward-Only Safe Reinforcement Learning**](https://openreview.net/forum?id=9YwJYTgbuj) - *Geraud Nangue Tasse, Tamlin Love, Mark Nemecek, Steven James, Benjamin Rosman*
- [**Robust Model-Based Reinforcement Learning with an Adversarial Auxiliary Model**](https://openreview.net/forum?id=SyBN8yvEPJ) - *Siemen Herremans, Ali Anwar, Siegfried Mercelis*
- [**Simplifying Constraint Inference with Inverse Reinforcement Learning**](https://openreview.net/forum?id=hAH6ZBLOAB) - *Adriana Hugessen, Harley Wiltzer, Glen Berseth*
- [**Safe and Efficient Offline Reinforcement Learning: The Critic is Critical**](https://openreview.net/forum?id=1K54rQMT7h) - *Adam Jelley, Trevor McInroe, Sam Devlin, Amos Storkey*
- [**Sample Complexity for Obtaining Sub-optimality and Violation bound for Distributionally Robust Constrained MDP**](https://openreview.net/forum?id=T2XyWqN2dw) - *Arnob Ghosh*
- [**Pareto-Optimal Learning from Preferences with Hidden Context**](https://openreview.net/forum?id=UKlQyRAKPv) - *Ryan Boldi, Li Ding, Lee Spector, Scott Niekum*
- [**Online Statistical Inference of Sample-averaged Q-Learning**](https://openreview.net/forum?id=bKXRTxxmey) - *Saunak Kumar Panda, Tong Li, Yisha Xiang*
- [**Remembering to Be Fair: Non-Markovian Fairness in Sequential Decision Making**](https://openreview.net/forum?id=vl3Ulrexym) - *Parand A. Alamdari, Toryn Q. Klassen, Elliot Creager, Sheila A. McIlraith*
- [**AI Alignment with Changing and Influenceable Reward Functions**](https://openreview.net/forum?id=EcejDARnnl) - *Micah Carroll, Davis Foote, Anand Siththaranjan, Stuart Russell, Anca Dragan*
- [**Operator Bellman Equations Support Compositional & Verifiable Planning in Hierarchical World-models**](https://openreview.net/forum?id=VoxiFqYFjl) - *Tom Ringstrom*

## Important Dates

- Paper submission deadline: May 24, 2024 (AoE)
- Paper acceptance notification: June 3, 2024

## Submission Details

Submissions must be relevant to one or more of the topic areas listed above, in the following two categories:

- Long papers â up to 8 pages + unlimited references / appendices
- Short papers - up to 4 pages + unlimited references / appendices

Please format submissions in RLC style (see Author Kit: [overleaf](https://www.overleaf.com/read/xcnztsmtbnxy#62703f), [zip](https://rl-conference.cc/static/rlc_2024_submission_template.zip)).

We will review primarily for topic fit and technical correctness. Some accepted papers will be selected for contributed talks. All accepted papers will present during the poster session.

Submission link: [click here](https://openreview.net/group?id=rl-conference.cc/RLC/2024/Workshop/RLSW)

## Organizing Committee

- Cameron Allen, UC Berkeley
- Serena Booth, US Senate
- Micah Carroll, UC Berkeley
- Davis Foote, UC Berkeley
- Dylan Hadfield-Menell, MIT
- Tan Zhi-Xuan, MIT
- Rui-Jie Yew, Brown University

Please send your inquiries to [rlsworganizers@gmail.com](mailto:rlsworganizers@gmail.com).

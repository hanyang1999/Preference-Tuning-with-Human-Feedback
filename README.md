# Preference Tuning Research Resources
This is the list of tutorials, workshops, papers, and resources on RL and preference tuning (with or without human feedback) research, which includes most (if not all) papers discussed in our survey paper: [Preference Tuning with Human Feedback on Language, Speech, and Vision Tasks: A Survey](https://arxiv.org/pdf/2409.11564).

The paper list will be updated over the time. You are always more than welcome to send a pull request for updating the list and be one of the contributors! 

## Table of Contents

- [🚀 Highlights](#-highlights)

- [📑 Research Papers](#-research-papers)
  - [Online Methods](#online-methods)
    - [RLHF](#rlhf)
      - [PPO](#ppo)
      - [REINFORCE](#reinforce)
    - [Online DPO](#online-dpo)
    - [Nash-Learning](#nash-learning)
    - [SFT-like](#sft-like)
    - [Multi-Modal Models](#multi-modal-models-online)
  - [Offline Methods](#offline-methods)
    - [Offline DPO](#offline-dpo)
    - [Multi-Modal Models](#multi-modal-models-offline)
  - [Combination](#combination)
  - [Sampling-Agnostic](#sampling-agnostic)

- [Blogs and Links](#Blogs-and-Links)
  
- [Other Related Survey Papers](#Other-Related-Survey-Papers)

- [Citation](#Citation)

## 🚀 Highlights
- 2025/04/30 Our survey paper is officially published by Journal of Artificial Intelligence Research (JAIR).
- 2025/04/07 We release the third version of our survey paper! We include more related relevant references e.g. [GRPO](https://arxiv.org/abs/2402.03300).
- 2025/02/07 Our paper is accepted by the Journal of Artifical Intelligence Research.

### Papers Table of Contents


### Online Methods

#### RLHF

- ##### PPO

  - **Ouyang, et al. (2022)** *Training Language Models to Follow Instructions with Human Feedback*. NeurIPS 2022 [[Paper](https://arxiv.org/abs/2203.02155)]
  - **Bai, et al. (2022)** *Constitutional AI: Harmlessness from AI Feedback*. arXiv [[Paper](https://arxiv.org/abs/2212.08073)]
  - **Wu, et al. (2023)** *Pairwise Proximal Policy Optimization: Harnessing Relative Feedback for LLM Alignment*. arXiv [[Paper](https://arxiv.org/abs/2310.00212)]
  - **Chakraborty, et al. (2024)** *MaxMin-RLHF: Towards Equitable Alignment of Large Language Models with Diverse Human Preferences*. arXiv [[Paper](https://arxiv.org/abs/2402.08925)]
  - **Dang, et al. (2024)** *RLHF Can Speak Many Languages: Unlocking Multilingual Preference Optimization for LLMs*. arXiv [[Paper](https://arxiv.org/abs/2407.02552)]
  - **Dong, et al. (2024)** *RLHF Workflow: From Reward Modeling to Online RLHF*. arXiv [[Paper](https://arxiv.org/abs/2405.07863)]

- ##### REINFORCE

  - **Li, et al. (2023)** *ReMax: A Simple, Effective, and Efficient Reinforcement Learning Method for Aligning Large Language Models*. ICML 2023 [[Paper](https://arxiv.org/abs/2310.10042)]
  - **Ahmadian, et al. (2024)** *Back to Basics: Revisiting REINFORCE Style Optimization for Learning from Human Feedback in LLMs*. arXiv [[Paper](https://arxiv.org/abs/2402.14740)]
  - **Shao, et al. (2024)** *DeepSeekMath: Pushing the Limits of Mathematical Reasoning in Open Language Models*. arXiv [[Paper](https://arxiv.org/abs/2402.03300)]

- #### Online DPO

  - **Xu, et al. (2023)** *Some Things Are More Cringe Than Others: Preference Optimization with the Pairwise Cringe Loss*. arXiv [[Paper](https://arxiv.org/abs/2312.16682)]
  - **Guo, et al. (2024)** *Direct Language Model Alignment from Online AI Feedback*. arXiv [[Paper](https://arxiv.org/abs/2402.04792)]
  - **Chen, et al. (2024)** *OPTune: Efficient Online Preference Tuning*. arXiv [[Paper](https://arxiv.org/abs/2406.07657)]
  - **Yuan, et al. (2024)** *Self-Rewarding Language Models*. arXiv [[Paper](https://arxiv.org/abs/2401.10020)]

- #### Nash-Learning

  - **Munos, et al. (2023)** *Nash Learning from Human Feedback*. arXiv [[Paper](https://arxiv.org/abs/2312.00886)]
  - **Wu, et al. (2024)** *Self-Play Preference Optimization for Language Model Alignment*. arXiv [[Paper](https://arxiv.org/abs/2405.00675)]

- #### SFT-like

  - **Dong, et al. (2023)** *RAFT: Reward rAnked FineTuning for Generative Foundation Model Alignment*. arXiv [[Paper](https://arxiv.org/abs/2304.06767)]
  - **Gulcehre, et al. (2023)** *Reinforced Self-Training (ReST) for Language Modeling*. arXiv [[Paper](https://arxiv.org/abs/2308.08998)]
  - **Yuan, et al. (2023)** *RRHF: Rank Responses to Align Language Models with Human Feedback Without Tears*. arXiv [[Paper](https://arxiv.org/abs/2304.05302)]
  - **Mukobi, et al. (2023)** *SuperHF: Supervised Iterative Learning from Human Feedback*. arXiv [[Paper](https://arxiv.org/abs/2310.16763)]

#### Multi-Modal Models (Online)

- ##### Diffusion

  - **Prabhudesai, et al. (2023)** *Aligning Text-to-Image Diffusion Models with Reward Backpropagation*. arXiv [[Paper](https://arxiv.org/abs/2310.03739)]
  - **Black, et al. (2024)** *Training Diffusion Models with Reinforcement Learning*. ICLR 2024 [[Paper](https://openreview.net/forum?id=QD-bvv3CO2)]
  - **Fan, et al. (2024)** *Reinforcement Learning for Fine-tuning Text-to-Image Diffusion Models*. NeurIPS 2024 [[Paper](https://arxiv.org/abs/2402.08498)]
  - **Clark, et al. (2023)** *Directly Fine-tuning Diffusion Models on Differentiable Rewards*. arXiv [[Paper](https://arxiv.org/abs/2309.17400)]
  - **Deng, et al. (2024)** *PRDP: Proximal Reward Difference Prediction for Large-scale Reward Finetuning of Diffusion Models*. CVPR 2024 [[Paper](https://arxiv.org/abs/2401.01517)]
  - **Xu, et al. (2024)** *ImageReward: Learning and Evaluating Human Preferences for Text-to-Image Generation*. NeurIPS 2024 [[Paper](https://arxiv.org/abs/2304.05977)]

- ##### VLLM

  - **Chen, et al. (2024)** *Reinforcement Learning for Fine-tuning Text-to-speech Diffusion Models*. arXiv [[Paper](https://arxiv.org/abs/2405.14632)]
  - **Zhang, et al. (2024)** *HIVE: Harnessing Human Feedback for Instructional Visual Editing*. CVPR 2024 [[Paper](https://arxiv.org/abs/2303.09618)]
  - **Sun, et al. (2023)** *Aligning Large Multimodal Models with Factually Augmented RLHF*. arXiv [[Paper](https://arxiv.org/abs/2309.14525)]
  - **Yu, et al. (2024)** *RLHF-V: Towards Trustworthy MLLMs via Behavior Alignment from Fine-Grained Correctional Human Feedback*. CVPR 2024 [[Paper](https://arxiv.org/abs/2312.15666)]
  - **Liang, et al. (2024)** *Rich Human Feedback for Text-to-Image Generation*. CVPR 2024 [[Paper](https://arxiv.org/abs/2402.05145)]

- ### Offline Methods

  - **Zhuang, et al. (2023)** *Behavior Proximal Policy Optimization*. arXiv [[Paper](https://arxiv.org/abs/2302.11312)]

- #### Multi-Modal Models (Offline)
  
  - **Wallace, et al. (2024)** *Diffusion Model Alignment Using Direct Preference Optimization*. CVPR 2024 [[Paper](https://arxiv.org/abs/2311.12908)]
  - **Zhou, et al. (2024)** *Aligning Modalities in Vision Large Language Models via Preference Fine-tuning*. arXiv [[Paper](https://arxiv.org/abs/2402.11411)]

- #### Offline DPO
  
  - **Rafailov, et al. (2024)** *Direct Preference Optimization: Your Language Model is Secretly a Reward Model*. NeurIPS 2024 [[Paper](https://arxiv.org/abs/2305.18290)]
  - **Chen, et al. (2024)** *Low-Redundant Optimization for Large Language Model Alignment*. arXiv [[Paper](https://arxiv.org/abs/2406.12606)]
  - **Guo, et al. (2024)** *Controllable Preference Optimization: Toward Controllable Multi-Objective Alignment*. arXiv [[Paper](https://arxiv.org/abs/2402.19085)]
  - **Tang, et al. (2024)** *Generalized Preference Optimization: A Unified Approach to Offline Alignment*. arXiv [[Paper](https://arxiv.org/abs/2402.05749)]
  - **Azar, et al. (2024)** *A General Theoretical Paradigm to Understand Learning from Human Preferences*. AISTATS 2024 [[Paper](https://proceedings.mlr.press/v238/azar24a.html)]
  - **Ethayarajh, et al. (2024)** *KTO: Model Alignment as Prospect Theoretic Optimization*. arXiv [[Paper](https://arxiv.org/abs/2402.01306)]
  - **Amini, et al. (2024)** *Direct Preference Optimization with an Offset*. arXiv [[Paper](https://arxiv.org/abs/2402.10571)]
  - **Hong, et al. (2024)** *ORPO: Monolithic Preference Optimization without Reference Model*. arXiv [[Paper](https://arxiv.org/abs/2403.07691)]
  - **Song, et al. (2024)** *Preference Ranking Optimization for Human Alignment*. AAAI 2024 [[Paper](https://arxiv.org/abs/2309.07864)]
  - **Park, et al. (2024)** *Disentangling Length from Quality in Direct Preference Optimization*. arXiv [[Paper](https://arxiv.org/abs/2403.19159)]
  - **Chowdhury, et al. (2024)** *Provably Robust DPO: Aligning Language Models with Noisy Feedback*. arXiv [[Paper](https://arxiv.org/abs/2403.00409)]
  - **Kim, et al. (2024)** *sDPO: Don't Use Your Data All at Once*. arXiv [[Paper](https://arxiv.org/abs/2403.19270)]
  - **Chen, et al. (2024)** *Mallows-DPO: Fine-Tune Your LLM with Preference Dispersions*. arXiv [[Paper](https://arxiv.org/abs/2405.14953)]
  - **Zhao, et al. (2024)** *RainbowPO: A Unified Framework for Combining Improvements in Preference Optimization*. arXiv [[Paper](https://arxiv.org/abs/2410.04203)]
  - **Meng, et al. (2024)** *SimPO: Simple Preference Optimization with a Reference-free Reward*. arXiv [[Paper](https://arxiv.org/abs/2405.14734)]
  - **Li, et al. (2024)** *Preference Tuning For Toxicity Mitigation Generalizes Across Languages*. arXiv [[Paper](https://arxiv.org/abs/2406.16235)]
  - **Zhao, et al. (2023)** *SLiC-HF: Sequence Likelihood Calibration with Human Feedback*. arXiv [[Paper](https://arxiv.org/abs/2305.10425)]

- ### Combination

  - **Fakoor, et al. (2020)** *P3O: Policy-on Policy-off Policy Optimization*. UAI 2020 [[Paper](https://proceedings.mlr.press/v124/fakoor20a.html)]
  - **Zhong, et al. (2024)** *DPO Meets PPO: Reinforced Token Optimization for RLHF*. arXiv [[Paper](https://arxiv.org/abs/2404.18922)]
  
- ### Sampling-Agnostic

  - **Zheng, et al. (2024)** *Weak-to-Strong Extrapolation Expedites Alignment*. arXiv [[Paper](https://arxiv.org/abs/2404.16792)]

- ## Blogs and Links
  - <b>Weng (2024)</b> <i>Reward Hacking</i>. Lilian Weng Blog <a href="https://lilianweng.github.io/posts/2024-11-28-reward-hacking/">[Blog]</a>

- ## Other Related Survey Papers
  - <b>opendilab</b> <i>awesome-RLHF</i>. <a href="https://github.com/opendilab/awesome-RLHF">[Github]</a>

- ## Citation

  If our paper and this github repo are helpful, you are more than welcome to cite our papers through the following bib tex:

  ```
  @article{winata2025preference,
    title={Preference tuning with human feedback on language, speech, and vision tasks: A survey},
    author={Winata, Genta Indra and Zhao, Hanyang and Das, Anirban and Tang, Wenpin and Yao, David D and Zhang, Shi-Xiong and Sahu, Sambit},
    journal={Journal of Artificial Intelligence Research},
    volume={82},
    pages={2595--2661},
    year={2025}
  }
  ```

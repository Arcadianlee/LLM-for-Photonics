## LLM-for-Photonics
Leveraging LLMs to design and optimize nanophotonics

This is the repository for our paper: LLM helps design and optimize photonic crystal
surface emitting lasers, by Renjie Li et al. available at https://hal.science/hal-04175312

![Screen Shot 2023-08-21 at 10 17 53](https://github.com/Arcadianlee/LLM-for-Photonics/assets/76676601/6a001b53-a9c1-4a96-a538-1a0824c59bba)

## Abstract:<br/>
Conventional design and optimization of Photonic Crystal Surface Emitting Lasers
(PCSEL) usually requires expert knowledge in semiconductor physics and optimization
algorithms, which is also known as the inverse design problem. However,
with the trend towards automation and depersonalization of the entire integrated
circuits (IC) industry, the conventional method, with the drawback of being relatively
labor-intensive and sub-optimal, warrants further refinement. This technical
dilemma remained until the emergence of Large Language Models (LLMs), such
as OpenAI’s ChatGPT and Google’s Bard. This paper explores the possibility of
applying LLMs to machine learning-based design and optimization of PCSELs.
Specifically, we utilize GPT-3.5 and GPT-4. By simply having conversations, GPT
assisted us with writing Finite Difference Time Domain (FDTD) simulation code
and deep reinforcement learning code to acquire the optimized PCSEL solution,
spanning from the proposition of ideas to the realization of algorithms. Given that
GPT will perform better when given detailed and specific questions, we break down
the PCSEL design problem into a series of sub-problems and converse with GPT
by posing open-ended heuristic questions rather than definitive commands. This
paper shows that LLMs, such as ChatGPT, can guide the nanophotonic design and
optimization processes, on both the conceptual and technical level, and we propose
new human–AI co-design strategies and show their practical implications. We
achieve a significant milestone for the first step towards an automated end-to-end
nanophotonic design and production pipeline.


## Algothims and software used:<br/>
Deep Q learning (DQN) and MIT Meep (https://meep.readthedocs.io/en/latest/)

Pytorch was used as the ML library and OpenAI gym was used for building the envs.<br/>
Meep FDTD was used as the environment for simulating nanophotonics.

## File structure
    .
    ├── ...
    ├── optim_PhC.py            # main scripts
    │   ├── envs                # RL environment scripts
    │   ├── src                 # source scripts written w/ meep (e.g. meep1.py)
    ├── README.md               # Readme file
    ├── Chat1_concept.txt       # Conversation sequences with gpt
    └── ...



## citation
If you used our code/idea for your research, please consider citing the paper as:
![Screen Shot 2023-08-07 at 13 43 25](https://github.com/Arcadianlee/LLM-for-Photonics/assets/76676601/c4f3ad7c-3c4f-4dec-a8ee-0dc23d872658)


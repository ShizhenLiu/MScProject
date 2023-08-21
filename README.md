# MScProject
This repository is the solution for the "Large Language Model-Driven Hierarchical Agents for the Open-World" project.

# Project Introduction
Reinforcement learning (RL) has been instrumental in driving successes in closed, well-defined gaming environments, such as the Atari 2600. Yet, open-world games like Minecraft introduce new complexities due to their dynamic and intricate settings, deviating from conventional RL challenges. Despite the potential avenues explored by models like Video Pre-Training (VPT) and insights from hierarchical structures, there remains a substantial gap in creating agents that mirror human-like gameplay. The primary contributions of this research revolve around the fusion of large language models (LLMs) with RL agents for optimized task performance in Minecraft's intricate environment. By integrating a decision-making component driven by an LLM with specialized sub-agents, our model fosters a flexible and economically efficient approach to varied tasks. Essential features include scalable architecture for complex tasks without extensive retraining and the integration of a scheduler mechanism. This work not only addresses the intricate world of Minecraft but also paves the way for utilizing LLMs in RL, offering avenues for tackling challenges in other complex open-world settings.

# How to run
To run the notebook, you need to install both MineRL v1.0 and MineRL v0.4. Please be aware that the version of 'gym' may affect the installation of MineRL. If you're unable to install it, check if the 'gym' version is 0.25.2. If you're unable to execute the remaining cells in the notebook after installation, try restarting the runtime. Link to the MineRL project: https://github.com/minerllabs/minerl.

To execute the task, run the LLM_planner_with_GPT.ipynb file. The weight files for the sub-agents can be found at this link: [link not provided]. Ensure the notebook file and weight files are in the same folder named "content". Please run the cells in the order: Install->Scenario->Sub-agents->Planner->Run Task. The Install step takes about half an hour. Restart the runtime once the Install cell has finished executing.

If you wish to train the sub-agents, run the train_subagents.ipynb file. The required dataset for training can be referred to at: https://minerl.readthedocs.io/en/v0.4.4/environments/index.html. This notebook file also includes code for fine-tuning and knowledge distillation. Note that training is under MineRL v0.4, while testing the sub-agents must be done under MineRL v1.0.

We have only tested the code to run stably on Google CoLab and cannot guarantee stable execution on other IDEs.

If you have questions about the content of the Minecraft environment, please refer to https://minecraft.fandom.com/wiki/Minecraft_Wiki


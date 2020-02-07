
# Weights & Biases x Qualcomm - SpaceInvaders Challenge

We’re excited to announce the W&B [SpaceInvaders](https://gym.openai.com/envs/SpaceInvaders-v0/) Challenge, a reinforcement learning competition. Your goal is to train reinforcement learning agents in OpenAI's gym environment. The contestants with the top 3 scores will receive prizes and be invited to share their solutions with the community. The challenge is open to Qualcomm employees.

![](https://thumbs.gfycat.com/CookedFriendlyAntarcticfurseal-size_restricted.gif)
## Getting Started

**To enter the competition:**
- [Sign up](https://app.wandb.ai/login?signup=true) for W&B.
- Download the [baseline notebook](https://colab.research.google.com/drive/1lz_qVRc44bjkWvi-0sWuJppM5DJ-64Q4) to get started. PLEASE NOTE: This notebook contains code for loading the gym environment, preprocessing data, and calculating & logging the cumulative average reward metrics. 
- Submit your test runs [here](https://app.wandb.ai/wandb/spaceinvaders-challenge/benchmark/submit). See submissions instructions below.

New to online contests with W&B, reinforcement learning and/or OpenAI gym? No problem! We have posted resources to help you understand the W&B Python libraries, supported frameworks, suitable algorithms and some articles on neural networks below under the Resources section.

Questions? Use the `#qualcomm-competition` [slack channel](http://bit.ly/wandb-forum), or email <qualcommcontest@wandb.com>.

## Submissions
You may submit your entries [here](https://app.wandb.ai/wandb/spaceinvaders-challenge/benchmark/submit). You'll need a Weights & Biases account to make submissions.

Each run must include the following files:

- Model file generated by [wandb.save()](https://docs.wandb.com/library/python/save)
- Model training script (.py file or notebook)
- Any other files necessary to recreate the model
- A LICENSE.md file

**Please ensure that you log your model file and all files necessary to recreate the model in your run using [wandb.save()](https://docs.wandb.com/library/python/save). Without this, we will be unable to evaluate your model.**

Also please ensure that your code is not in a public repo, but is visible to us by adding 'lavanyashukla' as a collaborator to your repo. We will use the model saved in the submitted run to recreate the model and evaluate it across the 5 random seeds.

## Evaluation
Your objective is to maximize the best 100-episode average reward. This means your model will play the game for 100 episodes, and we will calculate a running average of the cumulative reward gained as each of the episodes is played. After 100 episodes, this cumulative running average will be your final score for the run.

We encourage you to submit as many runs as you like. To verify results, we will pick the top 5-10 submissions as ranked by the evaluation metric (best 100-episode average reward), and run these agents through the SpaceInvaders environment. We will evaluate how the agents do across 5 randomly generated seeds. This means, your agent will be run for 100 episodes with 5 different seeds and generate a best 100-episode average reward for each seed. We will take the average of these scores to get the final best 100-episode average reward.

Entries will be ranked from highest to lowest by the best 100-episode average reward received across the 5 seeds.

The Best W&B Report will be awarded to the individual who creates the best writeup explaining their model architecture, training process and results achieved. You can find sample W&B reports [here](https://app.wandb.ai/stacey/deep-drive/reports/Find-Humans-and-Vehicles-in-Dashboard-Scenes---Vmlldzo0NDA1Ng), [here](https://app.wandb.ai/dewald123/Liu_pytorch/reports/Solar-Flare-Prediction--Vmlldzo0MDYwNw) and [here](https://app.wandb.ai/stacey/estuary/reports/Distributed-Training--Vmlldzo1MTE0MA).

## Prizes
- First place - $1000
- Second place - $500
- Third place - $200
- Best W&B Report - $500


## Timeline
- February 6 - Competition Announced
- April 10 - Deadline for final submissions
- May 1 - Winners announced
- TBD - Contest Retrospective Webinar

The deadlines are at 11:59PM on the days mentioned above PST.


## Leaderboard
You can find the [leaderboard here](https://app.wandb.ai/wandb/spaceinvaders-challenge/benchmark/leaderboard).
  
## Rules
- You are free to use any framework you feel comfortable in and submit as many times a day as you wish.
- We don’t allow the use of automated machine learning tool(s) in this competition.
- You may only have one account per individual.
- You can share small snippets of the code online or in our slack community, but not the full solution - until the submission deadline has passed.
- You can submit as many runs as you like.

## Resources
- [Weights & Biases Docs](https://docs.wandb.com/library/python)
- [Playing Atari with Deep Reinforcement Learning](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf)
- [How RL agents learn to play Atari games](https://www.youtube.com/watch?v=rbsqaJwpu6A&feature=youtu.be&t=9m55s)
- [Overcoming catastrophic forgetting in neural nets - Paper](https://deepmind.com/blog/article/enabling-continual-learning-in-neural-networks)
- [Frame Skipping and Pre-Processing for Deep Q-Networks on Atari 2600 Games](https://danieltakeshi.github.io/2016/11/25/frame-skipping-and-preprocessing-for-deep-q-networks-on-atari-2600-games/)
- [The A3C Algorithm](https://arxiv.org/pdf/1602.01783.pdf)
- [The Deep Q-learning algorithm](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf)

![](https://paper-attachments.dropbox.com/s_B99EA5A7E2C3A6034DED3BDBEF344777271F2DEC10A3548BB2647BA045D43B29_1580852759900_image.png)

## About Weights & Biases
Weights & Biases is an experiment tracking platform for deep learning. Import our python package into any training script with a few lines of code. Explore how hyperparameters affect model performance in realtime, record and visualize every detail of your research, compare metrics across thousands of runs, reproduce and quickly share findings with collaborators.

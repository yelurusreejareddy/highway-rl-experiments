# highway-rl-experiments

Systematic comparison of PPO, DQN, and A2C across three autonomous driving
environments using Stable-Baselines3 and Highway-Env.

## Environments

- highway-v0 - multi-lane highway driving (easy)
- roundabout-v0 - roundabout navigation (medium)
- intersection-v0 - intersection crossing (hard)

## Approach

Each algorithm was run in two phases:

- Baseline - default hyperparameters across all 3 environments
- Tuned - hyperparameter search (learning rate, batch size, gamma, epsilon) per environment

## Files Included

- highway_rl_experiments.ipynb - main notebook with training, tuning, and evaluation
- project_report.pdf - full write-up with analysis and conclusions
- baseline_videos/ - 9 episode recordings (3 algorithms x 3 environments, baseline)
- ppo_tuned_highway_video.mp4, dqn_tuned_highway_video.mp4, a2c_tuned_highway_video.mp4
- ppo_tuned_roundabout_video.mp4, dqn_tuned_roundabout_video.mp4, a2c_tuned_roundabout_video.mp4
- ppo_tuned_intersection_video.mp4, dqn_tuned_intersection_video.mp4, a2c_tuned_intersection_video.mp4
- baseline_checkpoints/ - saved models for all baseline runs
- tuned_checkpoints/ - saved models for all tuned runs
- json_metrics/ - training metrics for all algorithm-environment combinations
- baseline_charts/ - performance comparison charts per environment
- all_charts_ultimate.png - combined results overview

## Libraries

Python, Stable-Baselines3, Gymnasium, Highway-Env, PyTorch, matplotlib, numpy

## Goal

To understand how PPO, DQN, and A2C differ in performance and stability across
environments of increasing complexity, and how hyperparameter tuning affects each.

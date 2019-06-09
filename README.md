# Google-Project-Dopamine-Data-Visualization
Dopamine is a research framework for fast prototyping of reinforcement learning algorithms. It aims to fill the need for a small, easily grokked codebase in which users can freely experiment with wild ideas (speculative research).



In this colab we illustrate how to load and visualize the logs data produced by Dopamine.

Dopamine is a research framework for fast prototyping of reinforcement learning algorithms. It aims to fill the need for a small, easily grokked codebase in which users can freely experiment with wild ideas (speculative research).

Our design principles are:

    Easy experimentation: Make it easy for new users to run benchmark experiments.
    Flexible development: Make it easy for new users to try out research ideas.
    Compact and reliable: Provide implementations for a few, battle-tested algorithms.
    Reproducible: Facilitate reproducibility in results. In particular, our setup follows the recommendations given by [Machado et al. (2018)][machado].

In the spirit of these principles, this first version focuses on supporting the state-of-the-art, single-GPU Rainbow agent ([Hessel et al., 2018][rainbow]) applied to Atari 2600 game-playing ([Bellemare et al., 2013][ale]). Specifically, our Rainbow agent implements the three components identified as most important by [Hessel et al.][rainbow]:

    n-step Bellman updates (see e.g. [Mnih et al., 2016][a3c])
    Prioritized experience replay ([Schaul et al., 2015][prioritized_replay])
    Distributional reinforcement learning ([C51; Bellemare et al., 2017][c51])

For completeness, we also provide an implementation of DQN ([Mnih et al., 2015][dqn]). For additional details, please see our documentation.

More info on Dopamine: https://github.com/google/dopamine

In this colab we illustrate how to load and visualize the logs data produced by Dopamine, which are stored as pickle files. We demonstrate how to compare against the provided baselines using the plotting tools included with Dopamine, as well as how to plot the data using custom utilities (like matplotlib).

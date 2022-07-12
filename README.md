# NeurIPS 2022: MineRL BASALT Competition Intro Track Baseline Submission Kit

[![Discord](https://img.shields.io/discord/565639094860775436.svg)](https://discord.gg/BT9uegr)

This repository is the MineRL BASALT 2022 Competition Intro Track **baseline submission template**.

MineRL BASALT Intro Track is designed to help you get familiar with the submission system and MineRL. Your task is to create an agent which can obtain a diamond shovel, starting from a random, fresh world.

The baseline agent gets a diamond about 10% of the time and sometimes crafts a diamond pickaxe. Your task is to make it craft a diamond shovel.

See [the AICrowd competition page](https://www.aicrowd.com/challenges/neurips-2022-minerl-basalt-competition) for further information.

## Setting up

Install [MineRL v1.0.0](https://github.com/minerllabs/minerl) (or newer) and the requirements for [OpenAI VPT](https://github.com/openai/Video-Pre-Training).

Download the RL from Early Game model [.weights](https://openaipublic.blob.core.windows.net/minecraft-rl/models/rl-from-early-game-2x.weights) and [.model](https://openaipublic.blob.core.windows.net/minecraft-rl/models/2x.model) files for the OpenAI VPT model.

Place these files under `data` to match the following structure:

```
├── data
│   └── VPT-models
│       ├── 2x.model
│       └── rl-from-early-game-2x.weights
```


## Visualizing the model

To watch the baseline agent play, uncomment the `env.render()` line in `test.py` and run the following command:
```
python test.py
```
This will run a single short episode. If you want to see complete episodes, set `debug` to `false` in `aicrowd.json`.

## How to Submit a Model on AICrowd.

To submit this baseline agent follow the [submission instructions](https://github.com/minerllabs/basalt_intro_track_2022_competition_submission_template), but use this repo instead of the starter kit repo.

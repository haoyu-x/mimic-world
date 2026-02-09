# MimicWorld Benchmark

## Evaluation

### Visual Quality
- Open loop rollout
- Vision metrics

### Physical Quality
- Closed loop rollout
- Policy evaluation inside the world model

## Setup

```bash
git clone https://github.com/ARISE-Initiative/robomimic.git
git clone --branch v1.5.1 https://github.com/ARISE-Initiative/robosuite.git
```
## Installation
- [Robomimic Installation](https://robomimic.github.io/docs/introduction/installation.html)
- [Robosuite Installation](https://robosuite.ai/docs/installation.html)



## Resources
- [Robomimic Dataset Download](https://robomimic.github.io/docs/datasets/robomimic_v0.1.html)
- [Dataset Playback](https://robomimic.github.io/docs/tutorials/dataset_contents.html)
- [Data Collection Doc](https://robomimic.github.io/docs/datasets/robosuite.html)
- [Dataset Collection](https://github.com/ARISE-Initiative/robosuite/blob/v1.5.1/robosuite/scripts/collect_human_demonstrations.py)
- [Data Convertion](https://github.com/ARISE-Initiative/robomimic/blob/master/robomimic/scripts/conversion/convert_robosuite.py)
- [Environment Initialization](https://robomimic.github.io/docs/modules/environments.html)
- [Rollout](https://github.com/ARISE-Initiative/robomimic/blob/master/robomimic/utils/train_utils.py#L275)
- [Rollout](https://github.com/ARISE-Initiative/robomimic/blob/master/robomimic/scripts/run_trained_agent.py)

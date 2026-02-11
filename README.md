# MimicWorld Benchmark

## Evaluation

### Dataset design
- Play data
- Expert + noise replay
- Policy rollout

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

## Dataset Pipeline

### 1. Download Raw Dataset

```bash
python robomimic/scripts/download_datasets.py \
    --tasks square \
    --dataset_types ph mh \
    --hdf5_types raw
```

### 2. Extract Observations from Raw Data

```bash
bash robomimic/scripts/extract_obs_from_raw_datasets.sh
```

### 3. Split Train and Validation

```bash
python robomimic/scripts/split_train_val.py \
    --dataset datasets/square/mh/image_v15.hdf5
```

## Resources

### Dataset
- [Robomimic Dataset Download](https://robomimic.github.io/docs/datasets/robomimic_v0.1.html)
- [Dataset Playback](https://robomimic.github.io/docs/tutorials/dataset_contents.html)

### Data Collection
- [Data Collection Doc](https://robomimic.github.io/docs/datasets/robosuite.html)
- [Dataset Collection Script](https://github.com/ARISE-Initiative/robosuite/blob/v1.5.1/robosuite/scripts/collect_human_demonstrations.py)
- [Data Conversion Script](https://github.com/ARISE-Initiative/robomimic/blob/master/robomimic/scripts/conversion/convert_robosuite.py)

### Environment & Rollout
- [Environment Initialization](https://robomimic.github.io/docs/modules/environments.html)
- [Rollout Utils](https://github.com/ARISE-Initiative/robomimic/blob/master/robomimic/utils/train_utils.py#L275)
- [Run Trained Agent](https://github.com/ARISE-Initiative/robomimic/blob/master/robomimic/scripts/run_trained_agent.py)
